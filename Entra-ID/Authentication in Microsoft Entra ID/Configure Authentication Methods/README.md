# Configure Authentication Methods

## Objective
Configure and manage authentication methods in Microsoft Entra ID to provide secure and flexible authentication options for users.

## Business Requirement
Organizations need centralized control over authentication methods to strengthen identity security, support Multi-Factor Authentication (MFA), and enable modern authentication methods across the environment.

## Pre-Requisites
- Microsoft Entra ID tenant
- Microsoft Entra ID P1 or P2 license
- Global Administrator or Authentication Policy Administrator role
- Access to Microsoft Entra Admin Center
- Defined authentication strategy and user groups

## Steps of the Task

1. Sign in to the Microsoft Entra Admin Center.
   <img width="1917" height="961" alt="MS Entra Admin Center" src="https://github.com/user-attachments/assets/e8d02d40-d14f-48b1-b4f7-1c00714ae380" />

2. Navigate to **Protection** → **Authentication Methods**.
3. Select **Policies**.
 <img width="1920" height="955" alt="image" src="https://github.com/user-attachments/assets/13c6571b-1f31-46b2-849a-ff41c4a995b5" />

4. Review the available authentication methods.
5. Enable the required authentication methods based on business requirements.
   <img width="1920" height="958" alt="image" src="https://github.com/user-attachments/assets/d79bc8d3-5744-45a9-80f5-5bd8db681f47" />

6. Assign the policy to specific users or groups.
    <img width="1908" height="950" alt="image" src="https://github.com/user-attachments/assets/9b1fb156-d17d-467a-99c1-0898889ae6e9" />

7. Configure method-specific settings as required.
    <img width="1908" height="940" alt="image" src="https://github.com/user-attachments/assets/80c2e70c-7453-4657-90c2-fdd81197f001" />

8. Click **Save** to apply the configuration.
9. Verify policy assignments and effective settings.
10. Test authentication methods with pilot users before production rollout.
