# Configure Microsoft Authenticator

## Objective
Enable Microsoft Authenticator as an authentication method for Multi-Factor Authentication (MFA) and passwordless sign-in.

## Business Requirement
Microsoft Authenticator provides a secure and user-friendly authentication experience through push notifications, number matching, and passwordless authentication capabilities.

## Pre-Requisites
- Microsoft Entra ID tenant
- Microsoft Entra ID P1 or P2 license
- Global Administrator or Authentication Administrator role
- Microsoft Authenticator application installed on user devices

## Steps of the Task

1. Sign in to the Microsoft Entra Admin Center.
   <img width="1917" height="961" alt="MS Entra Admin Center" src="https://github.com/user-attachments/assets/70c94127-3b5b-4906-a2b1-9bfdd0ac5e2f" />

2. Navigate to **Protection** → **Authentication Methods**.
   <img width="1920" height="955" alt="Authentication methods" src="https://github.com/user-attachments/assets/ce2ad2f9-0398-4419-a462-369c429c1431" />

3. Select **Microsoft Authenticator**.
4. Click **Enable**.
   <img width="1920" height="949" alt="image" src="https://github.com/user-attachments/assets/02c59f70-e048-409f-85e3-0ac67af3c959" />

5. Assign users or groups who will use Microsoft Authenticator.
  <img width="1920" height="950" alt="image" src="https://github.com/user-attachments/assets/6bc955af-4c92-4fe7-b5e3-b174e01306df" />
 
6. Enable **Push Notifications**.
    <img width="1901" height="781" alt="image" src="https://github.com/user-attachments/assets/89571833-91f3-4cfe-888a-a1294b25c214" />

7. Enable **Passwordless Authentication** if required.
8. Configure **Number Matching** settings.
    <img width="1913" height="950" alt="image" src="https://github.com/user-attachments/assets/262b78a6-e16d-440e-91bb-c0ed3a95dd26" />

9. Save the configuration.
10. Validate user registration and sign-in functionality.
