# Auth & Profile Role Matrix

> ℹ️ Last updated : 12 Jan 2026  

## Table of Contents
- [About](#about)
- [Roles Matrix](#roles-matrix)





## About
---
The **Authentication & Profile Role Matrix** is a structured framework that defines which user roles have access to authentication services and the specific features available to each role. It establishes clear guidelines for access control, ensuring that users only interact with authentication mechanisms appropriate to their role.

This document serves as a critical component of security and compliance strategies by preventing unauthorised access, enforcing role-based authentication policies, and maintaining system integrity. By mapping authentication features to all roles, the matrix provides transparency and consistency in authentication management.

## Roles Matrix
---

| Functionality | Feature | Super Admin (Web) | Admin (Web) | Manager (Web) | Manager (Mobile) | Operator (Mobile) | Manufacturer (Web) | Vendor IoT (Web) | Third Party (API) |
|---------------|---------|-------------------|-------------|---------------|------------------|-------------------|--------------------|------------------|-------------------|
| Authentication | Login  | ✔ Full | ✔ View-only | ✔ Full | ✔ View-only | ✔ Full | ✔ View-only | ✔ Full | ✔ Full |
| Authentication | Logout | ✔ Full | ✔ View-only | ✔ Full | ✔ View-only | ✔ Full | ✔ View-only | ✔ Full | ✔ Full |
| Profile | View Current User Profile | ✔ Full | ✔ View-only | ✔ Full | ✔ View-only | ✔ Full | ✔ View-only | ✔ Full | ✔ Full |
| Profile | View Profile Changelog History | ✔ Full | ✔ View-only | ✔ Full | ✔ View-only | ✔ Full | ✔ View-only | ✔ Full | ✔ Full |
| Profile | Edit Profile | ✔ Full | ✔ View-only | ✔ Full | ✔ View-only | ✔ Full | ✔ View-only | ✔ Full | ✔ Full |
| Profile | Edit Password | ✔ Full | ✔ View-only | ✔ Full | ✔ View-only | ✔ Full | ✔ View-only | ✔ Full | ✔ Full |





