# Restore Deleted Group in Microsoft Entra ID

## Objective

To restore a previously deleted Microsoft Entra ID group when the group is still within the available recovery period.

## Business Requirement

A deleted group may need to be restored due to accidental deletion or an approved business requirement.

## Pre-requisites

- Access to the Microsoft Entra admin center.
- Appropriate permissions to restore groups.
- Approved restore request.
- Deleted group must still be available within the applicable retention period.
- Group name or other identifying information.

## Steps of the Task

### Step 1: Navigate to Groups

Go to:

Microsoft Entra ID → Groups → Deleted groups

### Step 2: Search for the Group

Search for the required deleted group.

Verify that the correct group has been identified.

### Step 3: Select the Group

Select the required deleted group.

### Step 4: Restore the Group

Select:

Restore group

Confirm the restoration when prompted.

### Step 5: Verify

Navigate to:

Microsoft Entra ID → Groups → All groups

Search for the group and verify that it has been successfully restored.