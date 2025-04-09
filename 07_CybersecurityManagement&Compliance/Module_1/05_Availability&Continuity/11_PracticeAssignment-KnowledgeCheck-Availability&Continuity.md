# Knowledge check: Availability and continuity

[Knowledge check: Availability and continuity 🔗](https://www.coursera.org/learn/cybersecurity-management-and-compliance/assignment-submission/S7nCw/knowledge-check-availability-and-continuity)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-management-and-compliance/assignment-submission/S7nCw/knowledge-check-availability-and-continuity/attempt)

1.  Question 1
    Anna is the IT Manager of a multi-national company and wants to utilize cloud services for their new web application. Her primary concerns are ensuring that the application remains functional even if a disaster strikes in one datacenter, and she also wants high accessibility and low latency.

Considering Anna's needs and based on the information provided, which of the following Azure offerings should she opt for?

- Azure virtual machines without manual replication across zones
- **Zone-redundant services**
  - Correct! Zone-redundant services are replicated across availability zones in a region, providing resilience against zone-level failures. This ensures that if one zone has an issue, the application remains functional in other zones. This setup also provides high availability and low latency.
- Azure Traffic Manager
- Non-zonal services

2. Question 2
   True or False: Microsoft handles all disaster recovery tasks, including virtual machine replication in Azure.

- **True**
- False

3. Question 3
   You are the cloud architect for a global company that has decided to move its services to Azure. In a recent board meeting, the CEO expressed concerns about potential downtimes and datacenter failures. You recall Azure's infrastructure provisions for such challenges.

Which of the following best explains Azure's infrastructure strategy to ensure high availability and disaster recovery for the company's services?

- Azure solely relies on individual data centers for application hosting, which means services are susceptible to regional failures.
- Azure’s strategy is to only have availability zones without regions, with each zone being an isolated datacenter anywhere in the world.
- Azure ensures high availability by solely depending on special regions like China East and Germany Central, which are operated under unique partnerships and models.
- **Azure uses both regions and availability zones, where each region is a distinct geographic area with datacenters. Availability zones are separate locations within a region, each having its own power, cooling, and networking.**
  - Correct! Regions provide geographical flexibility for optimal performance, while availability zones further enhance reliability by being physically separate within a region, ensuring services remain online even during data center failures.

4. Question 4
   Complete the following sentence. To cater to both reliability and scalability monitoring needs for an online sales platform while expecting a surge in traffic, you should **\_\_\_** for full-stack monitoring, use **\_\_\_** for deep insights into application health and configure Azure **\_\_\_** based on metrics analysis.

- **Implement Azure Monitor, Application Insights, auto-scaling rules**
  - Correct! Azure Monitor offers comprehensive monitoring, Application Insights provides application health data, and configuring auto-scaling rules will ensure the system scales as per demand.
- Use Azure Service Health, Application Insights, manual scaling alerts
- Solely depend on Azure AD Logs, Application Insights, auto-scaling for all Azure services

5. Question 5
   You are an Azure architect for a multinational shipping company. The company's board of directors has expressed concerns about potential large-scale disasters, such as hurricanes, affecting their tracking portal which is currently hosted in the East US Azure region. They've asked for your recommendations on how to make the system more resilient. While analyzing the current architecture of the tracking portal, you realize that some components are inherently global, some are regional, and some are configurable for multi-region support.

Which of the following approaches should you prioritize to ensure minimal disruption during a regional disaster?

- Increase the number of instances for each service in the East US Azure region to ensure that even if some instances fail, others remain operational.
- **Propose a multi-region architecture, replicating regional components to a secondary Azure region and ensuring that configurable components like Azure SQL Database and Azure Cosmos DB employ geo-replication.**
  - Correct! By replicating regional components to a secondary region and employing geo-replication for configurable components, you can achieve higher resilience and reduce downtime during regional disasters.
- Replace all regional components with their on-premises equivalents to reduce dependency on Azure regions.
- Migrate all services to global components like Azure DNS and Azure CDN to ensure worldwide accessibility.
