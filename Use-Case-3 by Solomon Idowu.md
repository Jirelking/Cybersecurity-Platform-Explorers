# Use Case 3: Role-Based Application Access Package for Cybersecurity Group 1 Team 

## Microsoft Solution
Microsoft Entra ID Governance

##Project By: 
Cybersecurity Group 1

##Program: 
Platform Explorers – Cybersecurity

##Date: 
3rd of June, 2026

## Overview
This project demonstrates how to implement **Role-Based Access Control (RBAC)** using **Microsoft Entra ID Governance (Access Packages)**.

The goal is to streamline access management by:
- Creating access packages for teams
- Enforcing approval workflows
- Automating access expiration
- Performing access reviews every 6 months

---

##  Objectives
- ✅ Create access packages for teams
- ✅ Assign access to users or groups
- ✅ Enable approval-based access requests
- ✅ Automate access reviews every 6 months
- ✅ Improve security and compliance

---

##  Architecture

``
User → Access Package → Apps / Groups / Resources
↓
Approval Process
↓
Access Granted
↓
Access Review (6 Months)

##  Technologies Used
- Microsoft Entra ID
- Microsoft Entra ID Governance
- Access Packages (Entitlement Management)
- Azure AD Security Groups
- Enterprise Applications

---

##  Implementation Steps

###  Step 1: Create Groups

Create required groups: 

Group Name: Group 1 Collaboration

<img width="1913" height="914" alt="Group 1 catalog" src="https://github.com/user-attachments/assets/ebd403fd-2991-4611-adaf-6abc1679ef4d" />

                                                  Fig 1: Group 1 Collaboration Page

---

### 🔹 Step 2: Go to Identity Governance
1. Open **Microsoft Entra Admin Center**
2. Navigate to:

Identity Governance → Entitlement Management → Access Packages

<img width="1908" height="912" alt="1" src="https://github.com/user-attachments/assets/a9dd5532-b4a9-42b5-91cf-fc2866e1f4c6" />

                                            Fig 2: New access package creation group

---

### 🔹 Step 3: Create Access Package
- Click: **New Access Package**
- Name: `Group 1 Access Package`
- Description: `To give access to the group members`

<img width="1908" height="912" alt="1" src="https://github.com/user-attachments/assets/ffbbe170-30c5-43d8-a082-d1bbf75081c3" />

                                                Fig 3: New Access Package Creation 

---

### 🔹 Step 4: Add Resources
Add:
- Security Groups
- Applications
- SharePoint sites 

<img width="1913" height="912" alt="2" src="https://github.com/user-attachments/assets/b44561fa-1169-405f-81f3-2374248e2e7a" />

                                                  Fig 4: To Add Resource Page

---

### 🔹 Step 5: Create Policy

#### ✅ Request Settings
- Allow users in directory
- Require justification

- #### ✅ Approval Settings
- Enable approval
- Assign approvers:

<img width="1919" height="907" alt="3" src="https://github.com/user-attachments/assets/33ec879e-2638-458e-aff1-efde489c14f1" />

                                          Fig 5a: Allow user request policy creation

<img width="1916" height="909" alt="4" src="https://github.com/user-attachments/assets/4653f7dd-fbdd-4d81-afb0-be966afdaf72" />

                                           Fig 5b: Allow user request policy creation

<img width="1919" height="899" alt="5" src="https://github.com/user-attachments/assets/133de7df-d8fd-4650-808a-38057b41e5ab" />
                                      
                                           Fig 5c: Allow user request policy creation

<img width="1916" height="915" alt="6" src="https://github.com/user-attachments/assets/c14ff1e7-6f2a-4f49-88a4-e1401be89e4a" />
                     
                                           Fig 5d: Allow user request policy creation

---

#### 🔹 Step 6: Lifecycle Settings
- Expiration: **180 days (6 months)**
- Allow renewal

<img width="1565" height="913" alt="7" src="https://github.com/user-attachments/assets/368d217e-cdc2-4287-88f0-0c9b6649933e" />

                                            Fig 6a: Lifecycle Settings Page

<img width="1918" height="901" alt="8" src="https://github.com/user-attachments/assets/40ce993d-b70a-4d47-b935-08de88f4798c" />

                                            Fig 6b: Lifecycle Settings Page

---

### 🔹 Step 7: Enable Access Reviews
- Frequency: **Every 6 months**
- Reviewers:
- Managers
- Resource Owners

<img width="1919" height="908" alt="10" src="https://github.com/user-attachments/assets/4b246065-6d15-4780-94c5-af7174ee5306" />

                                                Fig 7a: Access Review Page

<img width="1919" height="911" alt="11" src="https://github.com/user-attachments/assets/3a9e9f76-faf6-4980-80f5-ca2836cf6eaf" />

                                                Fig 7b: Access Review Page
              
<img width="1919" height="917" alt="12" src="https://github.com/user-attachments/assets/3084ad56-7f2e-41ee-954f-861ddddee1cf" />

                                                Fig 7c: Access Review Page



### 🔹 Step 8: Assign Access

#### Option 1: User Request
- Via **My Access Portal**

- https://myaccess.microsoft.com/@freepengo.com#/access-packages/cb03fe11-4b00-48d7-8199-9e966506ea6b

#### Option 2: Admin Assignment
- Assign users/groups directly

---

### 🔹 Step 9: Testing
1. User requests access

<img width="1919" height="893" alt="Access Request" src="https://github.com/user-attachments/assets/54a6a2df-e059-479f-abff-7d648a28a0a7" />

                                                      Fig 9a: Request Access Page 1


   <img width="1918" height="886" alt="Additional Question" src="https://github.com/user-attachments/assets/76e5d5e6-74ef-4188-ad3d-638be97393b1" />

                                                      Fig 9b: Request Access Page 2




2. Approver approves

 
3. Access is granted
 

4. Verify group membership + app access  

---
