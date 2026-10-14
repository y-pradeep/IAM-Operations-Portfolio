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
2. Navigate to **Protection** → **Password Reset**.
3. Select **Authentication Methods**.
4. Choose available methods such as Mobile Phone, Email, Microsoft Authenticator, and Security Questions.
5. Configure the number of required methods.
6. Configure registration settings.
7. Enable SSPR for target users or groups.
8. Save the configuration.
9. Perform password reset testing.
10. Review audit logs and reporting.
