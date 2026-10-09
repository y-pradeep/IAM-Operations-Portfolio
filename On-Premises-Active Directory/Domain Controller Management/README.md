# Promote Server to Domain Controller

## Overview
This document outlines the procedure for promoting a Windows Server to an Active Directory Domain Services (AD DS) Domain Controller. This activity is a critical task in Identity and Access Management (IAM) and enables centralized authentication, authorization, Group Policy management, and directory services within the enterprise environment.

---

# Task Details

| Item | Details |
|--------|---------|
| Task Name | Promote Server to Domain Controller |
| Technology | Microsoft Active Directory Domain Services (AD DS) |
| Server Role | Domain Controller |
| Administrator Access | Required |
| Change Type | Infrastructure Configuration |
| Impact | Authentication and Directory Services |

---

# Objective

Promote a Windows Server to a Domain Controller to provide Active Directory services for the organization, ensuring centralized identity and access management.

---

# Prerequisites

Before promoting the server, verify the following:

- Windows Server installed and fully patched.
- Static IP address configured.
- Correct hostname assigned.
- DNS server settings configured.
- Local Administrator privileges available.
- Server joined to the network.
- Required firewall ports allowed.
- Server meets enterprise security standards.

---

# Implementation Procedure

## Step 1: Verify Server Configuration

Validate:

- Server hostname
- Static IP configuration
- DNS settings
- Time synchronization
- Network connectivity

### PowerShell Validation

```powershell
ipconfig /all
hostname
ping <DNS_Server_IP>
```
<img width="627" height="473" alt="image" src="https://github.com/user-attachments/assets/30877fc4-b87e-4f43-b94b-3b1cbda22725" />

---

## Step 2: Install Active Directory Domain Services Role

### Server Manager Method

1. Open **Server Manager**.
2. Select **Manage** → **Add Roles and Features**.
   
<img width="1006" height="715" alt="image" src="https://github.com/user-attachments/assets/410c3155-d188-484f-84c3-5ae2101615d6" />

3. Choose **Role-based or feature-based installation**.

<img width="819" height="567" alt="image" src="https://github.com/user-attachments/assets/cb89be94-df0d-4906-a0e8-abb78ac67d42" />

4. Select target server.
   
<img width="785" height="559" alt="image" src="https://github.com/user-attachments/assets/c4c22dc0-2e2a-4eb6-ad28-33bbd95de68a" />

5. Check **Active Directory Domain Services**.
6. Click **Add Features**.
   
<img width="786" height="560" alt="image" src="https://github.com/user-attachments/assets/6c73874e-cdc4-4465-aa5f-6919357146c2" />

7. Proceed through the wizard.
8. Click **Install**.
   

## Step 3: Promote Server to Domain Controller

After AD DS installation completes:

1. Open **Server Manager**.
2. Click the notification flag.
3. Select **Promote this server to a domain controller**.
<img width="1020" height="719" alt="image" src="https://github.com/user-attachments/assets/7610a778-3004-4d6c-a80c-96e2bba1096a" />

---
## Step 4: Select Deployment Configuration

### Add Domain Controller to Existing Domain

Used when deploying an additional Domain Controller.
<img width="869" height="621" alt="image" src="https://github.com/user-attachments/assets/2232a3c6-7911-45da-b02c-4f09c399176a" />

Example:
Existing Domain:
ABC.com

## Step 5: Configure Domain Controller Options

Configure:

- Domain Name System (DNS)
- Global Catalog (GC)
- Site Name
- Directory Services Restore Mode (DSRM) Password

### Recommended Configuration

| Setting | Value |
|----------|--------|
| DNS Server | Enabled |
| Global Catalog | Enabled |
| Read Only DC | Disabled (unless required) |
| DSRM Password | Strong Enterprise Password |
<img width="776" height="567" alt="image" src="https://github.com/user-attachments/assets/b7a60e61-87e1-4c94-8eff-3d52f1575b55" />

---

## Step 6: Review DNS Options

Accept warnings if:

- Creating a new forest
- No existing DNS delegation exists

Proceed by clicking **Next**.
<img width="809" height="582" alt="image" src="https://github.com/user-attachments/assets/9f22547e-fb8c-4213-8424-3167decf9362" />

---

## Step 7: Configure Paths

Default locations:

```
Database Folder:
C:\Windows\NTDS

Log Files:
C:\Windows\NTDS

SYSVOL:
C:\Windows\SYSVOL
```

Modify only if storage architecture requires separate volumes.
<img width="775" height="564" alt="image" src="https://github.com/user-attachments/assets/90634607-86b5-44c6-87ab-e8179e580cd4" />

---

## Step 8: Prerequisites Check

Run validation checks.

Expected Result:

```
All prerequisite checks passed successfully.
```

Resolve any reported errors before continuing.
<img width="803" height="574" alt="image" src="https://github.com/user-attachments/assets/48bdc954-d434-421c-9bff-1af3bb5c48c6" />

---

## Step 9: Install and Promote

Click **Install**.

System will:

- Configure Active Directory
- Install DNS services
- Create SYSVOL
- Promote server as Domain Controller
- Reboot automatically

---

# Post-Implementation Validation

## Verify Domain Controller Status

```powershell
Get-ADDomain
```

Expected output should display:

- Domain Name
- Domain Mode
- PDC Emulator
- RID Master
- Infrastructure Master
<img width="959" height="684" alt="image" src="https://github.com/user-attachments/assets/f2e5b40e-8fab-4f18-abfa-a494992fd51d" />

---

## Verify AD DS Service

```powershell
Get-Service NTDS
```

Expected:

```
Running
<img width="521" height="178" alt="image" src="https://github.com/user-attachments/assets/6b77c4b4-f111-47ef-baee-fe9581cc2456" />

```
