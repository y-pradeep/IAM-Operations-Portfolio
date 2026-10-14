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
2. Navigate to **Protection** → **Authentication Methods**.
3. Select **Temporary Access Pass**.
4. Enable the policy.
5. Assign target users or groups.
6. Configure pass lifetime.
7. Configure pass length and one-time use settings.
8. Save the configuration.
9. Navigate to **Users** and select the target user.
10. Generate and securely share the Temporary Access Pass.
