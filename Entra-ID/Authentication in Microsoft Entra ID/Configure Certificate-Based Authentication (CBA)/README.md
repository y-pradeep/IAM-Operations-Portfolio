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
 <img width="1917" height="961" alt="MS Entra Admin Center" src="https://github.com/user-attachments/assets/37b93ea9-f45e-4763-b3bb-cc58571b54ef" />

2. Navigate to **Protection** → **Authentication Methods**.
 <img width="1920" height="955" alt="Authentication methods" src="https://github.com/user-attachments/assets/30be2164-ebe5-43eb-8178-852bfe9c553c" />

3. Select **Certificate-Based Authentication**.
4. Enable the authentication method.
 <img width="1899" height="940" alt="image" src="https://github.com/user-attachments/assets/14ebaf34-fdcc-400c-96ce-a84ff89a7e62" />

5. Upload trusted Root CA certificates.
6. Upload Intermediate CA certificates.
7. Configure certificate binding settings.
 <img width="1905" height="947" alt="image" src="https://github.com/user-attachments/assets/a2b07978-3fd6-43f0-a894-c3c54f7d6b34" />

8. Assign target users or groups.
 <img width="1918" height="950" alt="image" src="https://github.com/user-attachments/assets/f0138b0d-8214-4ab7-9e40-9d677b7a8b37" />

9. Save the configuration.
10. Validate certificate-based authentication.
