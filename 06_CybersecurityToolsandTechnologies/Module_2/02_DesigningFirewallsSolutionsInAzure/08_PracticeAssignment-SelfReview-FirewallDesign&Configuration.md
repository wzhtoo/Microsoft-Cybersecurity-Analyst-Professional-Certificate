# Self review: Firewall design and configuration

[Self review: Firewall design and configuration 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/assignment-submission/E8cul/self-review-firewall-design-and-configuration)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-tools-and-technologies/assignment-submission/E8cul/self-review-firewall-design-and-configuration/attempt)

Introduction
In the
Firewall design and configuration
exercise, you had the opportunity to create an effective and secure Azure Firewall solution tailored to meet the specific requirements of ABC Inc. The exercise allowed you to explore essential concepts and best practices related to network topology, firewall rules, NAT rules, application rules, logging and monitoring, high availability options, and security considerations.

Now, it's time to assess your understanding and application of the concepts covered in the exercise through a self-review quiz.

1.  Question 1
    Which topology did you identify as the best suited solution for ABC Inc.’s Azure Firewall design?

- Fully meshed
- **Hub-and-spoke**
  - Well done. The Hub-and-Spoke topology provides centralized traffic control and enhanced security for ABC Inc.'s virtual networks.

2. Question 2
   Which firewall rules did you include for the Azure Firewall design?

- Only outbound
- **Inbound and outbound**
  - Well done. The design should include essential rules to control traffic between virtual networks and the internet, as well as inter-spoke communication.
- Only inbound

3. Question 3
   Are NAT rules needed for the virtual networks to communicate with the internet?

- **Yes**
  - Well done. NAT rules are necessary for enabling internet access for the spoke virtual networks through Azure Firewall.
- No

4. Question 4
   Have you considered the importance of enabling logging for the Azure Firewall?

- **Yes**
  - Well done. Enabling logging is crucial for security analysis and monitoring of the firewall's activities.
- No

5. Question 5
   Which security considerations are important when configuring and maintaining Azure Firewall for web application protection? Select all that apply.

- Implementing default passwords
- **Regular updates and patches**
  - That’s correct. Regular updates and patches are crucial to keep the Azure Firewall secure and protected against potential vulnerabilities.
- **User-defined routes (UDRs)**
  - That’s correct. Using UDRs to direct traffic to Azure Firewall for inspection is an important part of the security strategy.
- That’s correct. It’s vital to ensure secure access to Azure Firewall's management ports from trusted networks and authorized administrators.
  - That’s correct. It’s vital to ensure secure access to Azure Firewall's management ports from trusted networks and authorized administrators.
- Just-in-time (JIT) access
- **Network security groups (NSGs)**
  - That’s correct. Applying NSGs to the virtual networks provides valuable traffic control and access restrictions.
