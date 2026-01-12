# Authentication & Profile

> ℹ️ This article was last updated on 1 May 2025  

## Table of Contents
- [About](#about)
- [Roles](#roles)
- [Associated Component](#associated-component)
- [System Data Architecture](#system-data-architecture)
- [Special Notes](#special-notes)
  - [Token Expiry Time](#token-expiry-time)
  - [Multi-login Mechanism](#multi-login-mechanism)
  - [User Role Login Platform](#user-role-login-platform)





## About
---

Authentication in SMILE is designed to be secure, scalable, and efficient, ensuring that only authorised users can access the system, particularly given the presence of sensitive clinical data. SMILE employs a dedicated Authentication Service that acts as an abstraction layer over the underlying identity and access management (IAM) tool. Currently, this Authentication Service is built on top of Keycloak, an open-source IAM solution that provides robust features such as Role-Based Access Control (RBAC) and secure token management using JSON Web Tokens (JWT). This architectural design allows SMILE to rely on its own authentication interface while retaining the flexibility to switch out the underlying IAM tool in the future without impacting the broader system.

The Authentication Service interacts with both Keycloak and the SMILE Database to manage user data. Core identity attributes—such as usernames, emails, and roles—are maintained via the Authentication Service and backed by Keycloak. Meanwhile, the SMILE Database holds additional user-related information such as location, phone number, and program assignments. This separation of concerns ensures data integrity, system flexibility, and compliance with security standards.

To further enhance security, the Authentication Service leverages features such as token expiration and refresh, ensuring authentication tokens remain valid only for a defined duration. Additionally, the system logs authentication events, allowing administrators to track user activity and effectively monitor security-related incidents.

By incorporating Keycloak through its own Authentication Service, SMILE ensures secure, compliant, and adaptable user access management. This approach enables implementation of RBAC, secure authentication flows, and audit logging while maintaining the agility to evolve its IAM infrastructure as needed.


## Roles
---

The Authentication Service is accessible to all user roles within the system, enabling secure login, logout, and credential recovery for every user. While authentication is required for all roles, the level of access within the application is determined by the user’s assigned role. When a user is created in SMILE, a corresponding identity is established in the underlying IAM system, with role mappings managed centrally. Upon login, role information is included in the authentication token, which the SMILE application uses to determine the specific modules and services each user can access. This approach lays the foundation for a Role-Based Access Control (RBAC) model that ensures users interact only with the parts of the system relevant to their responsibilities.

> ℹ️ **Note**  
> For more information about roles that can access this Authentication service, please visit the  
> [Authentication Role Matrix](#).

## Associated Component
---

This Authentication service is associated with **All Services**, whether Core or Non-Core, to ensure secure access control. Verifying user identities and permissions ensures that only authorised and privileged users can access and perform the functionalities and features assigned to them, maintaining the integrity and security of the system.

## System Data Architecture
---

> ℹ️ **Note**  
> For more information on the Authentication System Architecture, please visit the  
> [System Data Architecture](#). page

## Special Notes
---

### Token Expiry Time
- The user accesses the system by `access_token`.
- The `access_token` will expire after 24 hours.
- For example, if the user logs in to the system at `08:18:14`, then the token will expire at `08:18:14`.
- After 24 hours, the system will refresh the `access_token` using the `refresh_token` without requiring the user to log in again.

> ℹ️ For more information, please visit the [Authentication Implementation Guide](#). page

### Multi-login Mechanism
- A user can log in to only **one device** at a time;
- The term **one device** refers to either a platform or a browser;
- If the user has a valid token to the system (logged in) and then logs in on a second device, the first device will automatically log out, and the token will be automatically expired.

### User Role Login Platform
- Each user has a defined login platform based on their role;;
- For example, the **Operator** user role can only access the system on the **Mobile platform**. Therefore, the Operator role cannot log in to the Web platform..

> ℹ️ For more information, please visit the [Authentication Role Matrix](#). page




