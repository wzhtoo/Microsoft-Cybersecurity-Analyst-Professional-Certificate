# Knowledge check: Security capabilities of Microsoft Sentinel

[Knowledge check: Security capabilities of Microsoft Sentinel 🔗](https://www.coursera.org/learn/microsoft-sc-900-exam-preparation-and-practice/assignment-submission/tDOi4/knowledge-check-security-capabilities-of-microsoft-sentinel)

## Assignment

[Assignment 🔗](https://www.coursera.org/learn/microsoft-sc-900-exam-preparation-and-practice/assignment-submission/tDOi4/knowledge-check-security-capabilities-of-microsoft-sentinel/attempt)

1.  Question 1
    Imagine you want to gather continuous information on your workplace to ensure that no attack occurs; which of the following will perform this action?

- **SIEM**
  - That's correct! SIEM (Security Information and Event Management) focuses on continuously monitoring and analyzing security events and information in your workplace. This means that a continuous review is conducted on all actions to mitigate any attacks as quickly as possible.
- SOAR
- SOC

2. Question 2
   Sentinel requires logs to perform its vigilance. Where are these logs likely to be found?

- Azure Blob Storage
- **Azure Workbooks**
  - Explanation: In the context of Microsoft Sentinel:

Azure Workbooks are used to visualize and analyze log data that Sentinel collects. While logs themselves are stored in Log Analytics workspaces, Workbooks provide access to these logs through interactive dashboards and reports.

Let’s break down the incorrect options:

Azure Blob Storage is for unstructured data like images, backups, or general-purpose storage—not specifically used for Sentinel's log collection.

Azure Playbooks are used for automated responses (via Logic Apps), not for storing or accessing logs.

So even though logs are technically stored in Log Analytics, when you're interacting with or reviewing them in Sentinel, Azure Workbooks is the go-to option

- Azure Playbook

3. Question 3
   Out of the following set of activities, which one most closely matches the Sentinel's behaviors?

- Collects, ejects, investigates, and redirects
- **Collects, detects, investigates and reports**
  - That's correct! Sentinel can be configured to perform those actions by straddling both SIEM and SOAR spheres of influence.
- Collects, detects, patches, and reports

4. Question 4
   Where can you locate the automation steps that can be triggered in response to configurable system signals?

- **Playbook**
  - That's correct! A playbook is a central location to store automated responses. Playbooks will contain executable sequences that a SOAR system will call given the event's occurrence.
- Workspace
- Monitor

5. Question 5
   True or False: Sentinel can only connect with Microsoft Applications.

- True
- **False**
  - That's correct! Microsoft is configurable to connect with other SaaS applications. This makes it a cross-platform product, adding to its versatility.
