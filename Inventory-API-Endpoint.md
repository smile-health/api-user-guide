# Inventory API Endpoint

> ℹ️ Last updated: 12 Jan 2026

## Table of Contents
- [About](#about)
- [API Endpoint](#api-endpoint)

---

## About

The **Inventory Service API Endpoint** provides seamless access to real-time stock 
information across web and mobile applications, enabling efficient inventory tracking 
and management.

On the web app, Super Admins and Admins can view stock data across all entities. 
In contrast, on the mobile app, Managers and Operators can only access stock information 
for their assigned entity. This role-based access ensures data security and relevant 
inventory visibility for each user level.

The **Inventory Service API** plays a critical role in optimising stock monitoring, improving 
operational efficiency, and ensuring accurate inventory management across the organization.

---

## API Endpoint

| **Type** | **API URL** | **API Name** | **Web App** | **Mobile App** |
|----------|-------------|--------------|-------------|----------------|
| GET | /stocks | Stocks Lists | ✔️ | ✔️ |
| GET | /stocks/entities | Stock by Entity | ✔️ | ✔️ |
| GET | /stocks/details | Stock Detail | ✔️ | ✔️ |
| GET | /stocks?entity_id={entity_id}&with_details=1&material_id={material_id} | Stock Batch Detail | ✔️ | ✔️ |
| GET | /batches | Batches | ✔️ | ✔️ |
| GET | /stock-qualities | Stock Qualities List | ✔️ | ✔️ |
| GET | /stock-consumptions | Stock Consumption | ✔️ | ✔️ |
| GET | /stock-consumptions/detail | Stock Consumption Detail | ✔️ | ✔️ |
| GET | /stocks/xls | Stocks List Export | ✔️ | ❌ |
| GET | /app/data/materials | Material Stock App Data for Mobile only | ❌ | ✔️ |
| GET | /stocks/entities/sort | Stocks By Entity with Sort | ✔️ | ✔️ |

