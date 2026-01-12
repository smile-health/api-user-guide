# Order API Endpoint

> ℹ️ Last updated: 12 Jan 2026

## Table of Contents
- [About](#about)
- [API Endpoint](#api-endpoint)

---

## About

The **Order API Endpoints** provide a comprehensive solution for managing orders across web
and mobile applications, enabling efficient order processing and tracking. This API supports 
functionalities such as viewing the order list, creating new orders, viewing order details, and 
managing order statuses, ensuring smooth order management within the system.

Access to these functionalities is role-based, allowing users to interact with orders according 
to their assigned permissions. This ensures secure data handling, streamlined workflows, and 
efficient operational control.

The Order API Endpoints play a key role in optimizing order management, improving tracking 
accuracy, and enhancing overall business efficiency.

---

## API Endpoint

| **Type** | **API URL** | **API Name** | **Web App** | **Mobile App** |
|----------|-------------|--------------|-------------|----------------|
| GET | /order | Order List | ✔️ | ✔️ |
| GET | /order/delivery-types | Order Delivery Type | ✔️ | ✔️ |
| GET | /orders/counts | Order Status Count | ✔️ | ✔️ |
| GET | /orders/xls | Export Excel Order List | ✔️ | ❌ |
| GET | /orders/{id} | Order Detail | ✔️ | ✔️ |
| GET | /orders/{id}/request-letter/xls | Download Order Letter Document | ✔️ | ❌ |
| GET | /orders/{id}/nota-confirmation/xls | Download Order Confirmation Note Document | ✔️ | ❌ |
| GET | /orders/{id}/nota-batch/xls | Download Order Batch Note Documentn | ✔️ | ❌ |
| GET | /orders/{id}/sbbk/xls | Download Order SBBK Document | ✔️ | ❌ |
| GET | /orders/{id}/var/xls | Download Order VAR Document | ✔️ | ❌ |
| PUT | /orders/{id}/cancel | Cancel Order | ✔️ | ✔️ |
| PUT | /orders/{id}/confirms | Confirm | ✔️ | ✔️ |
| PUT | /orders/{id}/pendings | Pending | ✔️ | ✔️ |
| PUT | /orders/{id}/allocates | Allocate | ✔️ | ✔️ |
| PUT | /orders/{id}/ships | Ships | ✔️ | ✔️ |
| POST | /orders/{id}/order-item-stocks | Create Order Item Stock | ✔️ | ✔️ |
| PUT | /orders/{id}/order-item-stocks | Update Order Item Stock | ✔️ | ✔️ |
| POST | /orders/{id}/comments | Create Comment | ✔️ | ✔️ |
| POST | /orders/request | Create Request Order | ✔️ | ✔️ |
| POST | /orders/distribution | Create Distribution Order | ✔️ | ✔️ |
| POST | /orders/return | Create Return Order | ✔️ | ✔️ |
| POST | /orders/central-distribution | Create Central Distribution Order | ✔️ | ✔️ |
| POST | /orders/relocation | Create Relocation Order | ✔️ | ✔️ |
| GET | /order-reasons | Order Reason | ✔️ | ✔️ |
| GET | /entities | Get List Entities | ✔️ | ✔️ |
| GET | /entities/{id}/activities | Get List Activity Entity | ✔️ | ✔️ |
| GET | /entities/{id}/vendors | Get List Vendor Entity | ✔️ | ✔️ |
| GET | /stocks/entities | Stock List Entities | ✔️ | ✔️ |
| PUT | /orders/{id}/fulfilled | Fulfilled | ✔️ | ✔️ |
| PUT | /orders/{id}/validate | Validate | ✔️ | ✔️ |
| GET | /orders/{id}/integration-logs | Order Integration Logs | ✔️ | ✔️ |
| GET | /contract | Contract Number | ✔️ | ✔️ |

