# Module quiz: Cryptography

[Module quiz: Cryptography 🔗](https://www.coursera.org/learn/cybersecurity-threat-vectors-and-mitigation/assignment-submission/L9zhO/module-quiz-cryptography)

## Assignments

[Assignments 🔗](https://www.coursera.org/learn/cybersecurity-threat-vectors-and-mitigation/assignment-submission/L9zhO/module-quiz-cryptography/attempt)

1.  Question 1
    Sam wants to securely communicate with a new supplier, but they haven't agreed on a shared key beforehand. Which type of encryption should they use?

- Caesar Cipher
- **Asymmetric encryption**
  - That's correct. Asymmetric encryption, which uses a pair of public and private keys, is often used when two parties need to communicate securely but haven't agreed on a shared key beforehand.
- Symmetric encryption

2. Question 2
   Sam wants to ensure that the online transactions made by customers on the business website are secure. Which encryption protocol should Sam use to secure communication between the web server and the client's browser?

- Advanced Encryption Standard (AES)
- **SSL/TLS**
  - That's correct. SSL/TLS (Secure Sockets Layer/Transport Layer Security) is used to secure communication between web servers and clients. It is the standard protocol for securing online transactions, and ensures that all data exchanged between the web server and client's browser is encrypted
- RSA encryption

3. Question 3
   Which encryption tool uses a combination of symmetric and asymmetric encryption to secure email communication and can also be used to encrypt files and folders?

- **PGP (Pretty Good Privacy)**
  - That's correct! PGP uses a combination of symmetric and asymmetric encryption to protect email messages and can also be used to encrypt files and folders.
- Bitlocker
- VPN

4. Question 4
   The RSA algorithm is based on the mathematical properties of even numbers.

- True
- **False**
  - That's correct. The RSA algorithm is actually based on the mathematical properties of prime numbers, not even numbers.

5. Question 5
   Which hashing algorithm is considered highly secure against collision attacks and is widely adopted for applications that require high levels of security?

- Salting
- MD5
- **SHA-256**
  - That's correct. SHA-256, part of the SHA-2 family, is highly secure against collision attacks and is widely used in applications requiring strong security, such as digital signatures, password hashing, and blockchain technology.

6. Question 6
   Digital signatures are the same as digital certificates, and they are used for encrypting communication.

- True
- **False**
  - That's correct. Digital signing is a process which involves creating a unique digital fingerprint or hash of the document and encrypting it using the sender's private key to create a digital signature.

7. Question 7
   Which of the following statements correctly describes the role of Certificate Authorities (CAs) in the context of digital certificates?

- Certificate Authorities (CAs) are databases that store sensitive information for websites and services.
- **Certificate Authorities (CAs) are trusted organizations that validate and issue digital certificates, ensuring the authenticity of the certificate holder's identity.**
  - That's correct. CAs play a crucial role in the internet's trust system by validating the identities of entities and issuing digital certificates with their digital signatures, which guarantees that the certificate holder is genuine.
- Certificate Authorities (CAs) are responsible for encrypting data transmitted over the internet.

8. Question 8
   What is one of the key benefits of using signed URLs?

- **Increased security by requiring a valid signature to access protected resources.**
  - That's correct. By requiring a valid signature, signed URLs help prevent unauthorized access to protected resources, making it particularly useful for sensitive data or confidential documents.
- Allowing unlimited access to the resources for all users.
- Sharing the secret key with the end user for transparency.

9. Question 9
   What is the primary difference between authentication and authorization in the context of access control?

- **Authentication is verifying the identity of a user, while authorization determines what actions or resources an authenticated user can access.**
  - That's correct. Authentication is the process of verifying the identity of a user, ensuring they are who they claim to be. Once authenticated, authorization comes into play by defining what actions or resources the user is allowed to access based on their role or permissions.
- Authentication allows users to perform actions within a system, while authorization verifies the identity of users.
- Authentication and authorization are synonymous and have no difference.

10. Question 10
    Acme Corporation is looking for an authentication and authorization protocol to allow their users to log in once and gain access to multiple systems, applications, or services without having to log in again. Which protocol should Acme Corporation consider using?

- OpenID Connect
- **SAML (Security Assertion Markup Language)**
  - That's correct. SAML is a standard for exchanging authentication and authorization data between parties and is often used to implement Single Sign-On (SSO).
- OAuth
