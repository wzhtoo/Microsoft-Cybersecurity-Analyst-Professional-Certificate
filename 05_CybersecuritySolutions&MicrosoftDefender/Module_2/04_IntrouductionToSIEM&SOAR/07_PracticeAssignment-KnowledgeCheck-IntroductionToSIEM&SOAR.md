# Knowledge check: Introduction to SIEM and SOAR

[Knowledge check: Introduction to SIEM and SOAR 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/assignment-submission/t2OiL/knowledge-check-introduction-to-siem-and-soar)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-solutions-and-microsoft-defender/assignment-submission/t2OiL/knowledge-check-introduction-to-siem-and-soar/attempt)

1.  Question 1
    What are the four security operation areas of Microsoft Sentinel?

- **Collect, Detect, Investigate and Respond**
  - That's correct! Microsoft Sentinel collects data that is used to detect alerts and threats, which can then be investigated before a response is neede
- Collect, Detect, Investigate and Redirect
- Collect, Detect, Investigate, and Repair

2. Question 2
   Once Microsoft Sentinel has been deployed, what needs to be configured next?

- Threat response
- Data analysis
- Threat hunting
- **Data collection using data connectors**
  - That's correct! Microsoft Sentinel uses data connectors to collect data ready for analysis.

3. Question 3
   True or false: To use Microsoft Sentinel, a virtual machine needs to be deployed within Azure.

- True
- **False**
  - That's correct! Microsoft Sentinel is a service that you deploy within Azure. No virtual machines are needed.

4. Question 4
   Microsoft Sentinel combines both SIEM and SOAR. What two features form part of SOAR?

- Threat hunting
- **Automation rules**
  - That's correct! Microsoft Sentinel uses automation rules to help automate some of the simple security response tasks.
- **Playbooks**
  - That's correct! Microsoft Sentinel uses playbooks to automate responses and remediate incidents.
- Analytics

5. Question 5
   What is used to convert syslog data before it is sent to Microsoft Sentinel?

- **Log analytics agent**
  - That's correct! The log analytics agent can be installed on a VM to convert syslog data from different sources to Microsoft Sentinel.
- APIs
- Workbooks

6. Question 6
   You are responsible for implementing a Security Orchestration, Automation, and Response (SOAR) solution using Microsoft Sentinel. Which of the following options accurately describes how Sentinel can be utilized for SOAR?

- Sentinel enables you to centrally collect and analyze security data, but it does not support automation or response actions.
- **Sentinel combines centralized security data collection and analysis with automation and response capabilities, making it an ideal choice for implementing SOAR.**
  - That's correct! Microsoft Sentinel integrates with various data sources to collect and analyze security events, logs, and telemetry from across the organization. Sentinel also offers automation and response capabilities, allowing security teams to orchestrate actions and automate responses to detected threats.
- Sentinel provides automation and response capabilities, but it doesn’t have the ability to collect and analyze security data.
