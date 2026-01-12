# Transaction API Endpoint

> ℹ️ Last updated: 12 Jan 2026

## Table of Contents
- [About](#about)
- [API Endpoint](#api-endpoint)

---

## About

The **Transaction API Endpoints** provide a seamless way to manage financial and inventory-related 
transactions across web and mobile applications. This API enables users to view transaction list, 
create new transactions, and retrieve transaction details, or export transaction list, ensuring accurate 
and efficient transaction processing.

Access to these functionalities is role-based, allowing users to interact with transaction data according 
to their assigned permissions. This ensures secure financial operations, maintains data integrity, 
and supports smooth transaction workflows.

The **Transaction API Endpoints** are essential for optimizing transaction management, improving 
record accuracy, and enhancing overall operational efficiency.

---

## API Endpoint

| **Type** | **API URL** | **API Name** | **Web App** | **Mobile App** |
|----------|-------------|--------------|-------------|----------------|
| GET | /transactions | Transaction Lists | ✔️ | ✔️ |
| GET | /transactions/{id} | Transaction Detail | ✔️ | ✔️ |
| GET | /transactions-discard | Transaction List Discard | ✔️ | ✔️ |
| GET | /transactions/elastic | Transaction Lists Elastic | ✔️ | ✔️ |
| GET | /transactions/xls | Transaction Lists Export | ✔️ | ❌ |
| GET | /transactions/type | Transaction Types | ✔️ | ✔️ |
| GET | /transactions/reason | Transaction Reasons | ✔️ | ✔️ |
| GET | /transactions/consumption | Transaction List Consumption | ✔️ | ✔️ |
| GET | /transactions/rabies-sequence | Transaction Rabies Sequence | ✔️ | ✔️ |
| POST | /transactions/add-stock | Transaction Add Stock | ✔️ | ✔️ |
| POST | /transactions/remove-stock | Transaction Reduce Stock | ✔️ | ✔️ |
| POST | /transactions/discard-stock | Transaction Discard Stock | ✔️ | ✔️ |
| POST | /transactions/consumption | Transaction Consumption | ✔️ | ✔️ |
| POST | /transactions/return-of-health-facitilies | Transaction Return from Health Facilities | ✔️ | ✔️ |
| POST | /transactions/cancelation-discard | Transaction Cancellation of Discard | ✔️ | ✔️ |
| POST | /transactions/consumption | Transaction Consumption (Rabies) | ✔️ | ✔️ |
| POST | /transactions/consumption | Transaction Consumption (Dengue) | ✔️ | ✔️ |
| GET | /transactions/return-of-health-facitilies | Transaction Lists Return of Health Facilities | ✔️ | ✔️ |
| GET | /transactions/transfer-stock | Transaction Relocation Between Program | ✔️ | ✔️ |
| POST | /transfer-stock/stocks | List Stock Material | ✔️ | ✔️ |

