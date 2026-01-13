# Master Data Role Matrix

> ℹ️ Last updated : 13 Jan 2026  

## Table of Contents
- [About](#about)
- [Roles Matrix](#roles-matrix)


## About
---
The Role Matrix delineates the various functionalities and permissions assigned to different user roles within the Master Data service, specifically for Super Admin and Admin. It distinguishes between full access and view-only capabilities, providing a clear reference for understanding user responsibilities in managing master data. 

The matrix includes various settings, such as user management, entity management, and material data, detailing the specific actions each role can perform. This structured approach ensures clarity in access levels and enhances the management of master data across the system.

## Role Matrix
---
| Functionalities                          | Features                                      | Super Admin Full | Super Admin View-only | Admin Full | Admin View-only |
|-------------------------------------------|-----------------------------------------------|:-------:|:------------:|:----------:|:---------------:|
| Global Setting - Program Management       | View Program List                            | ✔| ✔ | ❌ | ❌ |
| Global Setting - Program Management       | Export Program List                          | ✔ | ✔ | ❌ | ❌ |
| Global Setting - Program Management       | View Detail Program                          | ✔ | ✔ | ❌ | ❌ |
| Global Setting - Program Management       | Create Program                               | ✔ | ❌ | ❌ | ❌ |
| Global Setting - Program Management       | Edit Program                                 | ✔ | ❌ | ❌ | ❌ |
| Global Setting - Program Management       | View List of Activity in Program Detail      | ✔ | ✔ | ❌ | ❌ |
| Global Setting - Program Management       | Create Activity in Program Detail            | ✔ | ❌ | ❌ | ❌ |
| Global Setting - Program Management       | Edit Activity in Program Detail              | ✔ | ❌ | ❌ | ❌ |
| Global Setting - Program Management | Update Activity Status in Program Detail | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - User Management | View User List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - User Management | Export User List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - User Management | Download Template User | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - User Management | Import User Data List | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - User Management | View Detail User Data | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - User Management | Create User | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - User Management | Edit User | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Entity Management | View Entity List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Entity Management | Export Entity Data List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Entity Management | Download Template for Import Entity Data | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Entity Management | Import Entity Data | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Entity Management | View Detail Entity | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Entity Management | View List User on an Entity Global | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Entity Management | Create Entity | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Entity Management | Edit Entity | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Material Data | View Material Data List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Material Data | Export Material Data List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Material Data | Download Template for Import Material Data | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Material Data | Import Material Data | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Material Data | View Detail Material Data | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Material Data | Create Material Data | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Material Data | Edit Material Data | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Material Data | View Detail Material Data Non Hierarchy | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Material Data | Export Material Data List Non Hierarchy | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Material Data | Import Material Data Non Hierarchy | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Material Data | Create Material Non Hierarchy | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Material Data | Edit Material Data Non Hierarchy | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Material Data | Update Status Material Non Hierarchy | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Manufacturer | View Manufacturer List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Manufacturer | Export Manufacturer List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Manufacturer | Download Template for Import Manufacturer Data | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Manufacturer | Import Manufacturer Data List | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Manufacturer | View Detail Manufacturer | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Manufacturer | Create Manufacturer | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Manufacturer | Edit Manufacturer | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Budget Source | View Budget Source List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Budget Source | Export Budget Source List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Budget Source | View Detail Budget Source | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Budget Source | Create Budget Source | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Budget Source | Edit Budget Source | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Asset Type | View Asset Type List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Asset Type | Export Asset Type List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Asset Type | Download Template for Import Asset Type Data | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Asset Type | Import Asset Type Data List | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Asset Type | View Detail Asset Type | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Asset Type | Create Asset Type | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Asset Type | Edit Asset Type | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Asset Model | View Asset Model List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Asset Model | Export Asset Model List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Asset Model | Download Template for Import Asset Model Data | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Asset Model | Import Asset Model Data List | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Asset Model | View Detail Asset Model | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Asset Model | Create Asset Model | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Asset Model | Edit Asset Model | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Asset Vendor | View Asset Vendor List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Asset Vendor | Export Asset Vendor List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Asset Vendor | Download Template for Import Asset Vendor Data | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Asset Vendor | Import Asset Vendor Data List | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Asset Vendor | View Detail Asset Vendor | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - Asset Vendor | Create Asset Vendor | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - Asset Vendor | Edit Asset Vendor | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - PQS Code | View Asset PQS Code List | ✔️ | ✔️ | ❌ | ❌ |
| Global Setting - PQS Code | Export Asset PQS List | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - PQS Code | View Detail Asset PQS Code | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - PQS Code | Create Asset PQS Code | ✔️ | ❌ | ❌ | ❌ |
| Global Setting - PQS Code | Edit Asset Vendor | ✔️ | ❌ | ❌ | ❌ |
| Global Settings - Patient | View Patient List | ✔️ | ❌ | ❌ | ❌ |
| Global Settings - Patient | Download Template for Import Patient Data | ✔️ | ❌ | ❌ | ❌ |
| Global Settings - Patient | Import Patient Data List | ✔️ | ❌ | ❌ | ❌ |
| Global Settings - Target Group | View Target Group List | ✔️ | ❌ | ❌ | ❌ |
| Global Settings - Target Group | Import Target Group List | ✔️ | ❌ | ❌ | ❌ |
| Global Settings - Target Group | Export Target Group List | ✔️ | ❌ | ❌ | ❌ |
| Global Settings - Target Group | Download Template for Import Target Group Data | ✔️ | ❌ | ❌ | ❌ |
| Global Settings - Target Group | Edit Target Group | ✔️ | ❌ | ❌ | ❌ |
| Global Settings - Target Group | Deactivate Target Group | ✔️ | ❌ | ❌ | ❌ |
| Program Setting - User Management | View User List | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - User Management | View Detail User | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - User Management | Update User Status | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Activity Management | View Activity List | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Activity Management | Export Activity List | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Activity Management | View Detail Activity | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Activity Management | Create Activity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Activity Management | Edit Activity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Activity Management | Update Activity Status | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | View Entity List | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Entity Management | Export Entity Data List | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Entity Management | View Detail Entity | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Entity Management | Edit Entity's Active Transaction Status | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | Edit Entity’s Relocation Access Status | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | View List User on an Entity | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Entity Management | Update Entity Status | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | View Activity Implementation Time on Entity | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Entity Management | Edit Activity Implementation Time on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | Add New Period of Activity Implementation Time on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | Download Template for Import Customer & Vendor Relation on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | Import Customer & Vendor Relation on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | View List Distribution Customer on Entity | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Entity Management | Export Distribution Customer on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | Add Distribution Customer on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | Edit Activity of Distribution Customer on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | Delete Distribution Customer on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | View List Consumption Customer on Entity | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Entity Management | Export Consumption Customer on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | Add Consumption Customer on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | Edit Activity of Consumption Customer on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | Delete Consumption Customer on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | View List Vendor on Entity | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Entity Management | View Material-Entity Relation | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Entity Management | View Detail Material-Entity Relation | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Entity Management | Add Material-Entity Relation | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | Edit Material-Entity Relation | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Entity Management | Delete Material-Entity Relation | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Budget Source | View Budget Source List | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Budget Source | View Detail Budget Source | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Budget Source | Export Budget Source List | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Budget Source | Update Budget Source Status | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Stock Taking Period | View Stocktaking Period List | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Stock Taking Period | Export Stocktaking Period List | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Stock Taking Period | Create Stocktaking Period | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Stock Taking Period | Edit Stocktaking Period | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Stock Taking Period | Update Stocktaking Period Status | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Material Data | View List Material Data | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Material Data | Export Material Data | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Material Data | Download Template for Import Material Data | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Material Data | Import Material Data | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Material Data | View Detail Material Data | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Material Data | Edit Material Data | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Material Data | Update Material Status | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Material Data | View List Material Data Non Hierarchy | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Material Data | View Detail Material Data Non Hierarchy | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Material Data | Export Material Data Non Hierarchy | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Material Data | Import Material Data Non Hierarchy | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Material Data | Edit Material Data Non Hierarchy | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Impor Material-Entity Management | View Import Material-Entity History Log | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Impor Material-Entity Management | Download Template for Import Material-Entity Relation on Entity | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Impor Material-Entity Management | Import Material-Entity Relation | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Protocol | View Detail and Configure Protocol | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Protocol | Deactivate | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Asset Model | View List Asset Model | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Asset Model | Export Asset Model | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Asset Model | View Detail Asset Model | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Asset Model | Update Asset Model Status | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Asset Type | View List Asset Type | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Asset Type | Export Asset Type | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Asset Type | View Detail Asset Type | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Asset Type | Update Asset Type Status | ✔️ | ❌ | ✔️ | ❌ |
| Program Setting - Manufacturer | View Manufacturer List | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Manufacturer | View Detail Manufacturer | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Asset Vendor | View List Asset Vendor | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Asset Vendor | Export Asset Vendor | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Asset Vendor | View Detail Asset Vendor | ✔️ | ✔️ | ✔️ | ✔️ |
| Program Setting - Asset Vendor | Update Asset Vendor Status | ✔️ | ❌ | ✔️ | ❌ |


