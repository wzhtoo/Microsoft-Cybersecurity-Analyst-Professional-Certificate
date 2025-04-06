# Knowledge check: Azure Firewall protection

[Knowledge check: Azure Firewall protection 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/assignment-submission/q0PrQ/knowledge-check-azure-firewall-protection)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/assignment-submission/q0PrQ/knowledge-check-azure-firewall-protection/attempt)

1.  Question 1
    When working with Azure networks, what is used to connect virtual networks together to enable connectivity?

- **Peering**
  - That's correct! Peering is used to connect different virtual networks together, enabling connectivity.
- Subnets
- VNets
- NSGs

2. Question 2
   Where is the best place to host a firewall within Microsoft Azure when needing to protect a number of different resources, including internet and on-premise traffic?

- **Hub**
  - That's correct! Placing the Azure firewall services within a hub allows different resources to use the firewall from that central location. This includes different spokes, traffic from the internet and even on-premise networks.
- Spoke
- On-premise

3. Question 3
   What are the three different SKUs of the Azure Firewall? Select all that apply.

- **Basic**
  - That's correct! Azure Firewall Basic is intended for small and medium size businesses (SMB) to secure their Azure cloud environments.
- **Standard**
  - That's correct! Azure Firewall Standard provides the same features as the basic firewall but supports much higher throughputs and supports threat intelligence-based filtering.
- **Premium**
  - That's correct! Azure Firewall Premium provides advanced capabilities, and it’s recommended for customers looking to secure highly sensitive applications, such as payment processing.
- Essential

4. Question 4
   True or false: Azure Firewall is a fully stateful, centralized network firewall as-a-service, which provides network- and application-level protection across different subscriptions and virtual networks.

- **True**
  - That's correct! Azure Firewall is a cloud-native and intelligent network firewall security service that provides the ultimate threat protection for your cloud workloads running in Azure.
- False

5. Question 5
   What Azure Firewall rule is used to translate between public and private IP addresses?

- **NAT rules**
  - That's correct! Azure firewalls use network address translation (NAT) which translates between public and private IP addresses.
- Network rules
- Application rules

6. Question 6
   An organization wants to enhance the security of its cloud resources in Azure. Which of the following statements accurately describes how Azure Firewall can be utilized for this purpose?

- **Azure Firewall is a security service that prevents unauthorized access to virtual networks and filters outbound internet traffic.**
  - That’s correct! Azure Firewall is designed to secure virtual networks by preventing unauthorized access and filtering outbound internet traffic.
- Azure Firewall is a web application firewall that protects cloud resources from distributed denial-of-service (DDoS) attacks and SQL injection.
- Azure Firewall is a service that provides advanced threat protection by analyzing network traffic and applying access control policies.
- Azure Firewall is a monitoring tool that generates logs and alerts for potential security breaches in Azure cloud resources.
