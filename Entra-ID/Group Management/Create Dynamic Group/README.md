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
<img width="1908" height="942" alt="All groups" src="https://github.com/user-attachments/assets/d5b9a42c-47d6-4192-9e94-caa0400b82b1" />

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

<img width="1913" height="654" alt="image" src="https://github.com/user-attachments/assets/c93b3d3c-a6b7-46bc-a6f9-4b4ecae97ed1" />

### Step 5: Add Owner

Select the required group owner.

<img width="1916" height="948" alt="image" src="https://github.com/user-attachments/assets/7b2d09e6-2fdf-4c92-85a2-d1d3e89f15b1" />

### Step 6: Create the Group

Select Create.

<img width="1917" height="188" alt="image" src="https://github.com/user-attachments/assets/108ee076-13c6-4584-9b09-d57cbaf964f7" />

### Step 7: Verify

Verify that the group is created and that members are being evaluated according to the configured dynamic rule.

<img width="1920" height="949" alt="image" src="https://github.com/user-attachments/assets/8fc36f13-236d-406d-960f-81eef38234a3" />


<img width="1917" height="476" alt="image" src="https://github.com/user-attachments/assets/1c172563-b703-4322-b26f-dbb992f1e111" />


<img width="1916" height="914" alt="image" src="https://github.com/user-attachments/assets/17baf29f-77ed-4f7a-a214-6905398dcbbc" />


