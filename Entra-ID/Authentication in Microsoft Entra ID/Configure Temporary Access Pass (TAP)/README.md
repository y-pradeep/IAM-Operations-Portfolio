# Configure Temporary Access Pass (TAP)

## Objective
Enable Temporary Access Pass (TAP) to facilitate onboarding and recovery scenarios for users.

## Business Requirement
Temporary Access Pass allows users to register passwordless authentication methods securely without requiring existing MFA methods.

## Pre-Requisites
- Microsoft Entra ID tenant
- Microsoft Entra ID P1 or P2 license
- Authentication Administrator role
- Passwordless authentication strategy defined

## Steps of the Task

1. Sign in to the Microsoft Entra Admin Center.
 <img width="1917" height="961" alt="MS Entra Admin Center" src="https://github.com/user-attachments/assets/e63683e6-8869-4045-8c06-04965248f505" />

2. Navigate to **Protection** → **Authentication Methods**.
 <img width="1920" height="955" alt="Authentication methods" src="https://github.com/user-attachments/assets/ceaa637b-b24c-474b-affa-08a76a0495a0" />

3. Select **Temporary Access Pass**.
4. Enable the policy.
   <img width="1915" height="585" alt="image" src="https://github.com/user-attachments/assets/8d0e0bb1-5f5a-4ce4-810d-ad761cd5f521" />

5. Assign target users or groups.
 <img width="1906" height="949" alt="image" src="https://github.com/user-attachments/assets/b9343365-8519-4b47-83f2-b06c76c549d3" />

6. Configure pass lifetime.
7. Configure pass length and one-time use settings.
 <img width="1897" height="945" alt="image" src="https://github.com/user-attachments/assets/b8330133-a9f7-4dbc-afbe-32bda6da2723" />

8. Save the configuration.
9. Navigate to **Users** and select the target user.
10. Generate and securely share the Temporary Access Pass and share it with user for login.
 <img width="1890" height="957" alt="image" src="https://github.com/user-attachments/assets/fd78efce-85e1-4379-a1fd-4df7fa82ea53" />

