# Knowledge check: Azure VPN

[Knowledge check: Azure VPN 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/assignment-submission/6xj3t/knowledge-check-azure-vpn)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/assignment-submission/6xj3t/knowledge-check-azure-vpn/attempt)

1.  Question 1
    You are a network administrator for a company that has recently adopted cloud services in Microsoft Azure. The company's remote workforce needs secure access to Azure resources from their individual client computers. You are tasked with setting up the appropriate VPN connection type to meet this requirement.

Which VPN connection type should you configure to allow remote workers to securely access Azure resources from their individual client computers?

- ExpressRoute VPN
- Site-to-Site VPN
- **Point-to-Site VPN**
  - That’s correct. Point-to-Site VPN allows remote workers to securely connect to the Azure virtual network from their individual client computers.
- VNet-to-VNet VPN

2. Question 2
   Which of the following statements accurately describes the benefits of Azure VPN in terms of global reach and scalability?

- Azure VPN ensures scalability by facilitating secure connectivity for managing supply chains and collaborating with logistics partners.
- **Azure VPN offers global reach with availability in over 100 regions worldwide, allowing businesses to connect to Azure from anywhere across the globe.**
  - That’s correct. Azure VPN offers global reach with availability in over 100 regions worldwide. This allows businesses to connect to Azure from anywhere across the globe, enhancing their reach and accessibility.
- Azure VPN provides global reach by connecting retail stores to a central data center for seamless access to shared data and applications.
- Azure VPN ensures scalability by enabling remote monitoring and predictive maintenance of manufacturing equipment, optimizing production efficiency.

3. Question 3
   What is the purpose of IPsec tunnels in a VPN configuration on Azure?

- Monitoring the VPN connection status
- Establishing the Azure virtual network
- Providing authentication mechanisms
- **Enabling secure communication over the internet**
  - That’s correct. IPsec tunnels in a VPN configuration on Azure are responsible for creating a secure communication channel over the internet, ensuring the confidentiality, integrity, and authenticity of the transmitted data.

4. Question 4
   To authenticate clients connecting to a VNet over a point-to-site VPN connection in Azure, you need to upload the \***\*\_\_\*\*** certificate to Azure.

- **Root**
  - That’s correct. To authenticate clients connecting to a VNet over a point-to-site VPN connection in Azure, you need to upload the root certificate to Azure. The root certificate is considered trusted by Azure and is used for authentication.
- Client

5. Question 5
   Which authentication type is recommended for Point-to-Site (P2S) VPN connections in Azure?

- RADIUS authentication
- Active Directory integration
- Username and password
- **Azure certificate**
  - That’s correct. Azure certificate authentication is recommended for Point-to-Site (P2S) VPN connections in Azure. It involves generating a root certificate and client certificates, which are used for authentication when clients connect to the Azure VNet.
