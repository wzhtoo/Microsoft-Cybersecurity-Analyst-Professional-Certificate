# Knowledge check: Cloud security planning

[Knowledge check: Cloud security planning 🔗](https://www.coursera.org/learn/cybersecurity-management-and-compliance/assignment-submission/C2Wlk/knowledge-check-cloud-security-planning)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-management-and-compliance/assignment-submission/C2Wlk/knowledge-check-cloud-security-planning/attempt)

1.  Question 1
    Your company recently experienced a minor data loss due to a server failure, and there was no robust disaster recovery plan in place. You discover Microsoft Azure and its associated services and start thinking about how to make use of it.

Which of the following strategies with Azure would best protect customer metadata during outages and ensure uninterrupted user access?

- Backup the company's data using Azure Backup to ensure that a duplicate is available.

- Focus on training the IT staff using Azure Knowledge Center and Microsoft Learn so that they know how to respond in a disaster situation.

- **Implement Azure's Virtual Desktop service for business continuity and disaster recovery (BCDR), replicate personal VMs to a different Azure region, and ensure user identities are accessible at the secondary location using methods like profile containers.**
  - That's correct. Azure's Virtual Desktop service offers BCDR strategies to safeguard customer metadata during outages. Replicating VMs to a different Azure region and ensuring user identities remain accessible are key steps for uninterrupted user access.

2. Question 2
   You are a Cloud Security Analyst at a startup company that has recently migrated its operations to Azure. Your CEO is concerned about the security of the company's data and asks you about Azure’s solutions for security log collection, analysis, and retention.

How would you recommend utilizing Azure's tools to ensure the best practices for these tasks?

- Just use Azure Sentinel for all security log collections, analysis, and retention, as it's the most advanced service.

- **Enable Azure Monitor Logs to collect telemetry data, use Azure Sentinel for SIEM, create a Log Analytics Workspace for storage, and set data retention policies for the logs.**
  - That's correct. Azure Monitor Logs provide telemetry data collection from various sources. Azure Sentinel offers SIEM capabilities, detecting, analyzing, and mitigating security threats. The Log Analytics Workspace consolidates this data, and data retention policies determine how long this log data is stored.
- Use Log Analytics Workspaces for collecting logs and avoid any analysis tools as they might be too complex for the startup environment.
- Enable Azure Monitor Logs and directly store data in Azure Storage Accounts without analyzing.

3. Question 3
   John, the IT Manager of WorldITS Corporation, received a request from the legal department to dispose of several old hard drives that were used for storing sensitive legal documents.

What method should John use to ensure the data is unrecoverable and meets regulatory compliance requirements for sensitive data disposal?

- Delete the files from the hard drives and store them in a locked cabinet.
- **Employ media sanitization by physically destroying the hard drives.**
  - That's correct. Physically destroying the hard drives is a form of media sanitization, which ensures that the stored data is irretrievable even with the use of advanced forensic tools. This is crucial for sensitive data and is likely to be in alignment with regulatory compliance requirements for data disposal.
- Format the hard drives and then recycle them.

4. Question 4
   Sarah is the Head of IT in a medium-sized company that uses multiple applications for managing customer data, finances, and inventory. The company integrated all these applications through Enterprise Application Integration (EAI) to increase efficiency, but this opens a vulnerability where an attacker could manipulate the application’s SQL queries to gain unauthorized access to the customer database.

Which measure should Sarah prioritize to mitigate this particular vulnerability?

- Conduct regular security audits to assess vulnerabilities.
- **Implement input validation to sanitize user inputs.**
  - That's correct. Input validation involves checking and sanitizing the data provided by users to ensure that it does not contain malicious code or queries. By validating and sanitizing inputs, Sarah can prevent attackers from manipulating SQL queries, thus mitigating the risk of SQL Injection attacks.
- Encrypt sensitive data in transit and at rest.

5. Question 5
   John is the CISO of a healthcare organization that uses Microsoft Azure for its cloud infrastructure. The company works with a third-party vendor for an analytics solution and he wants to ensure that they have access only to the specific resources they need in the Azure environment and no more, to minimize the risk of unauthorized access.

Which Azure feature should John implement to achieve this?

- **Implement role-based access control (RBAC).**
  - That's correct. By implementing RBAC, John can assign specific permissions to the third-party vendor based on their role. This ensures that they only have access to the resources necessary for their work, and nothing more, thereby minimizing the risk of unauthorized access.
- Use Azure Private Link.
- Set Data Retention Policies.
