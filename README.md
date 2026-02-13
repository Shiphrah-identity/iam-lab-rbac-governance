# IAM Lab – Active Directory RBAC & Identity Governance (Hands-On)

This repository documents a hands-on Identity & Access Management (IAM) lab focused on **Active Directory identity structure** and **role-based access control (RBAC)** using **security groups**.

The goal was to simulate how real organizations structure identities and manage access **at scale** using governance-friendly patterns (groups, delegation, and access inheritance).

---
Skills Demonstrated

Identity provisioning (ADUC)

OU design for delegation

RBAC via security groups

Least privilege + auditability

Access inheritance validation

## What I Built (Lab Summary)

### ✅ Identity Structure (Active Directory)
- Created an on-prem AD domain (`corp.local`)
- Organized identities using **Organizational Units (OUs)**:
  - HR
  - IT
  - ServiceAccounts
  - Users
- Provisioned demo users:
  - `jsmith`, `hruser`, `itadmin`, `serviceacct`

### ✅ RBAC via Security Groups
- Created security groups aligned to role/dept:
  - `HR_Group`
  - `IT_Admins`
  - `Finance_Group`
- Assigned access using **group membership** (not user-by-user permissions)

### ✅ Access Inheritance (Proof of RBAC)
- Verified users inherit role access through the **Member Of** relationship  
  (centralized access management + audit-friendly governance)

---

## Screenshots (Evidence)

> Add your annotated images into `/images/` and update the paths below.

### 1) OU Structure – Departmental Segmentation
![OU Structure](images/slide1-ou-structure.png)

### 2) Security Group Membership – RBAC Assignment
![RBAC Assignment](images/slide2-rbac-assignment.png)

### 3) User Membership – RBAC Enforcement
![RBAC Enforcement](images/slide3-rbac-enforcement.png)

---

## Why This Matters (IAM Thinking)

### RBAC (Role-Based Access Control)
Instead of assigning permissions directly to users, access is assigned to **groups aligned to roles**.
This approach supports:
- **Least privilege**
- **Scalability**
- **Auditability**
- **Faster onboarding/offboarding**
- **Cleaner governance**

### Delegation-Friendly Structure
Departmental OUs make it easier to:
- delegate administration to appropriate teams
- apply policies consistently
- maintain clean identity boundaries

---

## Key Learnings

- **Structure matters**: OUs make identity administration scalable and organized.
- **Groups are governance**: group-based provisioning reduces complexity and audit risk.
- **Inheritance is the enforcement layer**: the user’s access story is visible and verifiable.

---

## How to Reproduce (High-Level Steps)

1. Install AD DS on Windows Server and promote to Domain Controller
2. Create OUs (HR, IT, ServiceAccounts, Users)
3. Create users aligned to each OU
4. Create security groups aligned to department roles
5. Add users to groups and validate “Member Of” inheritance

---

## Roadmap (Next Enhancements)
- Extend to Microsoft Entra ID (cloud identities)
- Add Conditional Access + MFA enforcement
- Add Access Reviews + PIM (Privileged Identity Management)
- Simulate Joiner/Mover/Leaver lifecycle controls

---

## Contact
If you work in IAM / Identity Security and want to connect, feel free to reach out on LinkedIn.
# iam-lab-rbac-governance
