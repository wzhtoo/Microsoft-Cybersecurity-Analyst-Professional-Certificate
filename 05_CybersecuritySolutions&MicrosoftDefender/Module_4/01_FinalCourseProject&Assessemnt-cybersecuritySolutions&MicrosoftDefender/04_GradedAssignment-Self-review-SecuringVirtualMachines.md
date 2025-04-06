# Self-review: Securing virtual machines

[Self-review: Securing virtual machines 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/assignment-submission/hRcF0/self-review-securing-virtual-machines)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/assignment-submission/hRcF0/self-review-securing-virtual-machines/attempt)

1.  Question 1
    Have you successfully deployed the Service_VM for the IT services provider?

- **Yes**
  - That’s great! Now that you have deployed a VM, the IT services provider can use it for further testing and training before protecting their production VMs.
- No

2. Question 2
   Have you successfully created a hub network with VNet peering?

- **Yes**
  - That’s great! Now the hub network and the Services_Test_Network can communicate securely.
- No

3. Question 3
   Have you successfully deployed an Azure Standard firewall ready to protect the network?

- **Yes**
  - That’s great! Now the Azure firewall is protecting the IT services provider network within Azure and it’s ready for extensive testing.
- No

4. Question 4
   You have a web application hosted on Azure. Which feature of the Azure Standard Firewall helps restrict inbound access to specific IP addresses?

- Network address translation (NAT)
- **Network rules**
  - That’s correct! By configuring network rules in Azure Standard Firewall, you can define specific source IP addresses or ranges that are allowed to access your web application.
- Custom application rules
- Load balancing rules

5. Question 5
   Have you successfully configured just-in-time access on the Services_VM?

- **Yes**
  - That’s great! Now the Services_VM’s management ports are now restricted to timed access, enhancing security..
- No

6. Question 6
   Have you successfully configured and deployed Azure Bastion?

- **Yes**
  - That’s great! Now the Services_VM can be accessed remotely by using the secure Bastion service provided by Microsoft.
- No

7. Question 7
   Which of the following protocols are supported by Azure Bastion for remote access? Select all that apply.

- **RDP (Remote Desktop Protocol)**
  - That’s correct! Azure Bastion supports RDP for remote access.
- HTTP (Hypertext Transfer Protocol)
- **SSH (Secure Shell)**
  - That’s correct! Azure Bastion supports SSH for remote access.
- FTP (File Transfer Protocol)

8. Question 8
   Were you able to remotely connect to the Services_VM using Azure Bastion and JIT access?

- **Yes**
  - That’s great! This proves that everything so far is working, and the IT services provider can carry out their testing and training.
- No

9. Question 9
   Have you successfully deployed Microsoft Sentinel?

- **Yes**
  - That’s great! Now the IT services provider can start to configure, train, and test before using the solution on the production network
- No

10. Question 10
    What does Microsoft Sentinel primarily help organizations with?

- Analyzing financial data
- Managing customer relationships
- Detecting and responding to security threats
  - That’s correct! Microsoft Sentinel is designed to help organizations be proactive in detecting and responding to security threats.

11. Question 11
    What is the name of the instance used for Azure Bastion configuration in Step 5?

- **Services_Bastion**
- AccessBastion
- BastionVM
- SecureBastion

12. Question 12
    What is the purpose of creating a hub network with VNet peering in Step 2 of the exercise?

- To provide remote access to virtual machines
- To deploy an Azure Standard Firewall
- To establish a connection to the public internet
- **To enable communication between virtual networks for enhanced security**
  - That’s correct! Creating a hub network with VNet peering allows for communication between virtual networks, enhancing security by enabling controlled data exchange between them. Well done!

13. Question 13
    What is the purpose of deploying the Azure Standard Firewall in Step 3 of the exercise?

- To manage JIT (just-in-time) access
- **To protect and secure the network**
  - That’s correct! The Azure Standard Firewall is deployed to protect and secure the network by filtering incoming and outgoing traffic, thus enhancing the network's security.
- To provide remote desktop access
- To monitor the testing environment

14. Question 14
    In Step 7, what type of workspace is created when implementing Microsoft Sentinel?

- Application Insights Workspace
- Logic App Workspace
- Azure Sentinel Workspace
- **Log Analytics Workspace**
  - That’s correct! Microsoft Sentinel uses a Log Analytics Workspace to collect and analyze security-related data for monitoring and detection.

15. Question 15
    What is the main purpose of enabling just-in-time (JIT) access on the Services_VM in Step 4 of the exercise?

- To allow unlimited and unrestricted access to the virtual machine
- To automatically deploy security updates to the virtual machine
- **To enhance security by controlling and limiting remote access to the virtual machine**
  - That’s correct! Just-in-time (JIT) access is implemented to enhance security by controlling and limiting remote access to the virtual machine's management ports. It ensures that access is only granted when needed, reducing the attack surface.
- To restrict remote access and only allow access during specified times
