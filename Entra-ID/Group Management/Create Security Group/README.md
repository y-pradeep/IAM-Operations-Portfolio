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

### Step 2: Create Group

Select:

New group

### Step 3: Configure Group Details

Select:

- Group type: Security
- Group name: Enter the required group name
- Group description: Enter the purpose of the group
- Microsoft Entra roles can be assigned to the group: Select as required
- Membership type: Assigned / Dynamic User / Dynamic Device

### Step 4: Configure Membership

If Assigned membership is selected, members can be added manually.

If Dynamic membership is selected, configure the membership rule.

### Step 5: Add Owner

Select the required group owner.

### Step 6: Create the Group

Select Create.

### Step 7: Verify

Verify that the group appears under:

Microsoft Entra ID → Groups → All groups