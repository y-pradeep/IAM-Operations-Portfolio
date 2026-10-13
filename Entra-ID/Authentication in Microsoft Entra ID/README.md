# Configure Self-Service Password Reset (SSPR) Authentication Methods in Microsoft Entra ID

## Objective

To configure the methods users can use to verify their identity when resetting passwords through Self-Service Password Reset.

## Business Requirement

SSPR allows eligible users to reset forgotten passwords without contacting IT support while maintaining identity verification requirements.

## Pre-requisites

- Access to the Microsoft Entra admin center.
- Appropriate permissions to manage password reset settings.
- Licensing appropriate to the organization's SSPR requirements.
- Target users or groups identified.
- Approved password reset and verification requirements.
- Required verification methods enabled and available to users.

## Steps of the Task

1. Navigate to **Microsoft Entra ID → Password reset**.
2. Open **Properties** and configure the users or groups allowed to use SSPR.
3. Select **Authentication methods**.
4. Configure permitted methods and the number of methods users must provide to reset passwords.
5. Save the configuration.
6. Review registration settings and configure registration requirements as appropriate.
7. Test with an eligible test account and verify that configured verification requirements are enforced.

