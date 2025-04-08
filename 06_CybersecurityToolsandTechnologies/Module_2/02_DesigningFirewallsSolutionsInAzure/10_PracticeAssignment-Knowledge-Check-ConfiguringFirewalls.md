# Knowledge check: Configuring firewalls

[Knowledge check: Configuring firewalls 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/assignment-submission/we91b/knowledge-check-configuring-firewalls)

## Assignment

[Knowledge check: Configuring firewalls 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/assignment-submission/we91b/knowledge-check-configuring-firewalls/attempt)

1.  Question 1
    What is the benefit of integrating Azure Firewall with Microsoft Sentinel in the context of network security in Microsoft Azure?

- **It helps in identifying emerging threats and applying appropriate security measures.**
  - That’s correct. By integrating Azure Firewall with Microsoft Sentinel, organizations can correlate firewall logs with other security event data, enabling better detection and response to potential threats. Additionally, threat intelligence integration helps in identifying emerging threats and applying appropriate security measures to enhance network security.
- It enables direct communication between virtual networks without the need for a gateway or VPN.
- It provides a centralized point for network services like Azure Firewall and Network Virtual Appliances (NVAs).
- It allows for enforcing restrictions on network traffic based on source/destination IP addresses, ports, and protocols.

2. Question 2
   XYZ Corporation has multiple on-premise applications that need to communicate with specific Azure services deployed in their virtual network. The company want to configure Azure Firewall to allow this communication while maintaining a robust security posture.

Which feature of Azure Firewall can the corporation use to simplify rule management and allow communication between its on-premises applications and specific Azure services hosted in its virtual network?

- **Azure Firewall application FQDN tags**
  - That’s correct. XYZ Corporation can use Azure Firewall Application FQDN Tags to simplify rule management and allow communication between their on-premises applications and specific Azure services hosted in their Virtual Network. These tags represent pre-defined groups of FQDNs for common Azure services, making it easier to create and manage rules.
- Threat Intelligence-Based Filtering
- Network rules
- Application rules

3. Question 3
   What are the main benefits of integrating network security groups (NSGs) with Azure Firewall in Microsoft Azure?

- Resource monitoring, virtual machine backup, and disaster recovery.
- Cost optimization, automatic scaling, and load balancing.
- **Centralized network security management, application-level filtering, and enhanced traffic inspection.**
  - That’s correct. Integrating NSGs with Azure Firewall brings benefits such as centralized network security management, application-level filtering, and enhanced traffic inspection.
- Real-time threat analysis, data encryption, and secure socket layer (SSL) decryption.

4. Question 4
   The recommended native option for enforcing network segmentation and controlling traffic flows across both VNets and subscriptions in Azure is \***\*\_\_\_\*\***.

- Virtual network peering
- Network security groups (NSGs)
- **Azure Firewall**
  - That’s correct. Azure Firewall provides layer 3 to layer 7 controls to govern traffic flows, enabling you to define communication rules and apply them consistently across VNets and subscriptions, enhancing network security.

5. Question 5
   Which of the following are design principles for ensuring reliability when configuring Azure Firewall? Select all that apply.

- **Deploy by using a secured virtual hub.**
  - That’s correct. Deploying by using a secured virtual hub is a design principle for ensuring reliability. A secured virtual hub can provide a centralized and secure connectivity point for your resources.
- Use a global Azure Firewall policy.
- Determine if you want to use third-party MSSP (Managed Security Service Provider).
- Enable threat intelligence on Azure Firewall.
