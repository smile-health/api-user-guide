# Auth & Profile API Endpoints

> ℹ️ Last updated : 12 Jan 2026  

## Table of Contents
- [About](#about)
- [API Endpoints](#api-endpoints)






## About
---
The document outlines various API endpoints related to the Authentication service. It includes methods for performing Authentication functionalities and features through the API, such as Login and Logout. Each endpoint is associated with a specific HTTP method and a brief description of its functionality.


## API Endpoints
---
> ℹ️ Click on each **API URL** entry from the table below to view the API’s detailed documentation.

| Type | API URL | API Name | Used by Web | Used by Mobile App |
|------|---------|----------|:-----------:|:------------------:|
| POST   | /login                       | Login                   | ✔️        | ✔️     |
| GET    | /validate-token              | Validate Token          | ✔️        | ✔️     |
| POST   | /logout                      | Logout                  | ✔️        | ✔️     |
| GET    | /account/profile             | Profile                 | ✔️        | ✔️     |
| GET    | /users/{keycloak_uuid}      | Get Detail Users by Keycloack         | ✔️        | ✔️     |
| GET    | /users/{id}/chg_history      | Get Change Logs         | ✔️        | ✔️     |
| PUT    | /users/{id}                  | Edit User               | ✔️        | ✔️     |
| POST   | /account/update-password     | Update Password         | ✔️        | ✔️     |
| GET    | /account/workspaces          | Get User’s Workspaces   | ✔️        | ✔️     |
| POST    | /account/login          | Login As Role   | ✔️        | ✔️     |
| POST    | /account/logout          | Logout As Role   | ✔️        | ✔️     |
| GET    | /permissions          | Get List Permissions   | ✔️        | ✔️     |
| GET    | /permissions          | Get List Permissions   | ✔️        | ✔️     |
| POST    | /roles          | Create Role Permissions  | ✔️        | ✔️     |
| PUT    | /roles/{id}                  | Update Role Permissions               | ✔️        | ✔️     |
| GET    | /roles          | Get List Role Permissions  | ✔️        | ✔️     |
| GET    | /roles/{id}          | Get Detail Role Permissions  | ✔️        | ✔️     |
| DELETE    | /roles/{id}          | Delete Detail Role Permissions  | ✔️        | ✔️     |







