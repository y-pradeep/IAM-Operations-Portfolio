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
2. Navigate to **Protection** → **Conditional Access**.
3. Click **New Policy**.
4. Enter a policy name.
5. Select target users or groups.
6. Select target cloud applications.
7. Configure conditions if required.
8. Under **Grant Controls**, select **Require Multi-Factor Authentication**.
9. Enable the policy.
10. Test policy behavior using pilot users.
