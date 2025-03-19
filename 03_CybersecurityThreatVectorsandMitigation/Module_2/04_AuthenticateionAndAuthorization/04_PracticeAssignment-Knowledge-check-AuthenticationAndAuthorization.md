# Knowledge check: Authentication and authorization

[Knowledge check: Authentication and authorization 🔗](https://www.coursera.org/learn/cybersecurity-threat-vectors-and-mitigation/assignment-submission/pFKPQ/knowledge-check-authentication-and-authorization)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-threat-vectors-and-mitigation/assignment-submission/pFKPQ/knowledge-check-authentication-and-authorization/attempt)

1.  Question 1
    Which of the following statements best describes the difference between authentication and authorization?

- Authentication is granting access based on user permissions, while authorization is verifying the identity of a user or system.
- Authentication and authorization are the same concept and are used interchangeably.
- **Authentication is verifying the identity of a user or system, while authorization is granting access based on user permissions.**
  - That’s correct. Authentication is the process of verifying the identity of a user or system, while authorization is the process of granting or denying access to resources, data, or systems based on the authenticated user's role or level of acces
- Authentication is a type of authorization, and authorization is a type of authentication.

2. Question 2
   Which authentication system uses digital certificates to verify the identity of a user, device, or application?

- LDAP
- Kerberos
- **Certificate-based authentication**
  - That’s correct. Certificate-based authentication uses digital certificates issued by a centralized certificate authority (CA) to verify the identity of a user, device, or application. LDAP, RADIUS, and Kerberos are other centralized authentication systems but do not primarily rely on digital certificates.
- RADIUS

3. Question 3
   Imagine you're the head of IT at a growing tech company. Your company has been experiencing security breaches due to weak user passwords. You have been tasked with implementing multi-factor authentication to enhance security.
   When considering your options, which of the following is a common factor used in multi-factor authentication? Select all that apply.

- **Something you know**
  - That’s correct. This factor is used in multi-factor authentication. It refers to information only the user should know, such as a password or PIN.
- Something you can guess
- **Something you are**
  - That’s correct. This factor is used in multi-factor authentication. It refers to the location of the user, which can be determined by GPS or other location-tracking technologies
- **Something you have**
  - That’s correct. This factor is used in multi-factor authentication. It refers to a physical object that the user possesses, such as a smartphone or a security token

4. Question 4
   In the context of password storage, what is the purpose of a salt?

- To verify the password during the login process.
- To encrypt the password.
- To make the password hashing process faster.
- **To ensure that the same password results in different hashes for different users.**
  - That’s correct. A salt is a random value generated and combined with the password before hashing. It ensures that even if two users have the same password, their hashes will be different, increasing the security of stored passwords.

5. Question 5
   You're working as the IT manager for a rapidly growing tech startup. Your company is adding new internal software and tools constantly. Your employees struggle to remember their various login credentials and the IT department is flooded with password reset requests.
   Which of the following benefits of a centralized authentication and authorization system could be a solution to your problem?

- It makes passwords more secure.
- It allows users to have multiple sets of credentials for different systems.
- **It simplifies the authentication process for users.**
  - That’s correct. Centralized authentication and authorization systems simplify the authentication process for users by allowing them to use a single set of credentials to access multiple systems and resources.
- It increases the complexity of the system.
