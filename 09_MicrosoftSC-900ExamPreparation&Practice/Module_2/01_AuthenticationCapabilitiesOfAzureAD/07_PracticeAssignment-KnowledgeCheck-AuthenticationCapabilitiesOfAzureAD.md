# Knowledge check: Authentication capabilities of Azure AD

[Knowledge check: Authentication capabilities of Azure AD 🔗](https://www.coursera.org/learn/microsoft-sc-900-exam-preparation-and-practice/assignment-submission/0eD1Y/knowledge-check-authentication-capabilities-of-azure-ad)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/microsoft-sc-900-exam-preparation-and-practice/assignment-submission/0eD1Y/knowledge-check-authentication-capabilities-of-azure-ad/attempt)

1.  Question 1
    Within your organization, Azure AD Identity Protection raised an alert after some unusual log-in attempts were made using an employee’s username with different passwords.

In this scenario, which of the following would provide the strongest protection?

- Introduce a banned password list.
- Create a custom list, removing common company-related passwords.
- **Implement multi-factor authentication (MFA).**
  - That’s correct! Multi-factor authentication has proven to be 90% more secure for an organization.

2. Question 2
   You’re a recruit at a company, and you want to impress by improving the firm’s security. You have flagged several employees whose security hygiene is questionable. So, you navigate to the authentication methodsin their user profiles to add additional authentication methods.

Which of the following is found under their authentication contact info? Select all that apply.

- **Email**
  - That’s correct! An employee’s email is found under their authentication contact info.
- **Phone**
  - That’s correct! An employee’s listed phone is found there.
- Address
- Fingerprint scan

3. Question 3
   Having added an additional authentication method to a user on Azure AD from their user profiles, you trigger a multi-factor authentication (MFA) request based on a conditional access policy configured to their location. Which authentication methods found in a user's authentication contact info would not be applicable to MFA?

- Alternative phone
- **Email**
  - That’s correct! An employee’s email cannot be used as the second factor in MFA.
- Phone

4. Question 4
   True or False: Azure does not use a security question to confirm anyone’s identity.

- True
- **False**
  - Azure AD does allow security questions as a part of its self-service password reset (SSPR) process. While it’s not the primary or most commonly used method for confirming identity (especially in the case of MFA), security questions can be used to verify identity if configured by the organization.

So, Azure AD can use security questions in certain scenarios, like password resets.

5. Question 5
   What is the most common trigger for MFA?

- With a conditional access policy for suspicious log-ins.
- **Sign-in.**
  - That’s correct! MFA is configured to be always triggered when a user attempts to sign in.
- Changing your password.
