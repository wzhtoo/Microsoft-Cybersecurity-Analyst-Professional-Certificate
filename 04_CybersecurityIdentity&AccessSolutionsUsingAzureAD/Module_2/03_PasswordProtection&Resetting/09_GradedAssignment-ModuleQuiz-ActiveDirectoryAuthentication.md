# Module quiz: Active directory authentication

[Module quiz: Active directory authentication 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/assignment-submission/8wz1P/module-quiz-active-directory-authentication)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/assignment-submission/8wz1P/module-quiz-active-directory-authentication/attempt)

1.  Question 1
    Complete the following sentence. Single sign-on (SSO) in Azure AD allows users to sign in once to \***\*\_\_\_\*\*** multiple applications and enhances \***\*\_\_\_\*\*** efficacy.

- Authenticate, workflow
- Access, security
- Authorize, authentication

2. Question 2
   You would like to give your users the ability to access both on-premises and cloud-based resources using a single password. Which feature of Azure AD Connect would you implement to achieve this?

- Azure AD Application Proxy
- **Pass-through authentication**
  - Correct! Pass-through authentication is a feature of Azure AD Connect that allows users to authenticate online against their on-premises AD credentials.
- Active Directory Domain Controller (AD DC)

3. Question 3
   Complete the following sentence. Azure AD **\_\_\_** Synchronization ensures that passwords are stored in both an on-premises AD and Azure AD, and stay secret and synchronized.

- Credential
- **Hash**
  - Correct! Azure AD Hash Synchronization allows for authentication without sending sensitive data by sending hashes, which are series of characters that result from applying a mathematical formula to the password to change its representation.
- Change

4. Question 4
   To add another layer of security, you decide to implement multi-factor authentication (MFA) that is triggered when a user attempts to gain access to the company’s payroll management software. Which option best describes what MFA requires before granting this access?

- Biometric data
- **Two or more checks**
  - Correct! The M in MFA stands for Multi, and it is about providing additional verification in certain conditions.
- Authentication

5. Question 5
   What is a PIN when used in MFA?

- Something you are
- **Something you know**
  - Correct! A PIN is a character sequence that is known only to you.
- Something you have

6. Question 6
   To help detect and stop unauthorized login attempts, you want to implement an Azure feature that uses machine learning and data analytics to identify deviant behavior. This then triggers MFA upon the attempt or denies access outright. Which feature allows you to do this?

- Strong protection
- Conditional Access
- **Azure Identity Protection**
  - Correct! Azure Identity Protection is an advanced feature that can add extra security without the need for additional vigilance.

7. Question 7
   In order to enable users to get back into their accounts quickly after forgetting their passwords while also lightening the workload of the organization’s IT staff, which feature would you implement?

- **Self-service password reset (SSPR)**
  - Correct! SSPR is a feature that allows users to reset their password without IT support.
- Password Writeback
- AD Connect Cloud Sync

8. Question 8
   Which of the following situations can be configured in SSPR? Select all that apply.

- Password writeback
- **Password reset**
  - Correct! It is possible to change an existing password with SSPR.
- **Password unlock**
  - Correct! It is possible to change an existing password with SSPR.
- Password validation

9. Question 9
   You are configuring authentication for the point-of-sale devices at Sam’s Scoops. Because of the fast-paced working environment, employees would like to gain entry to these devices as quickly as possible. Which of the following forms of identification best meets this need?

- Password
- **Facial recognition**
  - Correct! A properly configured device that scans a face offers a very quick real-time method of verification.
- PIN

10. Question 10
    Which authentication method uses public-key cryptography to provide strong authentication?

- **FIDO authentication**
  - Correct! FIDO authentication is strong and reliable for security purposes and does not hugely impact a user’s workflow
- OATH hardware tokens
- SMS-based authentication
