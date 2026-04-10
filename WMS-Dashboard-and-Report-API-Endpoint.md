# WMS Dashboard and Report API Endpoints

> ℹ️ Last updated : 10 Apr 2026  

## Table of Contents
- [About](#about)
- [API Endpoints](#api-endpoints)
  - [Report Waste Management APIs](#report-waste-management-apis)
  - [Dashboard APIs](#dashboard-apis)

## About
---
This document provides API endpoints for WMS dashboard and reporting features, including waste hierarchy summaries, activity monitoring, transaction history, waste tracking, logbooks, and exportable reports.

## API Endpoints
---
### Report Waste Management APIs
| Type | API URL | API Name | Used by Web | Used by Mobile App |
|------|---------|----------|:-----------:|:------------------:|
| GET | `/api/v1/waste/transactions` | Get All Waste | ✔️ | ❌ |
| GET | `/api/v1/waste/transactions/export` | Get Waste Export | ✔️ | ❌ |
| GET | `/api/v1/waste/tracking-by-characteristics/export` | Get Export Waste Tracking | ✔️ | ❌ |
| GET | `/api/v1/waste/tracking-by-waste-source` | Get Waste Tracking by Waste Source | ✔️ | ❌ |
| GET | `/api/v1/waste/tracking-by-waste-source/export` | Get Waste Tracking Waste Source Export | ✔️ | ❌ |
| GET | `/api/v1/waste/waste-tracking-all/export` | Get Waste Tracking All | ✔️ | ❌ |
| GET | `/api/v1/waste/logbook` | Get Waste Logbook | ✔️ | ❌ |
| GET | `/api/v1/waste/logbook/export` | Get Waste Logbook Export | ✔️ | ❌ |
| GET | `/api/v1/waste/waste-group/export` | Get Waste Group Export | ✔️ | ❌ |
| GET | `/api/v1/waste/waste-external/export` | Get Waste External Export | ✔️ | ❌ |
| GET | `/api/v1/waste/transaction-history` | Get Transaction History | ✔️ | ❌ |
| GET | `/api/v1/waste/waste-group-details/{wasteGroupId}` | Get Waste Group Details | ✔️ | ❌ |
| GET | `/api/v1/waste/waste-bag-internal-treatment-details/{wasteBagQrCodeId}` | Get Waste Bag Internal Treatment Details | ✔️ | ❌ |

### Dashboard APIs
| Type | API URL | API Name | Used by Web | Used by Mobile App |
|------|---------|----------|:-----------:|:------------------:|
| GET | `/api/v1/dashboard/cities/{cityId}/waste-hierarchy-summary` | Get Dashboard Waste Hierarchy Summary by City | ✔️ | ❌ |
| GET | `/api/v1/dashboard/provinces/{provinceId}/waste-hierarchy-summary` | Get Dashboard Waste Hierarchy Summary by Province | ✔️ | ❌ |
| GET | `/api/v1/dashboard/waste-hierarchy-summary` | Get Dashboard Waste Hierarchy Summary | ✔️ | ❌ |
| GET | `/api/v1/dashboard/waste-groups/admin-healthcare-facilities` | Get Dashboard Waste Group Admin HF | ✔️ | ❌ |
| GET | `/api/v1/dashboard/waste-groups/transporter` | Get Dashboard Waste Group Transporter | ✔️ | ❌ |
| GET | `/api/v1/dashboard/waste-groups/treatment` | Get Dashboard Waste Groups Treatment | ✔️ | ❌ |
| GET | `/api/v1/dashboard/waste-group-details/{id}` | Get Dashboard Waste Group Details | ✔️ | ❌ |
| GET | `/api/v1/dashboard/summary-activity-entities` | Get Dashboard Summary Activity Entities | ✔️ | ❌ |
| GET | `/api/v1/dashboard/summary-activity-entities/export` | Get Dashboard Summary Activity Entities Export | ✔️ | ❌ |
| GET | `/api/v1/dashboard/manual-scale-activity-entities` | Get Dashboard Manual Scale Activity | ✔️ | ❌ |
| GET | `/api/v1/dashboard/summary-users-activity` | Get Dashboard Summary Users Activity | ✔️ | ❌ |
