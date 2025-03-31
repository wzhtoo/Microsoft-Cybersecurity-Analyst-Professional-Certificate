# Knowledge check: Password protection and resetting

[Knowledge check: Password protection and resetting 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/assignment-submission/LvbZq/knowledge-check-password-protection-and-resetting)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/assignment-submission/LvbZq/knowledge-check-password-protection-and-resetting/attempt)

1.  Question 1

Your organization has implemented a hybrid Active Directory environment and wants to ensure that when a user updates their account password within the cloud-based directory, the change is also reflected in the on-premises directory. Which tool should be used to do this?

- **Azure AD Connect Cloud Sync**
  - Correct! Azure AD Connect Cloud Sync is used to configure, manage and sync Active Directories. It performs password writeback to ensure that password changes are aligned between on-cloud and on-premises active directories.
- Azure Active Directory Domain Services
- Azure Active Directory Risk Protection

2. Question 2

Which of the following scenarios outline when a Global Administrator is restricted from resetting a password?

- When SSPR has not been configured.
- When SSPR has been configured, but the Global Administrator has not been included in the authorized list.
- **A Global Administrator is never restricted.**
  - Correct! By default, a global administrator has SSPR enabled regardless of the configuration. This is to avoid inadvertently locking an organization out of the system.

1. Question 3

Complete the following sentence. Despite SSPR being enabled, the user still can’t access password reset because **\*\***\_**\*\***.

- the user has entered a password with insufficient strength.
- of Identity Protection.
- **the individual is excluded from SSPR.**
  - Correct! The system can include or exclude some individuals from services or features like SSPR.

4. Question 4

True or False: A secret question can be used as a form of user authentication when accessing a system.

- True
- **False**
  - Correct! A secret question is not generally used as a means of identification due to the danger posed by social phishing.

1. Question 5

What is Microsoft’s minimum recommended password length?

- 6 characters
- **8 characters**
  - Correct! Microsoft recommended that passwords be between 8 and 16 characters in length.
- 10 characters
