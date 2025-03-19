# Knowledge check: Digital signing and certificates

[Knowledge check: Digital signing and certificates 🔗](https://www.coursera.org/learn/cybersecurity-threat-vectors-and-mitigation/assignment-submission/yCHR0/knowledge-check-digital-signing-and-certificates)

## Assignments

[Assignments 🔗](https://www.coursera.org/learn/cybersecurity-threat-vectors-and-mitigation/assignment-submission/yCHR0/knowledge-check-digital-signing-and-certificates/attempt)

1.  Question 1
    What is the primary purpose of digital signatures?

- Compressing files.
- Encrypting messages.
- **Authenticating the sender and ensuring message integrity.**
  - That’s correct. Digital signatures authenticate the sender and ensure message integrity, verifying the sender's identity and confirming that the message has not been tampered with during transmission.
- Increasing message readability.

2. Question 2
   In the context of digital certificates, what is the main function of a public key?

- **Verifying digital signatures.**
  - That’s correct. The primary function of a public key in the context of digital certificates is to verify digital signatures, ensuring the sender's authenticity and confirming that the message has not been altered during transmission.
- Decrypting messages.
- Encrypting messages.
- Generating digital signatures.

3. Question 3
   What is the primary purpose of a Certificate Authority (CA) in the context of digital certificates?

- **To issue and manage digital certificates.**
  - That’s correct. The primary purpose of a Certificate Authority (CA) is to issue and manage digital certificates, acting as a trusted third party that verifies the identities of individuals, organizations, and devices.
- To store digital certificates.
- To generate private keys.
- To validate digital signatures.

4. Question 4
   Which of the following algorithms are typically used for generating digital signatures? Select all that apply.

- **RSA**
  - That’s correct. RSA is a widely used public key cryptosystem for digital signatures and encryption.
- Blowfish
- **ECDSA**
  - That’s correct. ECDSA is an elliptic curve-based digital signature algorithm.
- AES

5. Question 5
   Imagine that Riley prepares to send a confidential document to Morgan over a secure digital network. She wants to assure Morgan that the document is genuinely from her and hasn't been tampered with during transmission.
   In the digital signature scheme they're using, what does Riley use to create the digital signature attached to the document?

- **Riley's private key**
  - That’s correct. Riley uses her private key to create the digital signature. This ensures that only Riley, as the owner of the private key, can create a valid signature. Morgan then verifies the signature using Riley's public key.
- Morgan's public key.
- Riley's public key.
- Morgan's private key.
