# Knowledge check: Just-in-time access and encryption

[Knowledge check: Just-in-time access and encryption 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/assignment-submission/WJYGY/knowledge-check-just-in-time-access-and-encryption)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/assignment-submission/WJYGY/knowledge-check-just-in-time-access-and-encryption/attempt)

1.  Question 1
    When a VM receives an access request, Just-in-time (JIT) needs Defender for Cloud to configure two things. What are they?

- **Azure Firewall**
  - That's correct! The Azure firewall will need an allow rule to allow traffic to pass by Defender for Cloud.
- NSG
  - That's correct! The NSG, or network security group, will need an allow rule to allow traffic to pass by defender for cloud.
- Subnet
- VNet

2. Question 2
   When creating the JIT policy you specify the port numbers and how long the port should be open but what else forms part of this policy?

- **The IP address or addresses**
  - That's correct! Specific IP addresses can be defined or a wide range of IPs, including any address can be defined.
- User or users
- NSG rules that need to be changed
- Azure Firewall rules that need to be changed

3. Question 3
   What two best practices should be followed when data is at rest within Micorosft Azure?

- **Apply disk encryption to safeguard data.**
  - Feedback: That's correct! Encrypting disks using Bitlocker or Linux dm-crypt will help safeguard data.
- **Encrypt disks before writing data to them**
  - That's correct! Encrypting disks before storing data reduces the risk of this data being stolen or compromised.
- Encrypt data using SSL and TLS.
- Encrypt data using a VPN

4. Question 4
   Azure Key Vault is used for key management to create and control encryption keys but what else can it manage? Choose all that apply.

- **Certificate management**
  - That's correct! Azure Key Vault lets you easily provision, manage, and deploy public and private Transport Layer Security/Secure Sockets Layer (TLS/SSL) certificates.
- **Secrets management**
  - That's correct! Azure Key Vault can be used to securely store and tightly control access to tokens, passwords, certificates, API keys, and other secrets.
- User management

5. Question 5
   It is recommended that virtual hard disks (VHDs) are encrypted to protect data at rest, but what key should be used as an additional security layer to protect keys and secrets?

- **KEK**
  - That's correct! A KEK, or key encryption key, should be used to encrypt secrets and keys within Azure Key Vault.
- CEK
- PMK

6. Question 6
   You are a system administrator working with Microsoft Azure. A user in your organization requires temporary access to a specific resource for a limited period. Which option best describes the concept of Just in Time Access in Microsoft Azure?

- **Just in Time Access is a feature that provides temporary and controlled access to resources for users in Microsoft Azure.**
  - That’s correct! Just in Time Access allows users to have temporary and controlled access to resources in Microsoft Azure.
- Just in Time Access is a feature that allows users to manually request access to resources in Microsoft Azure.
- Just in Time Access is a feature that grants permanent access to resources for users in Microsoft Azure.
- Just in Time Access is a feature that automatically revokes access to resources after a certain period of time in Microsoft Azure.
