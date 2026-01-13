# Disposal Role Matrix

> ℹ️ Last updated: 13 Jan 2026

## Table of Contents
- [About](#about)
- [Role Matrix](#role-matrix)

---

## About

The **Disposal Role Matrix** defines the permissions and access levels for each role within the Disposal Service, 
ensuring a clear and structured workflow. It categorizes user roles based on their ability to view, manage,
and process disposal across different stages.

Higher-level roles, such as Super Admin and Admin, have full access to disposal management, including viewing 
all disposal, updating statuses and exporting disposal-related documents. Managers can track and manage 
disposal but have restrictions on administrative functions like exporting reports and downloading specific 
documents. Operators has limited privileges where they focus on on-field operational flow only to submit 
disposal and update certain statuses on mobile.

By structuring these roles and their functionalities, the **Disposal Role Matrix** ensures secure, efficient, 
and role-specific access to order processing while maintaining clear accountability.

---

## Role Matrix
> ℹ️ **Super Admin** and **Admin** can view the disposal of **all entities**;
> **Manager** and **Operator** can only view the disposal of their **own associated entity**.

| **Functionality** | **Feature** | **Super Admin - Web - Full** | **Super Admin - Web - View Only** | **Admin - Web - Full** | **Admin - Web - View Only** | **Manager - Web - Full** | **Manager - Web - View Only** |  **Manager - Mobile - Full** | **Manager - Mobile - View Only** |  **Operator - Mobile - Full** | **Operator - Mobile - View Only** | 
|----------|----------|----------|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| View Disposal Shipment | View All Disposal Shipment List | ✅ | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| View Disposal Shipment | View Disposal Shipment List as Sender | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| View Disposal Shipment | View Disposal Shipment List as Receiver | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Detail Disposal Shipment | View Detail Disposal Shipment with status "Shipped" | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Detail Disposal Shipment | View Detail Disposal Shipment with status "Fulfilled" | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Detail Disposal Shipment | View Detail Disposal Shipment with status "Cancelled" | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Detail Disposal Shipment | View Detail Material Disposal | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Detail Disposal Shipment | Input Comment on Detail Disposal Shipment | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Download Disposal Shipment Document | Export Disposal Shipment List | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ |
| Download Disposal Shipment Document | Download Handover Report Document | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ |
| Create Disposal Shipment | Select Sender Entity on Disposal Shipment | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Shipment | Select Receiver Entity on Disposal Shipment | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Shipment | Select Activity on Disposal Shipment | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Shipment | Select Material on Disposal Shipment | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Shipment | Input Batch Material Quantity on Disposal Shipment | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Shipment | Input Non Batch Material Quantity on Disposal Shipment | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Shipment | Preview disposal before Submit Disposal Shipment | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Shipment | Input Disposal Report Number | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Shipment | Input Comment on Disposal Shipment | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Shipment | Submit Disposal Shipment | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| View Self Disposal | View Self Disposal List | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Detail Self Disposal | View Detail Self Disposal with Batch Material | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Detail Self Disposal | View Detail Self Disposal with Detail Material | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Download Self Disposal Document | Export Self Disposal List | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ |
| Create Self Disposal | Select Entity on Self Disposal | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Self Disposal | Select Activity Entity on Self Disposal | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Self Disposal | Select Disposal Method on Self Disposal | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Self Disposal | Select Material on Self Disposal | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Self Disposal | Input Batch Material Quantity on Self Disposal | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Self Disposal | Input Non Batch Material Quantity on Self Disposal | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Self Disposal | Preview disposal before Submit Self Disposal | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Self Disposal | Input Handover Report Number Disposal | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Self Disposal | Input Comment on Self Disposal | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Self Disposal | Submit Self Disposal | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| View Disposal Instruction | View Disposal Instructionl List | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Detail Disposal Instruction | View Detail Disposal Instruction with status "WMS data is not yet available" | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Detail Disposal Instruction | View Detail Disposal Instruction with status "WMS Synchronisation" | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Detail Disposal Instruction | View WMS Detail on Detail Disposal Instruction | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Detail Disposal Instruction | View WMS Statuses History on Detail Disposal Instruction | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Detail Disposal Instruction | Input Comment on Detail Disposal Instruction | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Download Disposal Instruction Document | Export Disposal Instruction List | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ |
| Download Disposal Instruction Document | Download Handover Report Document | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ |
| Create Disposal Instruction | Select Entity on Disposal Instruction | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Instruction | Select Activity Entity on Disposal Instruction | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Instruction | Select Disposal Method on Disposal Instruction | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Instruction | Select Material on Disposal Instruction | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Instruction | Input Batch Material Quantity on Disposal Instruction | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Instruction | Input Non Batch Material Quantity on Disposal Instruction | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Instruction | Preview disposal before Submit Disposal Instruction | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Instruction | Input Handover Report Number Disposal | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Instruction | Input Comment on Disposal Instruction | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
| Create Disposal Instruction | Submit Disposal Instruction | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ | ✅ | ❌ |
