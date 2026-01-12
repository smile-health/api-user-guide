# Order Service

> ℹ️ Last updated: 12 Jan 2026

## Table of Contents
- [About](#about)
- [Role Matrix](#role-matrix)

---

## About

**Order Service** provides users to manage order processes with procedural material 
movements within an entity in SMILE, with various order types supported. It also provides
a centralized order process, ensures streamlined and accurate handling of orders and
associated material flows, improving operational efficiency and overall effectiveness.

This service functionalities manage the ordering process and material movement in the 
system. This includes recording orders, tracking and updating status, checking orders for 
material stock availability and managing material allocation. This service offers multiple 
functionalities that can be performed by the user, such as View Order, Detail Order, 
Download Order Document, Create Request Order, Edit Order, Create Distribution Order, 
Create Return Order, Create Central Distribution, Create Relocation, and Update Order Status. 
Each functionality adhering to specific business rules and data requirements. Functionalities 
Overview Document provides a structured breakdown of these capabilities, serving as a reference 
for how the service operates and what features it offers. 

In addition, the Role Matrix Document governs user access within the Transaction Service. 
Different roles—such as Super Admin, Admin, Manager, and Operator—are assigned 
specific privileges based on their responsibilities. For instance, while Super Admin and 
Admin can access the system through the Web App, Manager have access to both Web
and Mobile platforms, and Operator are limited to the Mobile platform. The Role Matrix also 
defines whether a user has full control over specific features or is restricted to view-only access. 
By establishing clear access levels, the Role Matrix ensures security, accountability, and compliance 
within the system.

---

## Roles

Order service can be performed by these roles:
1. Super Admin
2. Admin
3. Manager
4. Operator
5. Manufacture
> ℹ️ For detailed information about features that can be performed by each role, please
> visit **Order Role Matrix**.

---

## Associated Components
To support these functionalities, the SMILE system is integrated with several essential components, including:
1. **Inventory**: Check inventory availability and allocate material;
2. **Procurement**: Receive yearly planning information from the supplier (third party) or higher-level entity;
3. **Shipping**: Notify when the order is ready for shipping;
4. **Demand vs Supply Monitoring**: Notify when an order is placed and/or cancelled;
5. **Transactions**: Triggers create transactions after shipping is received.

---

## System Data Architecture
> ℹ️ For detailed information on the Order System Architecture, go to the **System Data Architecture**.

## Special Notes
### Order Status Level
This service has order status level with appropriate tracking and validation. Each status 
determines which actions are available and which next statuses are allowed. Refer to the 
table below for a full breakdown of status transitions. 
| **From Status** | **Action** | **To Status** | **Notes** |
|----------|----------|----------|----------|
| 🔴 Cancelled | - | - | Terminal status – cannot be changed |
| ⚪ Draft | Validate | 🟡 Pending  | Proccess the order to pending |
| ⚪ Draft | Cancel Order | 🔴 Cancelled  | Cancel the order |
| 🟡 Pending  | Cancel Order | 🔴 Cancelled  | Ends the order early; no further actions allowed |
| 🟡 Pending  | Confirm Order | 🟠 Confirmed  | Proceeds to the next step in the order process |
| 🟠 Confirmed  | Cancel Order | 🔴 Cancelled  | Cancel the order |
| 🟠 Confirmed  | Cancel Confirmation | 🟡 Pending  | Revert the confirmation and the order status return to Pending |
| 🟠 Confirmed  | Allocate | 🟣 Allocated | Material’s stock is assigned and locked |
| 🟣 Allocated  | Cancel Order | 🔴 Cancelled  | Cancel the order |
| 🟣 Allocated  | Ship Order | 🔵 Shipped  | Order is being shipped; material’s stock becomes stock in transit |
| 🔵 Shipped  | Cancel Order | 🔴 Cancelled  | Cancel the order |
| 🔵 Shipped  | Receive Order | 🟢 Fulfilled | Order has been successfully delivered and marked as received |
| 🟢 Fulfilled | - | - | Terminal status – cannot be changed |

### Order Type
This service has several types of orders, such as: 

**Order**

- Performs request orders from the customer entity to the vendor entity with a bottom-up process
- The initial status order of this order type is **Pending**.
- The Integration system (example: SIHA, SITB, DIN, Biofarma) can create order.
- After the Integration system create order, the status order of this is **Draft**.

**Allocation**

For allocation types, there are two different allocation types, such as: 
1. ** Distribution**
   - Performs distribution order of materials from top-level entities to lower-level entities that are their distribution customers, with a top-down process
   - The initial status order of this order type is **Allocated**.

2. **Central Distribution **
   - Performs central distribution order of materials directly from the highest-level entity to a specific entity without passing through the top-down process. 
   - The initial status of this order is **Shipped**.

**Return**
- Performs the return order of materials from the lower-level entity (as the receipt of the order) to the top-level entity because the materials are not suitable, damaged, or not needed
- The initial status order of this order type is **Allocated**.

**Relocation**
- Performs relocation order of materials from the entity to at the same level entity
  (example from DKI Jakarta Province to West Java Province) because the materials are
  low stock, population growth, outbreak or other.
- The initial status order of this order type is **Pending**.
