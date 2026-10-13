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

### Step 2: Select the Group

Search for and select the required Security Group.

### Step 3: Navigate to Licenses

Select:

Licenses

### Step 4: Add License

Select:

Assignments

Choose Add and select the required license.

### Step 5: Configure License Options

Review the available service plans and disable any services that are not required, if applicable.

### Step 6: Assign the License

Select:

Save

The license will be assigned to eligible members of the group.

### Step 7: Verify

Verify the license assignment under:

Group → Licenses

Then verify that the expected group members have received the assigned license.