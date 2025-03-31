# Module quiz: Active Directory access, protection, and governance management

[Module quiz: Active Directory access, protection, and governance management 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/assignment-submission/9TbIM/module-quiz-active-directory-access-protection-and-governance-management)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/assignment-submission/9TbIM/module-quiz-active-directory-access-protection-and-governance-management/attempt)

1.  Question 1
    After an audit revealed that certain employee accounts continued to have privileged access that was no longer needed, the administrator at Sam’s Scoops decided to implement role-based access control (RBAC). Which steps should be taken as part of this process? Select all that apply.

- Define what actions users are allowed to take.
- **Identify the roles that exist within an organization.**
  - Correct! Implementing RBAC involves identifying roles.
- Set the authentication method that applies to a role.
- **Assign permissions to roles.**
  - Correct! Implementing RBAC involves assigning permissions to roles.

2. Question 2
   An administrator wants to configure a Conditional Access policy that will prompt a user to go through multi-factor authentication (MFA) when certain signals are detected. Which of the following are common signals that Conditional Access policies can consider? Select all that apply.

- The length of time since the account password was last changed.
- **Named location information.**
  - Correct! Named location information is a common signal for Conditional Access policies.
- **Real-time sign-in risk detection.**
  - Correct! Real-time sign-in risk detection is a common signal for Conditional Access policies.
- Random application triggers.

3. Question 3
   You have assigned a User Administrator role, which grants permissions for managing resources that live in Azure AD. Which of the following role categories does this fall under?

- **Azure AD-specific roles**
  - Correct! The User Administrator role is limited to management of resources within Azure AD, but not other services.
- Service-specific roles
- Cross-service roles
- Privileged roles

4. Question 4
   What are the two types of role definitions in Azure AD?

- Basic roles and advanced roles.
- Fixed roles and flexible roles.
- **Built-in roles and custom roles.**
  - Correct! In Azure AD, there are two types of role definitions: built-in roles and custom roles.

5. Question 5
   What is the main policy engine within the Zero Trust model?

- Firewall
- Intrusion Detection System (IDS)
- Zero Trust Application Gateway
- **Conditional Access**
  - Correct! The Zero Trust model relies on Conditional Access to protect access to resources.

6. Question 6
   Imagine an organization that uses cloud-based applications and has many employees who work remotely. If the administrator wants to reduce the attack surface and increase visibility over user activity, which of the following security strategies should they employ?

- Network segmentation.
- **Treating identity as the primary security perimeter.**
  - Correct! Identity is widely viewed as the new security perimeter because it reduces the attack surface, increases visibility and control, and improves compliance.
- Firewall deployment.
- Cloud data encryption.

7. Question 7
   The administrator at an organization worries about potential security issues due to poorly managed access and wants to use Privileged Identity Management (PIM) to take a more secure approach. Which statement best describes how PIM can help to accomplish this?

- **PIM helps minimize the number of people with access to secure information, reducing the risk of unauthorized access and inadvertent impact on sensitive resources.**
  - Correct! PIM enables organizations to control and monitor access to important resources, minimizing the number of people with access to secure information.
- PIM is a feature that grants permanent privileged access to all users in Azure AD, increasing flexibility.
- PIM allows users to have unlimited access to resources in Azure AD, Azure, and other Microsoft Online services.
- PIM only supports time-bound access to Azure resources, excluding other Microsoft Online services.

8. Question 8
   What can be managed using Azure AD PIM?

- Only built-in Azure resource roles.
- Only custom roles in Azure AD.
- **Both built-in Azure resource roles and custom roles.**
  - Correct! Azure AD PIM can manage both built-in Azure resource roles and custom roles.
- Only Azure AD Premium P2 licenses.

9. Question 9
   What does Privileged Identity Management (PIM) help minimize?

- The number of applications and systems in Azure AD.
- **The number of people with access to secure information.**
  - Correct! Implementing PIM ensures that the fewest people have access to sensitive data, and those who do typically have it for a limited time.
- The number of authentication methods required for users.
- The number of permissions granted to regular users.

10. Question 10
    Which of the follow can you manage in Privileged Identity Management (PIM)? Select all that apply.

- Self-service password reset (SSPR)
- **PIM for Groups**
  - Correct! You can use PIM for Groups to set up just-in-time access to members of an Azure AD security group.
- Conditional Access
- **Azure AD roles**
  - Correct! You can use Azure AD roles to manage Azure AD and other Microsoft 365 online services.
