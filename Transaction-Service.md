# Transaction Service

_Last updated: 12 Jan 2026_

## Table of Contents
- [About](#about)
- [Roles](#roles)
- [Associated Components](#associated-components)
- [System Data Architectures](#system-data-architecture)
- [Special Notes](#special-notes)
  - [Transaction Type](#transaction-type)


---

## About

**Transaction Service** is one of the core service of the system, **responsible for managing and 
recording all stock movements** while ensuring accurate inventory updates. It provides a structured 
mechanism to track and update stock levels in real-time, facilitating seamless coordination between 
different entities. Every recorded transaction is logged in a comprehensive ledger, ensuring 
traceability and supporting historical analysis. By maintaining accurate stock records, the service 
enhances operational efficiency and helps prevent discrepancies in inventory management.

This service functionalities define the scope of operations available within the system. These include 
recording stock movements, maintaining a transaction ledger, and updating inventory levels in real-time. 
The service offers multiple functionalities that can be performed by the user, such as Transaction List, 
Add Stock Transaction, Remove Stock Transaction, Discard Transaction, Cancellation of Discard Transaction, 
Issue Transaction, and Return from Health Facility Transaction. Each functionality adhering to specific 
business rules and data requirements. Functionalities Overview Document provides a structured breakdown of 
these capabilities, serving as a reference for how the service operates and what features it offers.

In addition, the Role Matrix Document governs user access within the Transaction Service. Different 
roles—such as Super Admin, Admin, Manager, and Operator—are assigned specific privileges based 
on their responsibilities. For instance, while Super Admin and Admin can access the system through 
the Web App, Manager have access to both Web and Mobile platforms, and Operator are limited to 
the Mobile platform. The Role Matrix also defines whether a user has full control over specific 
features or is restricted to view-only access. By establishing clear access levels, the Role Matrix 
ensures security, accountability, and compliance within the system.

---

## Roles

Transaction service can be performed by these roles:
- Super Admin
- Admin
- Manager
- Operator
For more information about features that each role can perform, please visit the **Transaction Role Matrix**.

---

## Associated Components

1. **Inventory**: Updates stock levels in real-time based on recorded transactions.
2. **Reuse**: Receives information when consumed stock is repurposed for reuse.
3. **Consumption**: Receives updates when allocated stock has been consumed.
4. **Disposal**: Tracks when discarded stock has been either disposed of or returned.
5. **Warehouse Inspections**: Receives alerts when discrepancies in stock are identified during audits, enabling prompt resolution. 

---

## System Data Architecture

For more information on the Inventory System Architecture, please visit the **System Data Architecture**.

---

## Special Notes

### Transaction Type

There are several transaction types can be performed in SMILE:
1. **Add Stock Transaction**: Used to increase stock due to discrepancies between the system's recorded stock and the actual stock based on specific reasons.
2. **Remove Stock Transaction**: Used to reduce stock due to discrepancies between the system's recorded stock and the actual stock based on specific reasons.
3. **Discard Transaction**: Used to record the disposal of materials, whether due to expiration, breakage, damage, or other reasons.
4. **Cancellation of Discard Transaction**: Used to cancel the discarded status of materials that have already been recorded in a Discard Transaction due
   to changes in the condition of the materials.
5. **Last Mile Transaction**: Used for transactions related to issuance of the material to be consumpted by the user purposes. The Last Mile Transaction
   needed several additional data to be recorded, such as Patient data, Patient ID data, Patient’s sequencial consumption data, etc.
6. **Return from Last Mile**: Used for transactions aimed at returning excess materials, whether used or unused, also the one that has been discarded, back to the vendor entity.
7. **Relocation Between Programs**: Used to relocation needed several additional material to activity other program. The material must have more than one assigned program.
