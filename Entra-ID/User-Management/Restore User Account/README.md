# Restore User Account in Microsoft Entra ID

## Objective

To restore a previously deleted user account in Microsoft Entra ID when the user needs to regain access to organizational resources.

## Business Requirement

A deleted user account may need to be restored due to an accidental deletion, employee rehire, or other approved business requirement.

Restoring the account allows the existing user identity to be recovered without creating a new user account.

## Pre-requisites

- Access to the Microsoft Entra admin center.
- Appropriate administrative permissions to restore deleted users.
- Approved restore request.
- User's User Principal Name (UPN) or other unique identifier.
- Confirm that the correct user account has been identified.
- Verify that the user is available under Deleted users and is within the applicable retention period.

## Steps of the Task

### Step 1: Login to Microsoft Entra Admin Center

Navigate to the Microsoft Entra admin center and sign in using an authorized administrator account.

### Step 2: Navigate to Deleted Users

Go to:

Microsoft Entra ID → Users → Deleted users

### Step 3: Search for the User

Search for the required user using the User Principal Name (UPN) or another unique identifier.

Verify the user's details before proceeding.

### Step 4: Select the User

Select the required deleted user account from the list.

### Step 5: Restore the User

Select:

Restore user

Confirm the restoration when prompted.

### Step 6: Verify the User Account

Navigate to:

Microsoft Entra ID → Users → All users

Search for the restored user and verify that the account has been successfully restored.

### Step 7: Validate the Account

Verify the user's:

- Account status
- User Principal Name (UPN)
- Group memberships
- Licenses
- Application access

Ensure the account is restored as required by the approved request.