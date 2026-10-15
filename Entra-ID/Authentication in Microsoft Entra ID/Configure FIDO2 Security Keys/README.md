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
   <img width="1917" height="961" alt="MS Entra Admin Center" src="https://github.com/user-attachments/assets/1636e19c-5f11-48ad-90c3-227b986d86fc" />

2. Navigate to **Protection** → **Authentication Methods**.
   <img width="1920" height="955" alt="Authentication methods" src="https://github.com/user-attachments/assets/33ef3dc9-96ce-4f29-be5d-667e462cd5b6" />

3. Select **FIDO2 Security Key**.
4. Enable the authentication method.
   <img width="1905" height="947" alt="image" src="https://github.com/user-attachments/assets/e03c2def-b502-4492-9078-5c0999760704" />

5. Assign users or groups.
   <img width="1908" height="950" alt="image" src="https://github.com/user-attachments/assets/e5786397-a6c5-456a-b120-d7c0b946abf8" />

6. Enable self-service registration.
7. Configure key restrictions if applicable.
    <img width="1908" height="940" alt="image" src="https://github.com/user-attachments/assets/8b1e9045-4929-4b6f-8792-98474cb873d9" />

8. Save the configuration.
9. Instruct users to register their security keys.
10. Validate passwordless authentication using the registered key.
