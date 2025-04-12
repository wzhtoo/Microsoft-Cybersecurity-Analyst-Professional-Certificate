# Knowledge check: Basic security capabilities in Azure

[Knowledge check: Basic security capabilities in Azure 🔗](https://www.coursera.org/learn/microsoft-sc-900-exam-preparation-and-practice/assignment-submission/tOJYy/knowledge-check-basic-security-capabilities-in-azure)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/microsoft-sc-900-exam-preparation-and-practice/assignment-submission/tOJYy/knowledge-check-basic-security-capabilities-in-azure/attempt)

1.  Question 1
    True or False: Azure Firewall is a managed, cloud-based service that allows users to take full responsibility for its configuration and efficacy.

- True
- **False**
  - That's correct! Azure Firewall is a managed service, which means the responsibility for ensuring its efficacy lies with the cloud provider who is Microsoft, rather than the user.

2. Question 2
   As a new hire for an online firm, you have been tasked to review their security protocols. Currently, an important customer-facing application is deployed on the network with a network security group (NSG). The NSG ruleset prevents remote desktop protocol (RDP) requests from accessing it.

- What is the best course of action to take?
- Remove any NSG rules that prevent access from off-site.
- Create a duplicate of the service and deploy it on a network without the same level of NSG restrictions.
- **Create a new inbound rule with higher priority that conditionally allows outside access.**
  - That's correct! Creating a rule with higher priority means that the resource can be accessed, and by applying conditional access rules, you can ensure safe access.

3. Question 3
   A recent spate of DDoS attacks has been launched at your company. The bosses want a solution that will offer DDoS protection to the company but also output some telemetry that can be analyzed in azure monitor.

Which of the following options is a viable solution to achieve this?

- Azure Bastion
- DDoS infrastructure protection
- **DDoS Standard Plan**
  - That's correct! The DDoS Standard Plan offers a more robust defense, including machine learning for auto-tuning and integration with the Azure Monitor.

4. Question 4
   As the top security analyst at your firm, a new employee is implementing a customer-managed encryption process for your keys.

Where would you store your encryption keys?

- At the key store
- In Azure Bastion
- **Key vault**
  - That's correct! While the key store houses keys, it only does so when Microsoft manages the encryption. A customer-managed implementation retains the keys in the key vault.

5. Question 5
   True or False: Segmentation in network security refers to physically locating each department in its secular environment.

- **True**
- False
