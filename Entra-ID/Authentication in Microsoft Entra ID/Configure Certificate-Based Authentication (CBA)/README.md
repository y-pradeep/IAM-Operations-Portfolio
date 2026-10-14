# Configure Certificate-Based Authentication (CBA)

## Objective
Enable certificate-based authentication using digital certificates for secure user authentication.

## Business Requirement
Organizations with Public Key Infrastructure (PKI) require certificate-based authentication to enhance security and compliance.

## Pre-Requisites
- Microsoft Entra ID tenant
- Microsoft Entra ID P1 or P2 license
- Operational PKI infrastructure
- Root and Intermediate CA certificates
- Global Administrator role

## Steps of the Task

1. Sign in to the Microsoft Entra Admin Center.
2. Navigate to **Protection** → **Authentication Methods**.
3. Select **Certificate-Based Authentication**.
4. Enable the authentication method.
5. Upload trusted Root CA certificates.
6. Upload Intermediate CA certificates.
7. Configure certificate binding settings.
8. Assign target users or groups.
9. Save the configuration.
10. Validate certificate-based authentication.
