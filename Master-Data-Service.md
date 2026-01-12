# Master Data Service

> ℹ️ Last updated : 12 Jan 2026  

## Table of Contents
- [About](#about)
- [Roles](#roles)
- [Associated Component](#associated-component)
- [Special Notes](#special-notes)
  - [Setting Acces Control](#setting-acces-control)
  - [Selected Programs Policy](#selected-programs-policy)
  - [Import Data Performance Improvement](#import-data-performance-improvement)
  - [Create New Program Configuration Steps](#create-new-program-configuration-steps)
  





## About
---

This **Master Data** service serves as a foundational repository for managing system functionalities. It consolidates and manages essential business information across multiple programs, ensuring data consistency and providing a single source of truth for critical operations. This service is divided into **Global Settings** and **Program Settings**, each designed to address specific needs within the system's architecture.

**Global Settings** encompass configurations that are applied globally across all programs, providing a standardised and unified framework for the entire system. These settings ensure consistency and coherence, serving as the foundation for system-wide operations. On the other hand, **Program Settings** focus on configurations related to individual programs. These settings are applied exclusively within the scope of their respective programs, offering flexibility and customisation without impacting the overarching global framework.

The Master Data Service can only be accessed by the **Super Admin** and **Admin**, ensuring it is managed responsibly and securely. More specifically, configuration on **Global Settings** can only be handled by **Super Admin**, while configuration on **Program Settings** can be managed by both **Super Admin** and **Admin**. This repository is accessible solely through the **Web Platform**, maintaining a streamlined and controlled interaction point for managing global and program-specific settings.

## Roles
---

Master Data service can be performed by these roles:
1. Super Admin
2. Admin
   
> ℹ️ For more information about features that each role can perform, please visit the  
> [Master Data Role Matrix](#master-data-role-matrix).

## Associated Component
---
- [Authentication Service](#authentication-service)
- [Inventory Service](#inventory-service)
- [Order Service](#order-service)
- [Transaction Service](#transaction-service)
  
> ℹ️ For more information about the Associated Components, please visit the  
> [Integration Points](#). sections

## Special Notes
---

### Setting Acces Control 
- The Master Data service, including both Global and Program Settings, can only be accessed through the Web platform;.
- **Global Settings** can only be managed by a **Super Admin**;
- **Program Settings** can be managed by both **Super Admin** and **Admin**.


### Selected Programs Policy
- Each user's data needs to be associated with an Entity and a Program;
- Entity, Material, Budget Source, and Manufacturer data can be created without being assigned to a Program;
- Once data has been assigned to a Program, it cannot be removed or unassigned from the Program.

### Import Data Performance Improvement
- Users can create data in bulk by utilising the Import feature in each Master Data functionality;
- Users need to comply with the SMILE Data Template format when importing data;
- To improve import performance and reduce file size, users can delete all other sheets except the **Data Entry** or **Input Data** sheet.

### Create New Program Configuration Steps
The following steps are recommended steps on creating a new program along with configuration to other data:
1. Create a new program
2. Create activities to the program
3. Create a new material (leave the "Program" field empty)
4. Assign the program to entities via Edit Entity
5. Assign the program to users via Edit User
6. Assign the program to materials via Edit Material
7. Assign the program to manufacturers via Edit Manufacturer
8. Assign the program to budget sources via Edit Budget Source
9. Open the program from the Homepage or sidebar
10. Set additional material settings in Program Setting – Material Management
11. Set entity’s vendor status in Program Setting – Material Management
12. Set entity’s activity implementation dates in Program Setting – Entity Management
13. Set entity’s customer-vendor relationships (Distribution and Consumption) in Program Setting – Entity Management
14. Set entity’s material-entity relationships in Program Setting – Entity Management (via Create or Import)





