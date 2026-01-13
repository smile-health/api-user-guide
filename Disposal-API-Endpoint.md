# Disposal API Endpoint

> ℹ️ Last updated: 12 Jan 2026

## Table of Contents
- [About](#about)
- [API Endpoint](#api-endpoint)

---

## About

The **Disposal API Endpoints** provides a comprehensive solution for managing disposal in web and 
mobile applications from disposal transactions, facilitating efficient disposal processing and 
tracking. This API supports functions such as viewing disposal lists, creating new disposals, 
viewing disposal details, sending disposals and receiving smooth disposal management within the system.

Receiver entities disposal shipments have two types of disposal: **self-disposal** and **disposal instruction**
(having integration to a waste management system). If an entity only has a waste management system (WMS), 
it can perform disposal instruction with WMS integration. If an entity only has independent disposal, 
it can perform independent disposal in SMILE.

Access to these functions is role-based, allowing users to interact with disposal according to their 
assigned permissions. This ensures secure data handling, integrated workflows, and efficient operational control.

The **Disposal API Endpoint** plays a key role in optimize disposal management, improving tracking 
accuracy, and increasing overall business efficiency.

---

## API Endpoint

| **Type** | **API URL** | **API Name** | **Web App** | **Mobile App** |
|----------|-------------|--------------|-------------|----------------|
| GET | /disposal/methods | Disposal Methods | ✔️ | ✔️ |
| GET | /disposal/shipment | Disposal Shipment List | ✔️ | ✔️ |
| GET | /disposal/shipment/xls | Export Disposal Shipment List | ✔️ | ❌ |
| GET | /disposal/shipment/{disposalId} | Disposal Shipment Detail | ✔️ | ✔️ |
| POST | /disposal/shipment | Create Disposal Shipment | ✔️ | ✔️ |
| GET | /disposal/shipment/{disposalId}/download | Download Disposal Shipment Memorandum | ✔️ | ❌ |
| POST | /disposal/shipment/{shipmentId}/comment | Create Comment Disposal Shipment | ✔️ | ✔️ |
| PUT | /disposal/shipment/{shipmentId}/accept | Fulfilled- Disposal Shipment | ✔️ | ✔️ |
| PUT | /disposal/shipment/{shipmentId}/cancel | Cancel Disposal - Disposal Shipment | ✔️ | ✔️ |
| GET | /disposal/self-disposal | Self-Disposal List | ✔️ | ✔️ |
| GET | /disposal/self-disposal/xls | Export Self-Disposal List | ✔️ | ❌ |
| POST | /disposal/self-disposal | Create Self-Disposal | ✔️ | ✔️ |
| GET | /disposal/instructions | Disposal Instructions List | ✔️ | ✔️ |
| GET | /disposal/instructions/types | Disposal Instructions Type | ✔️ | ✔️ |
| GET | /disposal/instructions/{id} | Disposal Instructions Detail | ✔️ | ✔️ |
| GET | /disposal/instructions/{id}/download | Download Disposal Instructions Handover Report Document | ✔️ | ❌ |
| POST | /disposal/instructions | Create Disposal Instructions | ✔️ | ✔️ |
| GET | /disposal/instructions/xls | Export Disposal Instructions List | ✔️ | ❌ |
| POST | /disposal/instructions/{id}/comment | Create Comment Disposal Instructions | ✔️ | ✔️ |
| GET | /entities | Get List Entities | ✔️ | ✔️ |
| GET | /entities/{id}/activities | Get List Activity Entity | ✔️ | ✔️ |
| GET | /entities/{id}/vendors | Get List Vendor Entity | ✔️ | ✔️ |
| GET | /disposal/stocks/detail | Disposal Stock Detail | ✔️ | ✔️ |

