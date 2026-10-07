# Bulk User Account Creation in Microsoft Entra ID

## Objective

To create multiple user accounts in Microsoft Entra ID efficiently and consistently using a bulk user creation process.

## Business Requirement

As part of the IAM Joiner process, multiple user accounts may need to be created in Microsoft Entra ID for new employees, contractors, or other workforce populations.

Bulk creation reduces manual effort, improves consistency, and enables efficient onboarding of multiple users.

## Pre-requisites

- Access to the Microsoft Entra admin center.
- Appropriate administrative permissions to create users.
- Approved user creation/onboarding request.
- User details prepared in the required CSV format.
- Unique User Principal Names (UPNs) for all users.
- Required information such as:
  - First name
  - Last name
  - Display name
  - User Principal Name
  - Initial password
  - Usage location, where applicable
- Ensure the CSV file follows Microsoft's required bulk user upload format.

## Steps of the Task

### Step 1: Login to Microsoft Entra Admin Center

Navigate to the Microsoft Entra admin center and sign in using an authorized administrator account.

### Step 2: Navigate to Users

Go to:

Microsoft Entra ID → Users → All users

### Step 3: Select Bulk User Creation

Select:

New user → Bulk create

### Step 4: Prepare the CSV File

Download the CSV template provided by Microsoft Entra ID.

Populate the template with the required user details.

Example:

User name,Name,First name,Last name,Initial password
john.doe@contoso.com,John Doe,John,Doe,TempPassword
jane.smith@contoso.com,Jane Smith,Jane,Smith,TempPassword

«Use the current Microsoft-provided CSV template rather than creating a custom format, as required columns and formatting can vary.»

### Step 5: Upload the CSV File

Select Upload your CSV file and upload the completed CSV file.

Review the file for any validation errors.

### Step 6: Submit the Bulk Creation

Once the CSV file passes validation, select Submit to start the bulk user creation process.

Microsoft Entra ID processes the file and creates the user accounts.

### Step 7: Verify User Creation

Navigate to:

Microsoft Entra ID → Users → All users

Search for the newly created users and verify that the accounts were successfully created.

Validate the required attributes such as:

- Display name
- User Principal Name (UPN)
- Account status
- Usage location
- User type

### Step 8: Validate Access Requirements

Verify that the newly created accounts have the required licenses, groups, roles, and application access according to the approved onboarding requirements.