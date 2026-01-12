# Inventory Service

> ℹ️ Last updated: 12 Jan 2026

## Table of Contents
- [About](#about)
- [Roles](#roles)
- [Associated Components](#associated-components)
- [System Data Architectures](#system-data-architecture)
- [Special Notes](#special-notes)
  - [Stock Classification](#stock-classification)
  - [Stock Level Colour Legend](#stock-level-colour-legend)


---

## About

Inventory Service provides users with a comprehensive solution for tracking and managing the stock 
levels of all materials within SMILE. By ensuring that inventory levels are meticulously recorded and 
monitored, this service supports accurate stock management and upholds the integrity of the 
inventory system. This functionality is essential for maintaining transparency, reducing discrepancies, 
and ensuring seamless operations across the platform.

---

## Roles

Inventory service can be performed by these roles:
- Super Admin
- Admin
- Manager
- Operator
> ℹ️ For more information about features that each role can perform, please visit the **Inventory Role Matrix**.

---

## Associated Components

1. Inventory Tracking: Get stock conformity data from the inventory;
2. Orders: Maintain stock transfer process aligned with storage’s maximum capacity; allocate material from existing stock;
3. Transactions: Record stock data and stock transfer process (ideal). Record stock data and the stock transfer/consumption process (existing).

---

## System Data Architecture

> ℹ️ For more information on the Inventory System Architecture, please visit the **System Data Architecture**.

---

## Special Notes

### Stock Classification

There are several stock classifications in SMILE for operational business flow, such as:
1. Stock on Hand – The total quantity of material currently owned and physically available within an entity. Stock on Hand is the total of Available Stock and Allocated Stock;
2. Available Stock – Stock that is not reserved and can be used for operational business processes such as orders or transactions;
3. Allocated Stock – Stock that has been reserved or allocated for specific orders or transactions and is no longer available for other orders or transactions;
4. In-Transit Stock – The quantity of material that is on shipment between entities, no longer at the vendor or customer, and in the process of being delivered.

### Stock Level Colour Legend

A visual representation is included in the Inventory service as part of Inventory Tracking to help users determine the material’s stock level:
| **Status** | **Description** | **Condition** |
|------------|-----------------|---------------|
| (Red) Empty Stock | There is no material stock on the entity. | stock = 0 |
| (Yellow) Low Stock | The material’s stock level on the entity is below the minimum recommended stock threshold. | stock under minimum |
| (Green) On Range Stock | The material’s stock level on the entity is within the range of the minimum and maximum recommended stock threshold. | stok between minimum and maximum **or** stock min = 0 and max = 0 |
| (Blue) Overstock | The material’s stock level on the entity is above the maximum recommended stock threshold. | stock more than maximum |
