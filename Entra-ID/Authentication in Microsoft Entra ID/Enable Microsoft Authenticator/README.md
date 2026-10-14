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
2. Navigate to **Protection** → **Authentication Methods**.
3. Select **Microsoft Authenticator**.
4. Click **Enable**.
5. Assign users or groups who will use Microsoft Authenticator.
6. Enable **Push Notifications**.
7. Enable **Passwordless Authentication** if required.
8. Configure **Number Matching** settings.
9. Save the configuration.
10. Validate user registration and sign-in functionality.
