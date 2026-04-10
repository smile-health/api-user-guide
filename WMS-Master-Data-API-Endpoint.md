# Master Data API Endpoints

> ℹ️ Last updated : 10 Apr 2026  

## Table of Contents
- [About](#about)
- [API Endpoints](#api-endpoints)
  - [Master Data APIs](#master-data-apis)
  - [Asset Management APIs](#asset-management-apis)
  - [Partnership Management Data APIs](#parnership-management-data-apis)

## About
---

The document outlines various API endpoints related to user management. It includes methods for retrieving a list of users, creating new users, updating user information, and deleting users. Additionally, it provides endpoints for accessing user change logs, updating user status, and importing or exporting user data using Excel templates. Each endpoint is associated with a specific HTTP method and a brief description of its functionality.

## API Endpoints
---
### Master Data APIs
| Type | API URL | API Name | Used by Web | Used by Mobile App |
|------|---------|----------|:-----------:|:------------------:|
| GET | `/api/v1/entities/all` | Get Entity | ✔️ | ❌ |
| GET | `/api/v1/entities` | Get by entity detail | ✔️ | ✔️ |
| PUT | `/api/v1/entities/{id}` | Update status entities | ✔️ | ❌ |
| PATCH | `/api/v1/entities` | Update entities | ✔️ | ❌ |
| GET | `/api/v1/users` | Get Users | ✔️ | ❌ |
| PUT | `/api/v1/users/{id}` | Update users | ✔️ | ❌ |
| GET | `/api/v1/entity-settings` | Get Entity Setting | ✔️ | ❌ |
| POST | `/api/v1/entity-settings` | Add Entity Settings | ✔️ | ❌ |
| GET | `/api/v1/entity-settings/{id}` | Get Detail Entity Setting | ✔️ | ❌ |
| PUT | `/api/v1/entity-settings/{id}` | Update Entity Setting | ✔️ | ❌ |
| DELETE | `/api/v1/entity-settings/{id}` | Delete Entity Setting | ✔️ | ❌ |
| GET | `/api/v1/global-settings` | Get List Global Setting | ✔️ | ❌ |
| POST | `/api/v1/global-settings` | Add Global Setting | ✔️ | ❌ |
| PUT | `/api/v1/global-settings/{id}` | Update Global Setting | ✔️ | ❌ |
| DELETE | `/api/v1/global-settings/{id}` | Delete Global Setting | ✔️ | ❌ |
| GET | `/api/v1/healthcare-facility-settings` | Get List Healthcare Facility Setting | ✔️ | ❌ |
| POST | `/api/v1/healthcare-facility-settings` | Add Healthcare Facility Setting | ✔️ | ❌ |
| GET | `/api/v1/healthcare-facility-settings/{id}` | Get Detail Healthcare Facility Setting | ✔️ | ❌ |
| PUT | `/api/v1/healthcare-facility-settings/{id}` | Update Healthcare Facility Setting | ✔️ | ❌ |
| DELETE | `/api/v1/healthcare-facility-settings/{id}` | Delete Healthcare Facility Setting | ✔️ | ❌ |
| GET | `/api/v1/entity-location` | Get Entity Location | ✔️ | ❌ |
| POST | `/api/v1/entity-location` | Add Entity Location | ✔️ | ❌ |
| GET | `/api/v1/entity-location/{id}` | Get Detail Entity Location | ✔️ | ❌ |
| PUT | `/api/v1/entity-location/{id}` | Update Entity Location | ✔️ | ❌ |
| DELETE | `/api/v1/entity-location/{id}` | Delete Entity Location | ✔️ | ❌ |
| GET | `/api/v1/qr-code-config` | Get List QR Code Config | ✔️ | ❌ |
| POST | `/api/v1/qr-code-config` | Add QR Code Config | ✔️ | ❌ |
| GET | `/api/v1/qr-code-config/{id}` | Get Detail QR Code Config | ✔️ | ❌ |
| PUT | `/api/v1/qr-code-config/{id}` | Update QR Code Config | ✔️ | ❌ |
| DELETE | `/api/v1/qr-code-config/{id}` | Delete QR Code Config | ✔️ | ❌ |
| POST | `/api/v1/waste-hierarchy` | Add Waste Type | ✔️ | ❌ |
| POST | `/api/v1/waste-hierarchy` | Add Waste Group | ✔️ | ❌ |
| POST | `/api/v1/waste-hierarchy` | Add Waste Characteristic | ✔️ | ❌ |
| GET | `/api/v1/waste-hierarchy` | Get All Waste Type | ✔️ | ❌ |
| GET | `/api/v1/waste-hierarchy` | Get All Waste Group | ✔️ | ❌ |
| GET | `/api/v1/waste-hierarchy` | Get All Waste Characteristic | ✔️ | ❌ |
| GET | `/api/v1/waste-hierarchy/{id}` | Get Detail Waste Characteristic | ✔️ | ❌ |
| PUT | `/api/v1/waste-hierarchy/{id}` | Update Waste Hierarchy | ✔️ | ❌ |
| DELETE | `/api/v1/waste-hierarchy/{id}` | Delete Waste Hierarchy | ✔️ | ❌ |
| GET | `/api/v1/waste-hierarchy/explanation-waste-classification` | Get All Waste Hierarchy | ✔️ | ❌ |
| GET | `/api/v1/waste-hierarchy/parent-hierarchy` | Get Parent Waste Hierarchy | ✔️ | ❌ |
| GET | `/api/v1/waste-classification` | Get Waste Classification | ✔️ | ❌ |
| POST | `/api/v1/waste-classification` | Add Waste Classification | ✔️ | ❌ |
| GET | `/api/v1/waste-classification/{id}` | Get Detail Waste Classification | ✔️ | ❌ |
| PUT | `/api/v1/waste-classification/{id}` | Update Waste Classification | ✔️ | ❌ |
| DELETE | `/api/v1/waste-classification/{id}` | Delete Waste Classification | ✔️ | ❌ |
| GET | `/api/v1/waste-source` | Get Waste Source | ✔️ | ❌ |
| POST | `/api/v1/waste-source` | Add Waste Source | ✔️ | ❌ |
| GET | `/api/v1/waste-source/{id}` | Get Detail Waste Source | ✔️ | ❌ |
| PUT | `/api/v1/waste-source/{id}` | Update Waste Source | ✔️ | ❌ |
| DELETE | `/api/v1/waste-source/{id}` | Delete Waste Source | ✔️ | ❌ |

### Asset Management Data APIs
| Type | API URL | API Name | Used by Web | Used by Mobile App |
|------|---------|----------|:-----------:|:------------------:|
| GET | `/api/v1/asset` | Get Asset | ✔️ | ❌ |
| POST | `/api/v1/asset` | Add Asset | ✔️ | ❌ |
| GET | `/api/v1/asset/{id}` | Get Detail Asset | ✔️ | ❌ |
| PUT | `/api/v1/asset/{id}` | Update Asset | ✔️ | ❌ |
| DELETE | `/api/v1/asset/{id}` | Delete Asset | ✔️ | ❌ |
| GET | `/api/v1/asset-model` | Get Asset Model | ✔️ | ❌ |
| POST | `/api/v1/asset-model` | Add Asset Model | ✔️ | ❌ |
| GET | `/api/v1/asset-model/{id}` | Get Detail Asset Model | ✔️ | ❌ |
| PUT | `/api/v1/asset-model/{id}` | Update Asset Model | ✔️ | ❌ |
| DELETE | `/api/v1/asset-model/{id}` | Delete Asset Model | ✔️ | ❌ |
| GET | `/api/v1/healthcare-facility-asset` | Get List Healthcare Facility Asset | ✔️ | ❌ |
| GET | `/api/v1/healthcare-facility-asset/entity` | Get List Healthcare Facility Asset by Entity | ✔️ | ❌ |
| POST | `/api/v1/healthcare-facility-asset` | Add Healthcare Facility Asset | ✔️ | ❌ |
| GET | `/api/v1/healthcare-facility-asset/{id}` | Get Detail Healthcare Facility Asset | ✔️ | ❌ |
| PUT | `/api/v1/healthcare-facility-asset/{id}` | Update Healthcare Facility Asset | ✔️ | ❌ |
| PATCH | `/api/v1/healthcare-facility-asset/{id}` | Partial Update Healthcare Facility Asset | ✔️ | ❌ |
| DELETE | `/api/v1/healthcare-facility-asset/{id}` | Delete Healthcare Facility Asset | ✔️ | ❌ |
| GET | `/api/v1/asset-dongle/{id}` | Get Detail Asset Dongle | ✔️ | ❌ |
| POST | `/api/v1/asset-dongle` | Add Asset Dongle | ✔️ | ❌ |
| PUT | `/api/v1/asset-dongle` | Update Asset Dongle | ✔️ | ❌ |

### Partnership Management Data APIs
| Type | API URL | API Name | Used by Web | Used by Mobile App |
|------|---------|----------|:-----------:|:------------------:|
| GET | `/api/v1/partnership` | Get All Partnership | ✔️ | ❌ |
| GET | `/api/v1/partnership/multiple-transporter` | Get Partnership Multiple Transporter | ✔️ | ❌ |
| GET | `/api/v1/partnership/third-parties` | Get Partnership Third Party | ✔️ | ❌ |
| GET | `/api/v1/partnership/healthcare-thirdparty` | Get Partnership by Healthcare | ✔️ | ❌ |
| GET | `/api/v1/partnership/thirdparty` | Get Partnership by Third Party | ✔️ | ❌ |
| GET | `/api/v1/partnership/waste-classification` | Get Partnership Waste Classification | ✔️ | ❌ |
| GET | `/api/v1/partnership/waste-classification-consumer-thirdparty` | Get Waste Classification by Healthcare and Third Party | ✔️ | ❌ |
| POST | `/api/v1/partnership` | Add Partnership | ✔️ | ❌ |
| GET | `/api/v1/partnership/{id}` | Get Detail Partnership | ✔️ | ❌ |
| PUT | `/api/v1/partnership/{id}` | Update Partnership | ✔️ | ❌ |
| DELETE | `/api/v1/partnership/{id}` | Delete Partnership | ✔️ | ❌ |
| GET | `/api/v1/partner-vehicle` | Get Partner Vehicle | ✔️ | ❌ |
| POST | `/api/v1/partner-vehicle` | Add Partner Vehicle | ✔️ | ❌ |
| POST | `/api/v1/partner-vehicle/bulk-healthcare` | Add Bulk Partner Vehicle | ✔️ | ❌ |
| GET | `/api/v1/partner-vehicle/{id}` | Get Detail Partner Vehicle | ✔️ | ❌ |
| PUT | `/api/v1/partner-vehicle/{id}` | Update Partner Vehicle | ✔️ | ❌ |
| DELETE | `/api/v1/partner-vehicle/{id}` | Delete Partner Vehicle | ✔️ | ❌ |
| GET | `/api/v1/partner-vehicle/export` | Export Partner Vehicle | ✔️ | ❌ |
| GET | `/api/v1/partnership-operator-map` | Get List Partnership Operator | ✔️ | ❌ |
| POST | `/api/v1/partnership-operator-map` | Add Partnership Operator | ✔️ | ❌ |
| GET | `/api/v1/partnership-operator-map/operator-from-operatormap` | Get Partnership Operator from Operator Map | ✔️ | ❌ |
| GET | `/api/v1/partnership-operator-map/operator-thirdparty` | Get Partnership Operator Third Party | ✔️ | ❌ |
| PUT | `/api/v1/partnership-operator-map` | Update Partnership Operator | ✔️ | ❌ |
| DELETE | `/api/v1/partnership-operator-map` | Delete Partnership Operator | ✔️ | ❌ |

