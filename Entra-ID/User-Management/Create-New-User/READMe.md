# Microsoft Entra ID - New User Account Creation

## Objective

Create a cloud-only New User Account in Microsoft Entra ID. 

## Business Requirement
Provision a New user account to provide access to organizational resource and Microsoft 365 services.

## Prerequisites

Before creating a new user account, verify the following requirements:

- Microsoft Entra Administrator privileges:
  - User Administrator
  - Global Administrator
  - Privileged Role Administrator (if required)
- Approved user onboarding request.
- Required user information:
  - First Name
  - Last Name
  - Display Name
  - User Principal Name (UPN)
  - Department
  - Job Title
  - Manager Information
  - Usage Location
  - License Requirements
- Network access to Microsoft Entra Admin Center.

---

# User Creation Process

### Step 1: Access Microsoft Entra Admin Center

1. Navigate to:

   ```
   https://entra.microsoft.com
   ```
   <img width="1913" height="954" alt="image" src="https://github.com/user-attachments/assets/02729d36-e7cd-44f9-a495-a96eede3f470" />


2. Sign in with an administrative account.
---

### Step 2: Navigate to Users

1. Select **Entra ID**.
2. Select **Users**.
3. Click **All Users**.
4. Select **+ New User**.
<img width="1913" height="957" alt="image" src="https://github.com/user-attachments/assets/f7d1a83a-99d3-41a4-bd00-048dc0e71d36" />

---

### Step 3: Choose User Creation Type

Select one of the following options:

- Create New User

Creates a cloud-only user account directly in Microsoft Entra ID.

- Invite External User

Creates a guest account for external collaboration.

For employee onboarding, select:

```
Create New User
```
<img width="1911" height="314" alt="image" src="https://github.com/user-attachments/assets/ff7480b7-825d-4152-8ac4-f0897ea11a20" />

---

### Step 4: Configure Basic User Information

Populate the required fields:

| Field | Example |
|---------|---------|
| User Principal Name | john.doe@ABC.com |
| Display Name | John Doe |
| Mail Nickname | johndoe |
| First Name | John |
| Last Name | Doe |

---

### Step 5: Configure Account Settings

### Account Enabled

Ensure:

```
Enabled = Yes
```

### Password Settings

Choose either:

- Auto-generated password (recommended)
- Custom temporary password

Example:

```
Temp Password: P@ssw0rd!2025
```

> Note: Users must change their password during first sign-in.

Enable:

```
Require password change on first login = Yes

```
<img width="1910" height="954" alt="image" src="https://github.com/user-attachments/assets/168df5b1-0748-428e-a702-f50cdfad09dd" />
---

```
```
### Step 6: Assign Organizational Information

Populate business attributes:

| Attribute | Example |
|------------|---------|
| Department | Information Technology |
| Job Title | Systems Engineer |
| Company Name | Contoso Ltd |
| Office Location | Bangalore |
| Employee ID | EMP001234 |
| Manager | Jane Smith |

Select the user's operating country.

Example:
```
India

This setting is mandatory before assigning Microsoft licenses.

```
<img width="1919" height="952" alt="image" src="https://github.com/user-attachments/assets/82396c72-f859-405b-b402-c4cd9c4132d0" />

---
```
```
### Step 7: Assign Group Memberships

Add the user to appropriate security groups and Microsoft 365 groups.

Examples:

| Group | Description |
|---------|---------|
| Sales-Team | Members of Sales Department |
<img width="1920" height="959" alt="image" src="https://github.com/user-attachments/assets/828eadab-6bb0-40e6-a883-f121e5a6bc29" />

---
### Step 8: Assign Roles

Add the user to appropriate roles to the user account based on the access.

Examples:

| Role| Description |
|---------|---------|
| Helpdesk-Administrator | Can reset passwords for non-administrators and Helpdesk Administrators. |

<img width="1913" height="952" alt="image" src="https://github.com/user-attachments/assets/696c30a3-777b-4224-9330-5ee797cd75bf" />


## Step 09: Review and Create

Review all entered information.

Verify:

- User Principal Name
- Display Name
- Usage Location
- Group Memberships
- License Assignments

Click:

```
Review + Create
```

Then select:

```
Create
```
<img width="1920" height="957" alt="image" src="https://github.com/user-attachments/assets/e7ea58d6-51b8-4e93-ac88-ec7f7c625d5b" />

---

### New User Account Created Successfully ###
<img width="1905" height="945" alt="image" src="https://github.com/user-attachments/assets/74099427-6919-4f06-86cd-9b299ba7acfe" />


