# 📌 Role-Based Application Access Package (Microsoft Entra ID Governance)

## 📖 Overview
This project demonstrates how to implement **Role-Based Access Control (RBAC)** using **Microsoft Entra ID Governance (Access Packages)**.

The goal is to streamline access management by:
- Creating access packages for teams
- Enforcing approval workflows
- Automating access expiration
- Performing access reviews every 6 months

---

## 🎯 Objectives
- ✅ Create access packages for teams
- ✅ Assign access to users or groups
- ✅ Enable approval-based access requests
- ✅ Automate access reviews every 6 months
- ✅ Improve security and compliance

---

## 🏗️ Architecture

``
User → Access Package → Apps / Groups / Resources
↓
Approval Process
↓
Access Granted
↓
Access Review (6 Months)

## 🧰 Technologies Used
- Microsoft Entra ID
- Microsoft Entra ID Governance
- Access Packages (Entitlement Management)
- Azure AD Security Groups
- Enterprise Applications

---

## 📋 Prerequisites
- Microsoft Entra ID P2 License
- Admin Role:
  - Global Admin OR Identity Governance Admin
- Pre-created:
  - Security Groups
  - Enterprise Applications

---

## ⚙️ Implementation Steps

### 🔹 Step 1: Create Groups
Create required groups:
- Finance_Group
- HR_Group
- IT_Support_Group

---

### 🔹 Step 2: Go to Identity Governance
1. Open **Microsoft Entra Admin Center**
2. Navigate to:

Identity Governance → Entitlement Management → Access Packages

---

### 🔹 Step 3: Create Access Package
- Click: **New Access Package**
- Name: `Finance Access Package`
- Description: `Access for Finance Team`

---

### 🔹 Step 4: Add Resources
Add:
- Security Groups
- Applications
- SharePoint sites (optional)

Example:
- Finance_App  
- Finance_Group  

---

### 🔹 Step 5: Create Policy

#### ✅ Request Settings
- Allow users in directory
- Require justification

---

#### ✅ Approval Settings
- Enable approval
- Assign approvers:
- Manager
- IT Admin
- Application Owner

---

#### ✅ Lifecycle Settings
- Expiration: **180 days (6 months)**
- Allow renewal

---

### 🔹 Step 6: Enable Access Reviews
- Frequency: **Every 6 months**
- Reviewers:
- Managers
- Resource Owners

Enable:
- Auto apply results
- Remove access if not approved

---

### 🔹 Step 7: Assign Access

#### Option 1: User Request
- Via **My Access Portal**

#### Option 2: Admin Assignment
- Assign users/groups directly

---

### 🔹 Step 8: Testing
1. User requests access  
2. Approver approves  
3. Access is granted  
4. Verify group membership + app access  

---

## 🔍 Regex Enhancement

### ✅ Detect Question
```regex
(?i)may\s+i\s+know\s+the\s+name\s+of\s+your\s+group\s+leader\??


