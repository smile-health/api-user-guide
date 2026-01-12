# Inventiry Role Matrix

> ℹ️ Last updated: 12 Jan 2026

## Table of Contents
- [About](#about)
- [Role Matrix](#role-matrix)

---

## About

The **Inventory Service** is designed to provide a structured and efficient approach to 
managing stock-related data while ensuring precise role-based access control. With 
permissions defined for different user roles, it distinguishes between full access and 
view-only capabilities across both web and mobile platforms, maintaining security and 
operational efficiency.

This service enables users to monitor stock levels, access detailed batch information, and 
track inventory across materials, including those with and without hierarchical structures. 
It also supports the visibility of trademark materials and budget details within batch records, 
ensuring a comprehensive overview of inventory status. Additionally, authorised users on the 
web platform can export stock lists, facilitating better reporting and data management.

With well-defined roles, including Super Admin, Admin, Manager, and Operator, the Inventory 
Service ensures that each user has appropriate access based on their responsibilities. 
This structured approach enhances inventory transparency while maintaining control over 
sensitive data.

---

## Role Matrix
> ℹ️ **Super Admin** and **Admin** can view the inventory of **all entities**;
> **Manager** and **Operator** can only view the inventory of their **own associated entity**.

| **Functionality** | **Feature** | **Super Admin - Web - Full** | **Super Admin - Web - View Only** | **Admin - Web - Full** | **Admin - Web - View Only** | **Manager - Web - Full** | **Manager - Web - View Only** |  **Manager - Mobile - Full** | **Manager - Mobile - View Only** |  **Operator - Mobile - Full** | **Operator - Mobile - View Only** | 
|----------|----------|----------|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| View Stock | View Stock of Material Non-Hierarchy | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| View Stock | View Stock Detail per Activity of Material Non-Hierarchy | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| View Stock | View Batch Detail per Activity of Material Non-Hierarchy | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| View Stock | View Stock of Material with Hierarchy | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| View Stock | View Stock of Product Varian Material with Hierarchy | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| View Stock | View Batch Detail of Product Varian Material with Hierarchy | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| View Stock | View Budget Detail in Batch Detail | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| View Stock | Export Stock List | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ |





