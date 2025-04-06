# Knowledge check: Virtual security solutions

[Knowledge check: Virtual security solutions 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/assignment-submission/ViNg9/knowledge-check-virtual-security-solutions)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/assignment-submission/ViNg9/knowledge-check-virtual-security-solutions/attempt)

1.  Question 1
    What measurement does this graphic from Microsoft Defender for Cloud provide?

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/2e4fceae-db42-4413-aa00-9f482850c565image1.png?expiry=1743724800000&hmac=JocKvw3O7Z6cASa8Kya_wz6Hca1L9oiowUGIaZPphx4">

- **Secure score**
  - That's correct! The secure score is a measurement used by Defender for Cloud to represent the risk level of your Azure setup. The higher the score the lower the risk.
- Compliance score
- Posture score
- Inventory score

2. Question 2
   Defender for Cloud will provide recommendations for an Azure environment and how to remedy certain threats. What is displayed in this image?

<img src="https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/2e4fceae-db42-4413-aa00-9f482850c565image3.png?expiry=1743724800000&hmac=j8umAIvBFlv81OYdzKc-ZoicEWMjWigr7TnVrC_m_5M">

- **Attack path**
  - That's correct! The attack path shows threats that can be used against Azure resources in the current subscription.
- Cloud security explorer
- Inventory

3. Question 3
   What port is used to connect to Azure Bastion via the Azure portal?

- 80
- 3389
- **443**
  - That's correct! Azure Bastion uses port number 443 HTTPS with an HTML5 supported browser to provide secure access to the Azure Bastion service.
- 22

4. Question 4
   By using Azure Bastion what protocols do you keep from being exposed on the public internet? Select all that apply.

- **RDP**
  - That's correct! RDP is only used between the Azure Bastion service and the remote VM, thus not exposing the protocols to the public internet.
- **SSH**
  - That's correct! SSH is only used between the Azure Bastion service and the remote VM, thus not exposing the protocols to the public internet.
- HTTPS
- HTTP

5. Question 5
   True or false: Azure Bastion cannot work alongside JIT.

- **False**
  - That's correct! Using JIT and Azure Bastion together is a great way of protecting virtual machines within Azure.
- True

6. Question 6
   John is a cloud administrator responsible for managing remote access to Azure virtual machines (VMs). He wants to enhance the security of remote connections by using Azure Bastion. Which statement accurately describes Azure Bastion?

- Azure Bastion is a virtual network (VNet) resource that allows you to establish private network connections to Azure services over a private network.

- Azure Bastion is a cloud-based, load-balancing service that distributes incoming network traffic across multiple Azure VMs for high availability and fault tolerance.

- **Azure Bastion is a fully managed Platform as a Service (PaaS) solution that provides remote desktop protocol (RDP) and secure shell (SSH) access to Azure VMs without requiring a public IP address on the VM.**
  - That's correct! It is a fully managed PaaS solution specifically designed for securely accessing Azure VMs over the internet. It eliminates the need for exposing VMs directly to the public internet by providing RDP and SSH access through a secure HTML5-based web client, without requiring a public IP address on the VM. This enhances the security posture of remote connections.
- Azure Bastion is an Azure Active Directory (Azure AD) service that provides centralized identity and access management for Azure resources.
