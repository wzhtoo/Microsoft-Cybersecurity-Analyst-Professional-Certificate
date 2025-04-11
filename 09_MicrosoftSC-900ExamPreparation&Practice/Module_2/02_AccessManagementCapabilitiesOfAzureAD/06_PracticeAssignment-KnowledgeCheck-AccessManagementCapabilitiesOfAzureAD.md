# Knowledge check: Access management capabilities of Azure AD

[Knowledge check: Access management capabilities of Azure AD 🔗](https://www.coursera.org/learn/microsoft-sc-900-exam-preparation-and-practice/assignment-submission/Imy9K/knowledge-check-access-management-capabilities-of-azure-ad)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/microsoft-sc-900-exam-preparation-and-practice/assignment-submission/Imy9K/knowledge-check-access-management-capabilities-of-azure-ad/attempt)

1.  Question 1
    At your company, you notice that the security posture is not as good as it should be. After authentication is established, there are no subsequent checks to ensure that the authentication granted was toward an appropriate identity. What should you do?

- Implement a blanket MFA rule for all company users.
- Prevent authentication from any sign-ins in the blocked countries list.
- **Establish company policies and implement them.**
  - That’s correct! A conditional access policy brings signals together, to make decisions, and enforce organizational policies. Conditional access is based on company policies and monitors identities after being granted access.

2. Question 2
   A set of built-in rules that outlines what an identity can do is known as \_\_\_\_.

- **A templated role**
  - That’s correct! A templated role is a set of predefined permissions an entity can make. Microsoft has preconfigured templated roles that reflect typical tasks line of business found in many companies regardless of the industry.
- Highest privilege wins
- A templated conditional access policy line of business

3. Question 3
   Sign-in risk is one of the templated Conditional Access policies an organization can create. Which of the following is a sign-on risk?

- Sign-in from a device not shown to be owned by the user
- New users to your organization
- **The likelihood that the owner of an identity does not initiate the authentication request.**
  - That’s correct! It is a detected signal, indicating that the authentication may not be legitimate

4. Question 4
   True or False: When subscribed to the free license it is possible to configure role scope.

- True
- **False**
  - That’s correct! You can not configure scope on the free license, configuring scope requires a P2 license.

5. Question 5
   Which of the following is a security access policy enforced by Azure?

- **Least privilege**
  - That’s correct! The information security principle of least privilege stresses the fact that users and applications should be granted access only to the data and operations they require to perform their jobs. Only provide access to as much as a person needs when they need it.
- Geolocation tracking
- Highest privilege wins
