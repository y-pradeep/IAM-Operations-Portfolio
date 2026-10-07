# Delete User Account in Microsoft Entra ID

## Objective

To permanently remove a user account from Microsoft Entra ID when the identity is no longer required and the applicable retention and offboarding requirements have been completed.

## Business Requirement

As part of the IAM Joiner-Mover-Leaver (JML) process, user accounts that are no longer required must be removed in accordance with the organization's account lifecycle, data retention, and access management policies.

Deleting an account helps maintain a clean identity directory and prevents unnecessary user objects from remaining in the environment.

## Pre-requisites

- Access to the Microsoft Entra admin center.
- Appropriate administrative permissions to delete user accounts.
- Approved deletion/offboarding request.
- Confirmation that the correct user account has been identified.
- Verify that required data, mailbox, licenses, and access have been handled according to organizational policy.
- Confirm that the user is not required for any active business process or application dependency.
- For hybrid users, verify the organization's source-of-authority and synchronization process before deletion.

## Steps of the Task

### Step 1: Login to Microsoft Entra Admin Center

Navigate to the Microsoft Entra admin center and sign in using an authorized administrator account.

### Step 2: Navigate to Users

Go to:

Microsoft Entra ID → Users → All users

### Step 3: Search for the User

Search for the required user using the User Principal Name (UPN) or another unique identifier.

Verify the user's details before proceeding.

### Step 4: Open the User Account

Select the required user account and open the user's profile.

### Step 5: Delete the User

Select:

Delete user

Confirm the deletion when prompted.

### Step 6: Verify the Deletion

Navigate back to All users and search for the deleted user.

The user should no longer appear among active users.

«Deleted users are moved to the Deleted users area and can generally be restored during the configured retention period before permanent deletion.»

*** User Account Deleted Successfully ***