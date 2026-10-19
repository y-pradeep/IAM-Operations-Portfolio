# Assign License to Group in Microsoft Entra ID

## Objective

To assign a Microsoft license to a group so that eligible group members receive the assigned license automatically.

## Business Requirement

Group-based licensing simplifies license administration by automatically assigning licenses to users based on their group membership.

This reduces manual license assignment and supports consistent license management.

## Pre-requisites

- Access to the Microsoft Entra admin center.
- Appropriate permissions to manage licenses.
- Approved group-based licensing request.
- Existing Security Group.
- Required license available in the organization's tenant.
- Verify that the selected license is appropriate for the group's members.

## Steps of the Task

### Step 1: Navigate to Groups

Go to:

Microsoft Entra ID → Groups → All groups
<img width="1908" height="942" alt="All groups" src="https://github.com/user-attachments/assets/cf41e35a-8cef-47df-ad30-4b1c442a4b3b" />

### Step 2: Select the Group

Search for and select the required Security Group.
<img width="1913" height="947" alt="image" src="https://github.com/user-attachments/assets/37b29ce1-02e7-4397-8a76-b01af3d80751" />


### Step 3: Navigate to Licenses

Select:

Licenses


### Step 4: Assign the License

Select:

Save
<img width="1915" height="947" alt="image" src="https://github.com/user-attachments/assets/768d086f-1b09-4d94-96e1-51ee4ea32758" />

The license will be assigned to eligible members of the group.

### Step 5: Verify

Verify the license assignment under:

Group → Licenses

Then verify that the expected group members have received the assigned license.
<img width="1913" height="951" alt="image" src="https://github.com/user-attachments/assets/05096ecf-483c-468e-aab6-307c7b61d325" />
