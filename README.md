# az900lab

# Azure Fundamentals (AZ-900) Hands-On Lab

## Overview
This project demonstrates hands-on experience with core Microsoft Azure concepts aligned to the **AZ-900: Microsoft Azure Fundamentals** certification.  
The lab focuses on resource organization, compute, networking, storage, identity, and cost management — without moving into advanced administration topics.

This lab was intentionally designed to remain low-cost and foundational while building a base for future Azure Administrator (AZ-104) and identity labs.

---

## Objectives
- Understand Azure resource hierarchy (subscription, resource groups)
- Deploy and manage basic Azure compute resources
- Configure a virtual network and subnet
- Create and use Azure storage
- Apply Azure RBAC at the resource group level
- Review governance and cost management tools
- Practice cost-safe lab shutdown procedures

---

## Azure Services Used
- Azure Resource Groups
- Azure Virtual Network (VNet)
- Azure Virtual Machine (Windows)
- Azure Storage Account (Blob Storage)
- Microsoft Entra ID (Azure AD)
- Azure RBAC (IAM)
- Azure Advisor
- Azure Cost Management

---

## Lab Architecture
--------------------------------------------------+
|                Azure Subscription                |
|                                                  |
|  +--------------------------------------------+  |
|  |        Resource Group: rg-az900-lab         |  |
|  |                                            |  |
|  |  +-------------+      +----------------+  |  |
|  |  |  Virtual     |      |  Storage       |  |  |
|  |  |  Machine     |      |  Account       |  |  |
|  |  |  vm-az900    |      |  Blob Storage  |  |  |
|  |  +------+------+      +-------+--------+  |  |
|  |         |                         |           |
|  |  +------+-------------------------+--------+ |
|  |  |           Virtual Network (VNet)        | |
|  |  |           10.20.0.0/16                  | |
|  |  |   Subnet: 10.20.1.0/24                  | |
|  |  +------------------------------------------+ |
|  |                                            |  |
|  |  RBAC: Reader Role Assigned via Entra ID   |  |
|  +--------------------------------------------+  |
+--------------------------------------------------+
