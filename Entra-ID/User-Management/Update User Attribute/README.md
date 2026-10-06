# Microsoft Entra ID - User Attribute Update

## Objective

Update one or more attributes of an Existing User account in Microsoft Entra ID.

---

## Business Requirement

User atrributes may need to be updated  due to organizational changes such as department transerfer, job title updates, location changes,
manager changes, or contract information updates. Maintaining accurate user information ensures proper access governance and directory management.

---

## Prerequisites

Before updating user attributes, ensure the following:

- Appropriate Microsoft Entra administrative role:
  - User Administrator
  - Global Administrator
  - Helpdesk Administrator (limited updates)
- Approved service request or HR change request.
- Updated user information received from an authorized source.
- Access to Microsoft Entra Admin Center.

---

## User Attribute Update Process

### Step 1: Access Microsoft Entra Admin Center

Navigate to:

```
https://entra.microsoft.com
```

Sign in using an authorized administrative account.
<img width="1908" height="949" alt="image" src="https://github.com/user-attachments/assets/b7beb470-a60e-46cf-a6e4-63f21b45c631" />

---

## Step 2: Locate the User Account

1. Select **Entra ID**.
2. Select **Users**.
3. Click **All Users**.
4. Search for the target user using:
   - Display Name
   - User Principal Name (UPN)
   - Email Address
   - Employee ID

Example:

```
john.doe@abc.com
```
<img width="1919" height="955" alt="image" src="https://github.com/user-attachments/assets/8b314e29-3016-48dd-9f5b-950108a425b0" />

---

## Step 3: Open User Profile

1. Select the user account.
2. Open the **Properties** section.

Review existing user information prior to making modifications.

<img width="1912" height="953" alt="image" src="https://github.com/user-attachments/assets/111c566a-ec9e-4d8d-9cbb-d3d6677647b5" />

---

## Step 4: Update User Attributes

Modify the required attributes.

### Contact Information

| Attribute | Example Value |
|------------|---------------|
| Street Address | IT Park, Whitefield |
| City | Bengaluru |
| State | Karnataka |
| Postal Code | 123456 |
| Country | India |

<img width="1911" height="947" alt="image" src="https://github.com/user-attachments/assets/ffc9e54d-b696-43df-a3f3-5387f0d67654" />

---

### Organizational Information

| Attribute | Example Value |
|------------|---------------|
| Job Title | Senior Systems Engineer |
| Department | Information Technology |

<img width="1915" height="951" alt="image" src="https://github.com/user-attachments/assets/7a1834ee-12b7-4f6d-903a-63a2b3c6946a" />


---

## Step 5: Save Changes

After reviewing all updates:

1. Select **Save**.
2. Confirm successful update.

Expected Result:

```text
User profile updated successfully.
```
<img width="1910" height="624" alt="image" src="https://github.com/user-attachments/assets/3175338a-8249-4d41-bc1d-19d6fc5d0e89" />

<img width="1173" height="875" alt="image" src="https://github.com/user-attachments/assets/d2a8fd02-0f4f-47b0-aecf-f8160ae93081" />



---

