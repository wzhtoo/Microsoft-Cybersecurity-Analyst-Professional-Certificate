# Knowledge check: Roles and role-based access

[Knowledge check: Roles and role-based access 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/assignment-submission/CPTrq/knowledge-check-roles-and-role-based-access)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/assignment-submission/CPTrq/knowledge-check-roles-and-role-based-access/attempt)

1.  Question 1
    Which of the following statements are true about role-based access control (RBAC) in Microsoft Entra ID? Select all that apply.

- RBAC uses machine learning to evaluate user roles and set their access accordingly.
- **RBAC allows the head administrator to grant granular permissions to other administrators while adhering to the principle of least privilege.**
  - Correct! RBAC is a means of defining permissions for roles, which can then be assigned as needed to administrators, users, and groups. These can also be unassigned when no longer required.
- RBAC allows administrators to assign roles to roles that determine access to resources, without the need for additional authentication.
- **Microsoft Entra ID features built-in roles with pre-defined permissions, and custom roles that allow you to set permissions manually.**
  - Correct! While built-in roles cover many common access needs, custom roles are a good option for the more specific needs of an organization.

2. Question 2
   As an administrator, you would like to create a role called 'Shift Leads' and give it the permissions to access an employee scheduling application. This role would then be assigned to all Shift Leads working for Sam’s Scoops, granting them access without the need for further configuration. Which feature would enable you to do this?

- **Azure role-based access control (RBAC).**
  - Correct! Azure RBAC enables you to manage access control to Azure resources based on roles and permissions. It allows you to assign roles to users, groups, or service principals to control their level of access.
- Microsoft Entra Conditional Access
- Single sign-on (SSO) for cloud applications.
- Azure AD B2C for customer identity and access management.

3. Question 3
   What is the purpose of assigning custom roles in Azure RBAC?

- **To define granular permissions tailored to unique business needs.**
  - Correct! Assigning custom roles in Azure RBAC allows organizations to define granular permissions that are specifically tailored to their unique business needs. It provides the flexibility to assign precise access levels to users based on their responsibilities.
- To automate resource provisioning in Azure
- To enforce data encryption for Azure virtual machines
- To monitor network traffic patterns in real-time

4. Question 4
   At which scopes can role assignments be made in Azure RBAC?

- **Subscription level, resource group level, and individual resource level.**
  - That's correct! Role assignments in Azure RBAC can be made at the subscription level, resource group level, and individual resource level. This allows organizations to control access to Azure resources with different levels of granularity.
- Virtual network level, storage account level, and database level.
- Region level, availability set level, and virtual machine scale set level.
- Management group level, Microsft Entra ID level, and service principal level.

5. Question 5
   Which of the following statements best describes the role of the Global Administrator in Azure RBAC?

- **The Global Administrator has full access and control over all Microsoft 365 resources and services.**
  - Correct! The Global Administrator in Azure RBAC has the highest level of access and control in Microsoft 365. They have full privileges to manage and administer all Microsoft 365 resources and services within the organization.
- The Global Administrator manages user accounts and access to Azure resources.
- The Global Administrator is responsible for monitoring and managing security settings.
- The Global Administrator is responsible for managing virtual networks and network security groups.
