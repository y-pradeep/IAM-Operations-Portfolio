# Disable User Account in Microsoft Entra ID

## Objective

To disable a user's sign-in access in Microsoft Entra ID when the account is no longer required or access needs to be temporarily or permanently blocked.

## Business Requirement

As part of the IAM Joiner-Mover-Leaver (JML) process, user accounts must be disabled promptly when an employee leaves the organization, a contract ends, or access needs to be revoked.

This helps prevent unauthorized access to organizational applications and resources.

## Pre-requisites

- Access to the Microsoft Entra admin center.
- Appropriate administrative permissions to manage user accounts.
- Approved access request / offboarding request.
- User's User Principal Name (UPN) or other unique identifier.
- Verify that the correct user account has been identified before making the change.


## Steps of the Task

### Step 1: Login to Microsoft Entra Admin Center

Navigate to the Microsoft Entra admin center and sign in with an authorized administrator account.

### Step 2: Navigate to Users

Go to:

Microsoft Entra ID → Users → All users

### Step 3: Search for the User

Search for the user using the User Principal Name (UPN) or other unique identifier.

Verify the user's details before proceeding.

### Step 4: Open User Account

Select the required user account and open the user's profile.

### Step 5: Disable the Account

Navigate to the user's account properties and set:

Block sign-in → Yes

Save the changes.

### Step 6: Verify the Account Status

Reopen the user's profile and confirm that sign-in is blocked.

*** User Account has been disabled successfully ***
The account should show that the user is disabled / blocked from signing in.

Step 7: Revoke Sessions

If required by the organization's offboarding or security procedure, revoke the user's active sessions to terminate existing authentication sessions.

Step 8: Update the Request

Update the corresponding IAM/ITSM ticket with:

- Action performed
- User account
- Date/time
- Result/status
- Any relevant audit evidence

Status: Completed