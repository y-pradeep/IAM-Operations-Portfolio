# Configure FIDO2 Security Keys

## Objective
Enable FIDO2 Security Key authentication to provide phishing-resistant passwordless authentication.

## Business Requirement
FIDO2 Security Keys enhance security by eliminating password dependency and reducing phishing risks.

## Pre-Requisites
- Microsoft Entra ID tenant
- Microsoft Entra ID P1 or P2 license
- Supported FIDO2 Security Keys
- Authentication Administrator role

## Steps of the Task

1. Sign in to the Microsoft Entra Admin Center.
2. Navigate to **Protection** → **Authentication Methods**.
3. Select **FIDO2 Security Key**.
4. Enable the authentication method.
5. Assign users or groups.
6. Enable self-service registration.
7. Configure key restrictions if applicable.
8. Save the configuration.
9. Instruct users to register their security keys.
10. Validate passwordless authentication using the registered key.
