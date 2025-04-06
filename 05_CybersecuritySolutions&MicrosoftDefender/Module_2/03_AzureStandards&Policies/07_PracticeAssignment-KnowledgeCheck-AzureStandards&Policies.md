# Knowledge check: Azure Standards and policies

[Knowledge check: Azure Standards and policies 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/assignment-submission/OXYOZ/knowledge-check-azure-standards-and-policies)

# Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/assignment-submission/OXYOZ/knowledge-check-azure-standards-and-policies/attempt)

1.  Question 1
    How can you ensure that only cost-effective virtual machine SKU sizes are deployed?

- Periodically inspect the deployment to see which SKU sizes are used.
- **Create a policy in Azure Policy that specifies the allowed SKU sizes.**
  - That's correct! There's a built-in Azure policy to specify the allowed virtual machine SKU sizes. After the policy is enabled, it's applied whenever a virtual machine is created or resized.
- Create an Azure RBAC role that defines the allowed virtual machine SKU sizes.

2. Question 2
   Which option can you use to manage governance across multiple Azure subscriptions?

- Azure definitions
- **Management groups**
  - That's correct! The resources and subscriptions assigned to a management group automatically inherit the conditions applied to the management group.
- Resource groups
- Azure initiatives

3. Question 3
   You are a cloud architect responsible for optimizing costs and ensuring compliance with corporate standards in your organization's Azure environment. You have implemented Azure policies to enforce these standards. How does Azure policy evaluation help you achieve these goals?

- Azure policy evaluation is irrelevant to cost optimization and compliance with corporate standards.
- Azure policy evaluation primarily focuses on compliance with corporate standards and overlooks cost optimization.
- **Azure policy evaluation monitors cost optimization and ensures compliance with corporate standards.**
  - That's correct! Azure policy evaluation plays a crucial role in both cost optimization and compliance with corporate standards. By implementing Azure policies, organizations can enforce specific rules and guidelines to optimize resource usage and ensure adherence to compliance requirements.
- Azure policy evaluation only focuses on cost optimization and neglects compliance with corporate standards.

4. Question 4
   True or False: Within Azure policy, initiative definitions hold one or more policy definitions.

- **True**
  - That's correct! Initiative definitions hold policy definitions that can be applied to management groups, subscriptions, and resource groups.
- False

5. Question 5
   Audit, Deny, and Disabled are all examples of what within policy definitions?

- Categories
- **Effects**
  - That's correct! Effects are the actions taken within a policy definition.
- Artifacts
