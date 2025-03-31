# Self-review: Conditional policy

[Self-review: Conditional policy 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/assignment-submission/567QM/self-review-conditional-policy)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/assignment-submission/567QM/self-review-conditional-policy/attempt)

Organizations utilizing Conditional Access and the location condition, can enhance their security posture by preventing unauthorized access from specific network locations, bolstering their overall cloud app security.

In the exercise, you configured Conditional Access to block access by location in Azure. With the Location condition in Conditional Access, you now control access to the cloud apps based on the network location of a user. Answer the following questions to make sure that you understood and executed the tasks correctly.

1. Question 1
   What is the purpose of creating a Conditional Access policy to block access from unexpected locations at Sam’s Scoops?

- To restrict access to only known locations.
- **To reduce threats by creating extra steps for unusual activity.**
  - Correct. Signing in from a new or unknown location could be a potential signal that an identity has been compromised and hence requires an additional authorization step.
- Ensuring employees can only log on to a system from a workstation.

2. Question 2
   To configure Conditional Access, which of the following roles is appropriate?

- **Conditional Access Administrator**
  - Great work! By giving your policy a name that follows a meaningful standard, it will be easier for you to review and update the policy when necessary.
- User Administrator
- Helpdesk Administrator

3. Question 3
   Did you create your policy using Report-only mode initially?

- **Yes**
  - Well done! After confirming your settings using report-only mode, you can safely move the Enable policy toggle from Report-only to On
- No
