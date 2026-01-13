# Master Data API Endpoints

> ℹ️ Last updated : 13 Jan 2026  

## Table of Contents
- [About](#about)
- [API Endpoints](#api-endpoints)
  - [Global Setting APIs](#global-setting-apis)
  - [Program Setting APIs](#program-setting-apis)

## About
---

The document outlines various API endpoints related to user management. It includes methods for retrieving a list of users, creating new users, updating user information, and deleting users. Additionally, it provides endpoints for accessing user change logs, updating user status, and importing or exporting user data using Excel templates. Each endpoint is associated with a specific HTTP method and a brief description of its functionality.

> ℹ️ Master Data is the core foundation of SMILE repositories and data structures. Because of this, some APIs in the Master Data service may also be utilised as supporting APIs in other services.

## API Endpoints
---
### Global Setting APIs

| Type | API URL | API Name | Used by Web | Used by Mobile App |
|------|---------|----------|:-----------:|:------------------:|
| GET  | /programs     | Program List         | ✔️ | ❌ |
| GET  | /program/xls  | Export Program List | ✔️ | ❌ |
| GET | `/programs/{id}` | Program Detail | ✔️ | ❌ |
| POST | `/programs` | Create Program | ✔️ | ❌ |
| PUT | `/programs/{id}` | Edit Program | ✔️ | ❌ |
| GET | `/programs/{program_id}/activities` | Activity List | ✔️ | ❌ |
| GET | `/programs/{program_id}/activities/xls` | Export Activity | ✔️ | ❌ |
| GET | `/programs/{program_id}/activities/{activity_id}` | Activity Detail | ✔️ | ❌ |
| POST | `/programs/{program_id}/activities` | Create Activity | ✔️ | ❌ |
| PUT | `/programs/{program_id}/activities` | Edit Activity | ✔️ | ❌ |
| PUT | `/programs/{program_id}/activities/{activity_id}/status` | Update Activity Status | ✔️ | ❌ |
| GET | `/users` | Get User List | ✔️ | ❌ |
| GET | `/users/xls` | Export User List | ✔️ | ❌ |
| GET | `/users/xls-template` | Download Template User | ✔️ | ❌ |
| POST | `/users/xls` | Import User Data | ✔️ | ❌ |
| GET | `/users/{id}` | Get User Detail | ✔️ | ❌ |
| POST | `/users` | Create User | ✔️ | ❌ |
| PUT | `/users/{id}` | Edit User | ✔️ | ❌ |
| PUT | `/users/{id}/status` | Update Status User | ✔️ | ❌ |
| GET | `/users/{id}/chg_history` | Get User Changelogs | ✔️ | ❌ |
| GET | `/entities` | Get List Entity | ✔️ | ❌ |
| GET | `/entities/xls` | Export Entity | ✔️ | ❌ |
| GET | `/entities/xls-template` | Download Entity Template | ✔️ | ❌ |
| POST | `/entities/xls` | Import Entity | ✔️ | ❌ |
| GET | `/entities/{entity_id}` | Get Detail Entity | ✔️ | ❌ |
| POST | `/entities` | Add Entity | ✔️ | ❌ |
| PUT | `/entities/{entity_id}` | Edit Entity | ✔️ | ❌ |
| GET | `/entity-tags` | Get List Tags Entity | ✔️ | ❌ |
| GET | `/entity-types` | Get List Type Entity | ✔️ | ❌ |
| GET | `/provinces` | Get List Province | ✔️ | ❌ |
| GET | `/regencies` | Get List Regency | ✔️ | ❌ |
| GET | `/subdistricts` | Get List Sub District | ✔️ | ❌ |
| GET | `/villages` | Get List Villages | ✔️ | ❌ |
| GET | `/materials` | Global Lists Material Non-Hirarki / Product Template / Product Variant | ✔️ | ❌ |
| GET | `/materials/xls` | Export List | ✔️ | ❌ |
| GET | `/materials/xls-template` | Download Template (Non Hierarchy / Product Template / Product Variant) | ✔️ | ❌ |
| POST | `/materials/xls` | Import Material | ✔️ | ❌ |
| GET | `/materials/{id}` | Global Detail Material (Non-Hirarki / Product Template / Product Variant) | ✔️ | ❌ |
| POST | `/materials` | Create Material (Non-Hirarki / Product Template / Product Variant) | ✔️ | ❌ |
| PUT | `/materials/{id}` | Edit Material Global | ✔️ | ❌ |
| PUT | `/materials/{id}/status` | Update Material Status | ✔️ | ❌ |
| GET | `/material-levels` | Material Level | ✔️ | ❌ |
| GET | `/material-units` | Material Unit | ✔️ | ❌ |
| GET | `/material-types` | Material Type | ✔️ | ❌ |
| GET | `/manufactures` | List Manufacturer | ✔️ | ❌ |
| GET | `/manufactures/xls` | Export Manufacturer | ✔️ | ❌ |
| GET | `/manufactures/xls-template` | Template Manufacturer | ✔️ | ❌ |
| POST | `/manufactures/xls` | Import Manufacturer | ✔️ | ❌ |
| GET | `/manufactures/{id}` | Detail Manufacturer | ✔️ | ❌ |
| POST | `/manufactures` | Create Manufacturer | ✔️ | ❌ |
| PUT | `/manufactures/{id}` | Update Manufacturer | ✔️ | ❌ |
| GET | `/manufactures/type` | List Manufacturer Type | ✔️ | ❌ |
| GET | `/budget-sources` | Get Budget Source List | ✔️ | ❌ |
| GET | `/budget-sources/xls` | Export Budget Source Excel | ✔️ | ❌ |
| GET | `/budget-sources/{id}` | Get Budget Source Detail | ✔️ | ❌ |
| POST | `/budget-sources` | Create Budget Source | ✔️ | ❌ |
| PUT | `/budget-sources/{id}` | Update Budget Source | ✔️ | ❌ |
| GET | `/asset-types` | Get List Asset Type | ✔️ | ❌ |
| GET | `/asset-types/xls` | Export | ✔️ | ❌ |
| GET | `/asset-types/{id}` | Get Asset Type Detail | ✔️ | ❌ |
| GET | `/asset-types/xls-template` | Download Template | ✔️ | ❌ |
| POST | `/asset-types` | Create Asset Type | ✔️ | ❌ |
| POST | `/asset-types/xls` | Import Asset Type | ✔️ | ❌ |
| PUT | `/asset-types/{id}` | Update Asset Type | ✔️ | ❌ |
| GET | `/asset-models` | Get List Asset Models | ✔️ | ❌ |
| GET | `/asset-models/xls` | Export List Asset Model | ✔️ | ❌ |
| GET | `/asset-models/{id}` | Get Asset Model Detail | ✔️ | ❌ |
| GET | `/asset-models/xls-template` | Download Template | ✔️ | ❌ |
| POST | `/asset-models` | Create Asset Model | ✔️ | ❌ |
| POST | `/asset-models/xls` | Import Asset Model | ✔️ | ❌ |
| PUT | `/asset-models/{id}` | Update Asset Model | ✔️ | ❌ |
| GET | `/asset-vendors` | Get List Asset Vendor | ✔️ | ❌ |
| GET | `/asset-vendors/xls` | Export List Asset Vendor | ✔️ | ❌ |
| GET | `/asset-vendors/{id}` | Get Asset Vendor Detail | ✔️ | ❌ |
| GET | `/asset-vendors/xls-template` | Download Template | ✔️ | ❌ |
| POST | `/asset-vendors` | Create Asset Vendor | ✔️ | ❌ |
| POST | `/asset-vendors/xls` | Import Asset Vendor | ✔️ | ❌ |
| PUT | `/asset-vendors/{id}` | Update Asset Vendor | ✔️ | ❌ |
| GET | `/app/notif` | In App Notification | ❌ | ✔️ |
| GET | `/app/data/{id}/cva` | App Data: Customer - Vendor - Activities | ❌ | ✔️ |
| GET | `/app/data/trx-types` | App Data: Transaction Types | ❌ | ✔️ |
| GET | `/app/data/{id}/materials` | App Data: Materials | ❌ | ✔️ |

### Program Setting APIs

| Type | API URL | API Name | Used by Web | Used by Mobile App |
|------|---------|----------|:-----------:|:------------------:|
| GET | `/account/workspaces` | Get Workspaces | ✔️ | ✔️ |
| GET | `/users` | Get By Workspace | ✔️ | ❌ |
| GET | `/users/{id}` | Get Detail By Workspace | ✔️ | ❌ |
| PUT | `/users/{id}/status` | Update Status | ✔️ | ❌ |
| GET | `/activities` | Get List | ✔️ | ❌ |
| GET | `/activities/xls` | Export | ✔️ | ❌ |
| GET | `/activities/xls-template` | Template | ✔️ | ❌ |
| POST | `/activities/xls` | Import | ✔️ | ❌ |
| GET | `/activities/{id}` | Get Detail | ✔️ | ❌ |
| POST | `/activities` | Create | ✔️ | ❌ |
| PUT | `/activities/{id}` | Update | ✔️ | ❌ |
| GET | `/entities` | Get List Entity | ✔️ | ❌ |
| GET | `/entities/xls` | Export Excel List All Entity | ✔️ | ❌ |
| GET | `/entities/xls-template` | Download Template Entity | ✔️ | ❌ |
| POST | `/entities/xls` | Import Entity Data | ✔️ | ❌ |
| GET | `/entities/{id}` | Get Detail Entity | ✔️ | ❌ |
| PUT | `/entities/{id}/status` | Update Status Active Entity | ✔️ | ❌ |
| PUT | `/entities/{id}/status/vendors` | Update Status Vendor Entity | ✔️ | ❌ |
| GET | `/entities/{id}/customers/xls-template` | Export Template Excel List Customer | ✔️ | ❌ |
| POST | `/entities/{id}/customers/xls` | Import Excel Customer Entity | ✔️ | ❌ |
| GET | `/entities/{id}/customers` | Get List Customer Entity | ✔️ | ❌ |
| GET | `/entities/{id}/customers/xls` | Export Excel List Distribution or Consumption Customer | ✔️ | ❌ |
| POST | `/entities/customers` | Create Customer | ✔️ | ❌ |
| PUT | `/entities/customers` | Update Customer | ✔️ | ❌ |
| DELETE | `/entities/customers` | Delete Customer | ✔️ | ❌ |
| GET | `/entities/{id}/vendors` | Get List Vendor Entity | ✔️ | ❌ |
| GET | `/entities/{id}/activities` | Get List Activity Entity | ✔️ | ❌ |
| POST | `/entities/activities/submit-time` | Insert and Update Implementation Activity | ✔️ | ❌ |
| GET | `/entity-tags` | Get List Tags Entity | ✔️ | ❌ |
| GET | `/entity-types` | Get List Type Entity | ✔️ | ❌ |
| GET | `/provinces` | Get List Province | ✔️ | ❌ |
| GET | `/regencies` | Get List Regency | ✔️ | ❌ |
| GET | `/subdistricts` | Get List Subdistricts | ✔️ | ❌ |
| GET | `/entities/{id}/users` | Get List User Entity | ✔️ | ❌ |
| GET | `/entities/{id}/customers/list-relation-customers` | Get List Relation Customer Entity | ✔️ | ❌ |
| GET | `/entities/{entity_id}/materials` | List Material Entities | ✔️ | ❌ |
| POST | `/entities/{entity_id}/materials` | Create Material Entities Relationship | ✔️ | ❌ |
| PUT | `/entities/{entity_id}/materials` | Update Material Entities Relationship | ✔️ | ❌ |
| DELETE | `/entities/{entity_id}/materials/{entity_master_material_activities_id}` | Material Entities | ✔️ | ❌ |
| POST | `/entities/{entity_id}/materials/bulk` | Create Material Entities Relationship Bulk | ✔️ | ❌ |
| PUT | `/entities/{entity_id}/materials/{entity_master_material_id}/bulk` | Update Material Entities Relationship Bulk | ✔️ | ❌ |
| GET | `/entities-materials-bulk` | Log List Entities Materials Bulk | ✔️ | ❌ |
| POST | `/entities-materials-bulk/xls` | Import Material Entities Bulk | ✔️ | ❌ |
| GET | `/entities-materials-bulk/template` | Filter Template Material Entities | ✔️ | ❌ |
| GET | `/materials` | Lists (Non Hierarchy / Product Template / Product Variant) | ✔️ | ❌ |
| GET | `/materials/xls` | Export (Non-Hirarki / Product Template / Product Variant) | ✔️ | ❌ |
| POST | `/materials/xls` | Import Update (Non-Hirarki / Product Variant) | ✔️ | ❌ |
| GET | `/materials/{id}` | Material Details (Non Hierarchy / Product Template / Product Variant) | ✔️ | ❌ |
| PUT | `/materials/{id}` | Update (Non-Hierarchy / Product Template / Product Variant) | ✔️ | ❌ |
| GET | `/manufactures` | Get List by Program | ✔️ | ❌ |
| GET | `/manufactures/{id}` | Get Detail By Program | ✔️ | ❌ |
| PUT | `/manufactures/{id}` | Update Status | ✔️ | ❌ |
| GET | `/budget-sources` | Get By Workspace | ✔️ | ❌ |
| GET | `/budget-sources/{id}` | Get Detail By Workspace | ✔️ | ❌ |
| GET | `/budget-sources/xls` | Export Excel | ✔️ | ❌ |
| GET | `/app/notif` | In App Notification | ❌ | ✔️ |
| GET | `/app/data/{id}/cva` | App Data: Customer - Vendor - Activities | ❌ | ✔️ |
| GET | `/app/data/trx-types` | App Data: Transaction Types | ❌ | ✔️ |
| GET | `/protocols` | 	Get List Protocols | ✔️ | ❌ |
| GET | `/protocols/{protocol_id}/material-activities` | Get List Material Activities Protocol | ✔️ | ❌ |
| POST | `/protocols/material-activities` | Set Protocol to Material Activities | ✔️ | ❌ |
| PUT | `/protocols/{protocolId}/status` | Update Protocol Status | ✔️ | ❌ |
| DELETE | `/protocols/{protocolId}/material-activities/{id}` | Delete Material Activities | ✔️ | ❌ |


