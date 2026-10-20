# Configure Conditional Access MFA Requirements

## Objective
Enforce Multi-Factor Authentication (MFA) using Conditional Access policies.

## Business Requirement
Organizations require MFA enforcement to protect identities and secure access to cloud applications.

## Pre-Requisites
- Microsoft Entra ID P1 or P2 license
- Conditional Access Administrator role
- Defined user and application scope

## Steps of the Task

1. Sign in to the Microsoft Entra Admin Center.
<img width="1917" height="961" alt="MS Entra Admin Center" src="https://github.com/user-attachments/assets/4f1a93ad-d570-4a20-9e63-bf0bff5ee391" />

2. Navigate to **Entra ID** → **Conditional Access**.
 <img width="1917" height="951" alt="image" src="https://github.com/user-attachments/assets/5c032348-28bd-468c-b856-3566cfd5abd4" />

3. Click **New Policy**.
 <img width="1914" height="141" alt="image" src="https://github.com/user-attachments/assets/45711060-7e07-4cd7-b705-65038406a850" />

4. Enter a policy name.
 <img width="1917" height="289" alt="image" src="https://github.com/user-attachments/assets/caae0c3e-2312-4128-b80a-a0dc01de0ab5" />

5. Select target users or groups.
 <img width="1914" height="949" alt="image" src="https://github.com/user-attachments/assets/f27c188e-d91a-4e05-969d-113bf814341b" />

6 Select target cloud applications.
 <img width="1905" height="850" alt="image" src="https://github.com/user-attachments/assets/1aad1918-bbd5-4567-8b62-dadd80f4e940" />

7. Configure conditions if required.

8. Under **Grant Controls**, select **Require Multi-Factor Authentication**.
 <img width="1917" height="952" alt="image" src="https://github.com/user-attachments/assets/ba81eccd-fde4-4564-94a9-6a747ef4ab01" />

9. Enable the policy.
 <img width="1917" height="945" alt="image" src="https://github.com/user-attachments/assets/c2d2abae-5c6e-4527-a553-aecbc2aafdd6" />

10. Test policy behavior using pilot users.
