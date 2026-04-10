# WMS Transaction API Endpoint

> ℹ️ Last updated: 10 Apr 2026

## Table of Contents
- [About](#about)
- [API Endpoint](#api-endpoint)
  - [Waste Management APIs](#waste-management-apis)
---

## About

The waste management domain encompasses the complete lifecycle of healthcare waste – from initial bag creation and weighing, 
through intermediate storage and treatment, to transportation handover and external disposal. 
This is the largest domain in the BADR WMS API, comprising over 30 endpoints.

---

## API Endpoint

### Waste Management APIs
| Type | API URL | API Name | Used by Web | Used by Mobile App |
|------|---------|----------|:-----------:|:------------------:|
| GET | `/api/v1/waste` | Get All Waste | ✔️ | ❌ |
| POST | `/api/v1/waste` | Add Waste | ✔️ | ❌ |
| PATCH | `/api/v1/waste/temporary-store` | Update Waste Temporary Store | ✔️ | ❌ |
| PATCH | `/api/v1/waste/cold-store` | Update Waste Cold Store | ✔️ | ❌ |
| PATCH | `/api/v1/waste/internal_landfill` | Update Waste Internal Landfill | ✔️ | ❌ |
| PATCH | `/api/v1/waste/autoclave` | Update Waste Autoclave | ✔️ | ❌ |
| PATCH | `/api/v1/waste/incinerate` | Update Waste Incinerate | ✔️ | ❌ |
| PATCH | `/api/v1/waste/sterilise` | Update Sterilise | ✔️ | ❌ |
| POST | `/api/v1/waste/follow-up-treatment` | Add Follow Up Treatment | ✔️ | ❌ |
| PATCH | `/api/v1/waste/follow-up/transport-request` | Update Follow Up Transport Request | ✔️ | ❌ |
| POST | `/api/v1/waste/handover/transport-request` | Update Handover Transport Request | ✔️ | ❌ |
| PATCH | `/api/v1/waste/follow-up/transport-external-request` | Update Transporter External | ✔️ | ❌ |
| POST | `/api/v1/waste/handover/transport-external-request` | Add Handover Transport External Request | ✔️ | ❌ |
| POST | `/api/v1/waste/pick-up/transport-external-request` | Add Waste Pick Up Transporter External | ✔️ | ❌ |
| POST | `/api/v1/waste/handover/treatment-external-request` | Add Handover Treatment External Request | ✔️ | ❌ |
| POST | `/api/v1/waste/receiving/treatment-external-request` | Add Receiving Treatment External Request | ✔️ | ❌ |
| GET | `/api/v1/waste-transport-external-group` | Get Waste Transport External | ✔️ | ✔️ |
| GET | `/api/v1/waste-transport-external-group/detail` | Get Detail Waste Transport External | ✔️ | ✔️ |
| GET | `/api/v1/waste-treatment-external-group` | Get Waste Treatment External | ✔️ | ✔️ |
| GET | `/api/v1/waste-treatment-external-group/detail` | Get Detail Waste Treatment External | ✔️ | ✔️ |
| GET | `/api/v1/bast` | Get BAST | ✔️ | ❌ |
| GET | `/api/v1/bast/{bast_no}` | Get Detail BAST | ✔️ | ❌ |
| PUT | `/api/v1/bast/confirm` | Confirm BAST | ✔️ | ❌ |
| GET | `/api/v1/manual-scale` | Get Manual Scale | ✔️ | ❌ |
| POST | `/api/v1/manual-scale` | Add Manual Scale | ✔️ | ❌ |
| PATCH | `/api/v1/manual-scale/active` | Update Status Manual Scale | ✔️ | ❌ |
