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
<img width="1916" height="952" alt="image" src="https://github.com/user-attachments/assets/cb7cdd2e-106c-40dd-80a1-f128dee9deca" />

### Step 2: Search for the Group

Search for the required deleted group.

Verify that the correct group has been identified.

### Step 3: Select the Group

Select the required deleted group.
<img width="1906" height="923" alt="image" src="https://github.com/user-attachments/assets/6a57a040-8ded-4b7d-b755-c53b3c9d5c47" />

### Step 4: Restore the Group

Select:

Restore group

Confirm the restoration when prompted.
<img width="1910" height="508" alt="image" src="https://github.com/user-attachments/assets/a2c3072e-f1bf-4d7c-bb3e-9464155447cb" />

### Step 5: Verify

Navigate to:

Microsoft Entra ID → Groups → All groups

Search for the group and verify that it has been successfully restored.
<img width="1917" height="396" alt="image" src="https://github.com/user-attachments/assets/61c0da22-3188-40c5-819c-900491f29315" />
