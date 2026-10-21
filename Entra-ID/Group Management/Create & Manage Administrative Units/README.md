# Create & Manage Administrative Units in Microsoft Entra ID

## Objective

To create and manage Administrative Units (AUs) in Microsoft Entra ID for delegated administration of users, groups, and devices within a specific organizational scope. Administrative Units enable granular role delegation while maintaining security and governance through the principle of least privilege.

---

## Business Requirement

Organizations with multiple departments, regions, subsidiaries, or business units require decentralized administration without granting tenant-wide administrative privileges. Administrative Units provide a secure mechanism to delegate identity management responsibilities to local administrators while limiting their scope of access.

Key business benefits include:

- Delegated administration for regional or departmental IT teams.
- Reduced dependency on Global Administrators.
- Improved security through scoped administrative permissions.
- Enhanced compliance with segregation of duties requirements.
- Simplified management of users, groups, and devices.
- Better governance and operational efficiency.

---

## Steps of the Task

### Step 1: Sign in to Microsoft Entra Admin Center

1. Open a web browser.
2. Navigate to https://entra.microsoft.com.
3. Sign in using an account assigned one of the following roles:
   - Global Administrator
   - Privileged Role Administrator
   - Role Management Administrator
     
<img width="1917" height="961" alt="MS Entra Admin Center" src="https://github.com/user-attachments/assets/a8e8f586-7c4d-4cd9-aecf-918a985a831d" />

---

### Step 2: Navigate to Administrative Units

1. In the left navigation pane, select **Identity**.
2. Expand **Roles & Admins**.
3. Select **Administrative Units**.
   
<img width="1910" height="947" alt="image" src="https://github.com/user-attachments/assets/e7987ba8-2d9d-4bf1-8dda-ee5b024886a2" />

---

### Step 3: Create a New Administrative Unit

1. Click **+ Add Administrative Unit**.
2. Configure the following settings:

| Setting | Example Value |
|----------|--------------|
| Name | Europe-IT-AU |
| Description | Administrative scope for Europe IT Team |
| Restricted Management Administrative Unit | Yes/No based on business requirement |

<img width="1908" height="953" alt="image" src="https://github.com/user-attachments/assets/f1810732-2b88-4cfe-8e5b-5a84c3d9e295" />

3. Click **Review + Create**.
4. Click **Create**.
<img width="1917" height="945" alt="image" src="https://github.com/user-attachments/assets/71844c54-3bd6-4fe0-becb-31d0bd1c7d55" />

---

### Step 4: Add Users to the Administrative Unit

1. Open the newly created Administrative Unit.
2. Select **Users**.
3. Click **+ Add User**.
4. Search and select required users.
5. Click **Select**.
   
<img width="1917" height="959" alt="image" src="https://github.com/user-attachments/assets/5ef1912f-55b8-4a2e-b740-e5fb6ca77032" />

#### Example

```text
Administrative Unit: Europe-IT-AU

Users:
user1
user2
user3
```

---

### Step 5: Add Groups to the Administrative Unit

1. Open the Administrative Unit.
2. Select **Groups**.
3. Click **+ Add Group**.
4. Select the required Microsoft 365 or Security Groups.
5. Click **Select**.
   
<img width="1918" height="949" alt="image" src="https://github.com/user-attachments/assets/cc6f3b8e-4a91-4916-8e53-41fb8d8455b4" />

#### Example

```text
Europe-IT-Users
Europe-IT-Admins
```

---

### Step 6: Assign Administrative Roles

1. Open the Administrative Unit.
2. Select **Roles and Administrators**.
3. Click **+ Add Assignment**.
4. Select the appropriate role.
5. Select the administrator or administrative group.
6. Click **Assign**.
   
<img width="1917" height="955" alt="image" src="https://github.com/user-attachments/assets/97b889a0-84d8-454f-8807-9bf89429f3c2" />

#### Common Administrative Roles

- User Administrator
- Groups Administrator
- Password Administrator
- Helpdesk Administrator
- Authentication Administrator

#### Example

```text
Role: User Administrator

Assigned To:
Europe-IT-Admins
```

---

### Step 7: Validate Administrative Scope

1. Sign in with the delegated administrator account.
2. Navigate to Microsoft Entra Admin Center.
3. Verify the administrator can manage only:
   - Users within the Administrative Unit
   - Groups within the Administrative Unit
   - Devices within the Administrative Unit
4. Confirm no administrative access exists outside the assigned scope.

---

### Step 8: Modify Administrative Unit Membership

#### Add Members

1. Open the Administrative Unit.
2. Select **Users**, **Groups**, or **Devices**.
3. Click **+ Add**.
4. Select the required objects.
5. Save the changes.

#### Remove Members

1. Select the object from the Administrative Unit.
2. Click **Remove**.
3. Confirm the action.

---

### Step 09: Monitor and Audit Administrative Unit Activities

1. Navigate to **Monitoring & Health**.
2. Select **Audit Logs**.
3. Review activities related to:
   - Administrative Unit creation
   - Membership modifications
   - Role assignments
   - Administrative Unit deletion
4. Export logs if required for compliance or auditing purposes.

---

## Validation

Verify the following:

- Administrative Unit is successfully created.
- Users, groups, and devices are correctly assigned.
- Administrative roles are assigned appropriately.
- Delegated administrators can manage only scoped resources.
- Audit logs record all Administrative Unit activities.
- Least privilege principles are enforced.

---

## Expected Outcome

A Microsoft Entra ID Administrative Unit is successfully created and configured. Scoped administrators can manage designated users, groups, and devices without receiving tenant-wide administrative permissions, resulting in improved security, governance, and operational efficiency.
