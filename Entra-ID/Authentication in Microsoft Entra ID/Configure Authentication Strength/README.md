# Configure Authentication Strength

## Objective
Define authentication strength requirements for accessing applications and resources.

## Business Requirement
Authentication Strength allows organizations to enforce stronger authentication methods for sensitive resources.

## Pre-Requisites
- Microsoft Entra ID P1 or P2 license
- Conditional Access policies
- Security Administrator or Conditional Access Administrator role

## Steps of the Task

1. Sign in to the Microsoft Entra Admin Center.
   
 <img width="1917" height="961" alt="MS Entra Admin Center" src="https://github.com/user-attachments/assets/dab92606-b6e1-47a6-b69c-df71497a0e20" />

2. Navigate to **Entra ID** → **Authentication Strengths**.
 
 <img width="1913" height="957" alt="image" src="https://github.com/user-attachments/assets/bd353941-e1fc-49a4-832d-d4fe44453573" />

3. Review built-in authentication strengths.
4. Select an existing strength or create a custom strength.
5. Choose allowed authentication methods.
 
 <img width="1919" height="952" alt="image" src="https://github.com/user-attachments/assets/23309fc1-f9d9-4ab3-998b-b3d3971f72e5" />

6. Save the authentication strength.
7. Navigate to **Conditional Access**.
8. Create or modify a policy.
9. Assign the authentication strength to the policy.
 
 <img width="1880" height="945" alt="image" src="https://github.com/user-attachments/assets/57beab3e-0686-4211-a031-f513e0a64137" />

10. Validate user access and authentication requirements.
