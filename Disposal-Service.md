# Disposal Service

> ℹ️ Last updated: 13 Jan 2026

## Table of Contents
- [About](#about)
- [Roles](#roles)
- [Associated Components](#associated-components)
- [System Data Architecture](#system-data-architecture)
- [Special Notes](#special-notes)
  - [Order Status Level](#order-status-level)
  - [Order Type](#order-type)

---

## About

Disposal Service provides users to manage the waste disposal process with procedural material movements 
and discard transactions within entities in SMILE. This service also provides a centralized 
disposal process, ensuring efficient and accurate handling of orders and related material flows, 
thereby improving overall operational efficiency and effectiveness.

This service function manages the disposal process and material movement within the system. 
This includes recording shipment disposal, shipment disposal, tracking and updating status, 
and recording disposal. There are three menus for this disposal feature, but users only need to use two 
of them. The first step is to create a disposal shipment to the top-level entity. Once the disposal 
shipment has been received by the recipient entity, the recipient entity can carry out the disposal. 
The final step is for the receiver entity to carry out the disposal, which can be of two types depending 
on the condition of the entity. If the receiver entity is have integrated with the Waste Management System (WMS), 
it can carry out the disposal in the Disposal Instructions feature. If the recipient entity is not have 
integrated with the Waste Management System (WMS), it can carry out the disposal in the Self-Disposal feature.

In addition, the Role Matrix Document governs user access within the Disposal Service. Different roles—such as 
Super Admin, Admin, Manager, and Operator—are assigned specific privileges based on their responsibilities. 
For instance, while Super Admin and Admin can access the system through the Web App, Manager have access to both 
Web and Mobile platforms, and Operator are limited to the Mobile platform. The Role Matrix also defines whether 
a user has full control over specific features or is restricted to view-only access. By establishing clear access levels, 
the Role Matrix ensures security, accountability, and compliance within the system.

---

## Roles

Order service can be performed by these roles:
1. Super Admin
2. Admin
3. Manager
4. Operator
> ℹ️ For detailed information about features that can be performed by each role, please
> visit **Disposal Role Matrix**.

---

## Associated Components
To support these functionalities, the SMILE system is integrated with several essential components, including:
1. Inventory: Check inventory total discard material;
2. Disposal: Send disposal instruction disposal data to WMS to wasted material and receive
   status wasted from WMS

---

## System Data Architecture
> ℹ️ For detailed information on the Order System Architecture, go to the **System Data Architecture**.

---

## Special Notes
### Disposal Shipment Status Level
This service has order status level with appropriate tracking and validation. Each status 
determines which actions are available and which next statuses are allowed. Refer to the 
table below for a full breakdown of status transitions. 
| **From Status** | **Action** | **To Status** | **Notes** |
|----------|----------|----------|----------|
| 🔴 Cancelled | - | - | Terminal status – cannot be changed |
| 🔵 Shipped  | Cancel Shipment | 🔴 Cancelled  | Cancel the disposal shipment |
| 🔵 Shipped  | Receive Shipment | 🟢 Fulfilled | Disposal shipment has been successfully delivered and marked as received |
| 🟢 Fulfilled | - | - | Terminal status – cannot be changed |

### Disposal Type
This service has several types of disposals, such as: 

**Self-Disposal**

- Perform disposal material by self-entity, when entity not have integration with WMS.
- Self-disposal have disposal method, such as:
   1. Landfill
      - Disposing of waste material by burying it in the ground after it has been crushed or
        mixed with other materials so that it cannot be recognized.
   2. Incineration / Pyrolysis
      - Material waste undergoes combustion or heating at high temperatures.
   3. Sterilization / Disinfection
      - Process of disposing material using physical (heat, radiation, thermal) or chemical (disinfectant) methods

**Disposal Instruction**

- Perform disposal material by WMS, when entity have integration with WMS.
- Disposal Instruction have disposal type, such as:
  1. Handed over to the Health Unit.
  2. BPOM/KEMENKES Test
