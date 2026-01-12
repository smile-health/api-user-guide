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
| GET | /transactions | Transaction Lists | Yes | Yes |
| GET | /transactions/{id} | Transaction Detail | Yes | Yes |
| GET | /transactions-discard | Transaction List Discard | Yes | Yes |
| GET | /transactions/elastic | Transaction Lists Elastic | Yes | Yes |
| GET | /transactions/xls | Transaction Lists Export | Yes | No |
| GET | /transactions/type | Transaction Types | Yes | Yes |
| GET | /transactions/reason | Transaction Reasons | Yes | Yes |
| GET | /transactions/consumption | Transaction List Consumption | Yes | Yes |
| GET | /transactions/rabies-sequence | Transaction Rabies Sequence | Yes | Yes |
| POST | /transactions/add-stock | Transaction Add Stock | Yes | Yes |
| POST | /transactions/remove-stock | Transaction Reduce Stock | Yes | Yes |
| POST | /transactions/discard-stock | Transaction Discard Stock | Yes | Yes |
| POST | /transactions/consumption | Transaction Consumption | Yes | Yes |
| POST | /transactions/return-of-health-facitilies | Transaction Return from Health Facilities | Yes | Yes |
| POST | /transactions/cancelation-discard | Transaction Cancellation of Discard | Yes | Yes |
| POST | /transactions/consumption | Transaction Consumption (Rabies) | Yes | Yes |
| POST | /transactions/consumption | Transaction Consumption (Dengue) | Yes | Yes |
| GET | /transactions/return-of-health-facitilies | Transaction Lists Return of Health Facilities | Yes | Yes |
| GET | /transactions/transfer-stock | Transaction Relocation Between Program | Yes | Yes |
| POST | /transfer-stock/stocks | List Stock Material | Yes | Yes |

