# Self-review: Policy implementation

[Self-review: Policy implementation 🔗](https://www.coursera.org/learn/advanced-cybersecurity-concepts-and-capstone-project/assignment-submission/jiYB3/self-review-policy-implementation)

## Assingment

[Assingment 🔗](https://www.coursera.org/learn/advanced-cybersecurity-concepts-and-capstone-project/assignment-submission/jiYB3/self-review-policy-implementation/view-feedback)

In Stage 5 of your project for VIP Events, you've taken on the critical task of developing and specifying Azure Policy configurations, with a focus on user authentication and network configuration for web applications. Your work involved crafting recommendations to secure Azure resources effectively and designing network guidelines tailored for web applications. These self-review questions will help you reflect on your approach.

1.  Question 1
    What is the most effective way to enforce multi-factor authentication (MFA) for users in the user authentication policy? Select all that apply.

Implement MFA for all users and allow them to opt out if necessary.

- **Enable MFA for critical user accounts and provide alternative authentication methods for other users.**
  - That's correct! Enabling MFA for critical user accounts and providing alternative authentication methods for other users strikes a balance between security and usability.
- **Enforce MFA for specific user roles based on their access privileges.**
  - That's correct! Enforcing MFA for specific user roles provides a more granular approach to security by focusing on users with elevated privileges.
- Require MFA for all users regardless of their role.

2. Question 2
   What are the best ways to restrict access to specific virtual networks (VNETs) when setting up a network configuration policy for web applications? Select all that apply.

- Block all traffic from the internet and allow connections only from authorized VNETs.
- **Utilize role-based access control (RBAC) to specify which users or groups can access the web applications from different VNETs.**
  - That's correct! Utilizing RBAC allows for fine-grained control over access permissions based on user roles or groups
- Implement a MAC address filtering system, allowing access only to devices with specific hardware addresses.
- **Employ a geolocation-based access policy, permitting connections only from specified locations.**
  - That's correct! Employing a geolocation-based access policy can enhance security by restricting access to web applications based on the geographical location of users.
- **Implement a whitelist approach, explicitly allowing access from predefined VNETs.**
  - That's correct! A whitelist approach provides a precise and controlled mechanism for restricting access to authorized VNETs.

3. Question 3
   When designing and implementing security policies for VIP Events, which of the following approaches is the most effective in mitigating insider threats? Select all that apply.

- **Establish clear reporting procedures for suspicious activity and empower employees to raise concerns without fear of retaliation.**

  - That's correct! Clear reporting procedures encourage employees to report suspicious activity, fostering a proactive approach to mitigating insider threats.

- **Conduct regular security awareness training for all employees, including event staff.**

  - That's correct! Regular security awareness training is essential for educating employees on security best practices and mitigating insider threats.

- Deploy perimeter defenses such as firewalls and intrusion prevention systems at the Internet-facing network to block threats from infiltrating the network.

- **Implement least privilege principles, granting users only the access they need to perform their tasks.**
  - That's correct! Implementing least privilege principles ensures that users have only the necessary access, reducing the risk of insider threats.
- **Implement continuous monitoring of user activity and utilize anomaly detection algorithms to identify potential insider threats.**
  - That's correct! Continuous monitoring and anomaly detection effectively identify and address potential insider threats.
- Implement a honeypot system within the network, intentionally exposing false vulnerabilities to divert insider threats.
