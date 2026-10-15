# Configure Self-Service Password Reset (SSPR) Authentication Methods

## Objective
Configure authentication methods used during Self-Service Password Reset (SSPR).

## Business Requirement
Enable users to securely reset or unlock their accounts without helpdesk assistance, reducing operational overhead.

## Pre-Requisites
- Microsoft Entra ID tenant
- Microsoft Entra ID P1 or P2 license
- Global Administrator or Authentication Administrator role
- SSPR enabled for users

## Steps of the Task

1. Sign in to the Microsoft Entra Admin Center.
 <img width="1917" height="961" alt="MS Entra Admin Center" src="https://github.com/user-attachments/assets/72bd621b-7c94-45c9-86bd-ac8f11e7a3f2" />

2. Navigate to **Protection** → **Password Reset**.
 <img width="1903" height="816" alt="image" src="https://github.com/user-attachments/assets/cd895118-3a0a-4aa9-8537-650d46eeaeea" />

3. Select **Authentication Methods**.
4. Choose available methods such as Mobile Phone, Email, Microsoft Authenticator, and Security Questions.
 <img width="1912" height="865" alt="image" src="https://github.com/user-attachments/assets/b82bfa42-580e-4f86-bd50-719626815121" />

5. Configure the number of required methods.
 <img width="1917" height="948" alt="image" src="https://github.com/user-attachments/assets/f5d56128-eb45-41a6-b206-639d59467a52" />

6. Configure registration settings.
7. Enable SSPR for target users or groups.
 <img width="1910" height="948" alt="image" src="https://github.com/user-attachments/assets/dee8b909-7269-4662-b0ea-cdeb96c060f4" />

8. Save the configuration.
9. Perform password reset testing.
10. Review audit logs and reporting.
