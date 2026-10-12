# Create Security Group in Microsoft Entra ID

## Objective

To create a Security Group in Microsoft Entra ID for managing access to applications, resources, and permissions.

## Business Requirement

Security Groups are used to manage user and device access efficiently through group-based access control and RBAC.

## Pre-requisites

- Access to the Microsoft Entra admin center.
- Appropriate permissions to create groups.
- Approved group creation request.
- Group name and description.
- Defined group purpose and ownership.
- Membership type identified as Assigned or Dynamic.

## Steps of the Task

### Step 1: Navigate to Groups

Go to:

Microsoft Entra ID → Groups → All groups

<img width="1888" height="917" alt="image" src="https://github.com/user-attachments/assets/638f6fe1-a498-4ea6-9494-df935f175968" />

### Step 2: Create Group

Select:

New group

### Step 3: Configure Group Details

Select:

- Group type: Security
- Group name: Enter the required group name
- Group description: Enter the purpose of the group
- Microsoft Entra roles can be assigned to the group: Select as required
- Membership type: Assigned (If Assigned membership is selected, members can be added manually.)
  
<img width="1906" height="584" alt="image" src="https://github.com/user-attachments/assets/87026bd2-97a5-420b-b0ee-82b8a159fd55" />


### Step 4: Add Owner & Members

Select the required group owner & add the members
<img width="1916" height="949" alt="image" src="https://github.com/user-attachments/assets/23f5b241-463c-4b62-a2fc-4a307155218c" />

<img width="1905" height="955" alt="image" src="https://github.com/user-attachments/assets/1ebefc81-e727-498b-b6ad-e7e7dff17d29" />

### Step 5: Create the Group

Select Create.

### Step 6: Verify

Verify that the group appears under:

Microsoft Entra ID → Groups → All groups

<img width="1911" height="930" alt="image" src="https://github.com/user-attachments/assets/ff7826ec-f006-436c-8825-f6bfcff3b7f3" />
