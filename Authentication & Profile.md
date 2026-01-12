# Authentication & Profile

> **Last updated:** 1 May 2025

## Table of Contents
- [About](#about)
- [Roles](#roles)
- [Associated Component](#associated-component)
- [System Data Architecture](#system-data-architecture)
- [Special Notes](#special-notes)
  - [Token Expiry Time](#token-expiry-time)
  - [Multi-login Mechanism](#multi-login-mechanism)
  - [User Role Login Platform](#user-role-login-platform)
- [Revision History](#revision-history)

---

## About

Authentication in **SMILE** is designed to be secure, scalable, and efficient, ensuring that only authorised users can access the system, particularly given the presence of sensitive clinical data.

SMILE employs a dedicated **Authentication Service** that acts as an abstraction layer over the underlying identity and access management (IAM) tool. Currently, this Authentication Service is built on top of **Keycloak**, an open-source IAM solution that provides robust features such as **Role-Based Access Control (RBAC)** and secure token management using **JSON Web Tokens (JWT)**.

This architectural design allows SMILE to rely on its own authentication interface while retaining the flexibility to switch out the underlying IAM tool in the future without impacting the broader system.

The Authentication Service interacts with both **Keycloak** and the **SMILE Database** to manage user data. Core identity attributes—such as usernames, emails, and roles—are maintained via the Authentication Service and backed by Keycloak. Meanwhile, the SMILE Database holds additional user-related information such as location, phone number, and program assignments.

This separation of concerns ensures:
- Data integrity  
- System flexibility  
- Compliance with security standards  

To further enhance security, the Authentication Service leverages features such as **token expiration and refresh**, ensuring authentication tokens remain valid only for a defined duration.

