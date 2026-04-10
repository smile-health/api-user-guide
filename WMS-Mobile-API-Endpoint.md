# Master Data API Endpoints

> ℹ️ Last updated : 10 Apr 2026  

## Table of Contents
- [About](#about)
- [API Endpoints](#api-endpoints)

## About
---

Mobile endpoints are registered under the /api/v1/mobile/ prefix and are optimized for field operations on handheld devices. 
They support QR code scanning, weight entry, follow-up actions, post-treatment workflows, GPS distance validation, and aggregated homepage data.

## API Endpoints
---
| Type | API URL | API Name | Used by Web | Used by Mobile App |
|------|---------|----------|:-----------:|:------------------:|
| POST | `/api/v1/mobile/enter-weight` | Add Waste | ❌ | ✔️ |
| GET | `/api/v1/mobile/homepage` | Get Homepage | ❌ | ✔️ |
| GET | `/api/v1/mobile/homepage/waste-bag-details/{wasteId}` | Get Waste Detail Homepage | ❌ | ✔️ |
| GET | `/api/v1/mobile/scan-qr-code/{id}` | Get Scan QR Code | ❌ | ✔️ |
| GET | `/api/v1/mobile/waste` | Get Waste | ❌ | ✔️ |
| GET | `/api/v1/mobile/waste/detail` | Get Waste Detail | ❌ | ✔️ |
| GET | `/api/v1/mobile/waste/report` | Get Waste Report | ❌ | ✔️ |
| POST | `/api/v1/mobile/waste/follow-up-treatment` | Add Follow Up Treatment | ❌ | ✔️ |
| GET | `/api/v1/mobile/waste/report-waste-status` | Get Report Waste Status | ❌ | ✔️ |
| POST | `/api/v1/mobile/waste/follow-up-action` | Add Follow Up Action | ❌ | ✔️ |
| POST | `/api/v1/mobile/waste/post-treatment` | Add Post Treatment | ❌ | ✔️ |
| POST | `/api/v1/mobile/waste/receiving-treatment-external` | Add Receive Treatment | ❌ | ✔️ |
| PATCH | `/api/v1/mobile/validate/distance-limit` | Update Distance Limit Validation | ❌ | ✔️ |
| GET | `/api/v1/mobile/disposal` | Get Disposal | ❌ | ✔️ |

