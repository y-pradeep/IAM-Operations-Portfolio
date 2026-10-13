# Create Dynamic Group in Microsoft Entra ID

## Objective

To create a Dynamic Group in Microsoft Entra ID where membership is automatically maintained based on defined membership rules.

## Business Requirement

Dynamic Groups reduce manual group administration by automatically adding or removing users or devices based on their attributes.

## Pre-requisites

- Access to the Microsoft Entra admin center.
- Appropriate permissions to create groups.
- Approved group creation request.
- Group name and description.
- Required membership criteria identified.
- User or device attributes available for the membership rule.

## Steps of the Task

### Step 1: Navigate to Groups

Go to:

Microsoft Entra ID → Groups → All groups

### Step 2: Create Group

Select:

New group

### Step 3: Configure Group Details

Select:

- Group type: Security or Microsoft 365
- Group name: Enter the required name
- Group description: Enter the purpose
- Membership type: Dynamic User or Dynamic Device

### Step 4: Configure Membership Rule

Select:

Add dynamic query

Configure the required membership rule based on user or device attributes.

### Step 5: Add Owner

Select the required group owner.

### Step 6: Create the Group

Select Create.

### Step 7: Verify

Verify that the group is created and that members are being evaluated according to the configured dynamic rule.