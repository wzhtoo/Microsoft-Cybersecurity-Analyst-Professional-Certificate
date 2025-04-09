# Self review: Identify and respond

[Self review: Identify and respond 🔗](https://www.coursera.org/learn/cybersecurity-management-and-compliance/assignment-submission/AN2Iu/self-review-identify-and-respond)

# Assignment

[Assignment 🔗](https://www.coursera.org/learn/cybersecurity-management-and-compliance/assignment-submission/AN2Iu/self-review-identify-and-respond/attempt)

In the exercise Identify and Respond, you were tasked with detecting and subsequently preventing an insider threat. Now you are ready to respond to the following questions to ensure that you understood and executed the tasks correctly.

1.  Question 1
    A new employee in your organization tried to access the "employee_data.csv" file from the Azure Blob Storage.

Which Azure feature would immediately alert you about this unusual data access pattern?

- Just-In-Time (JIT) VM access
- Azure Sentinel deployment
- **Azure Security Center alerts**
  - Correct! Azure Security Center can trigger alerts for unusual data access patterns.

2. Question 2
   After detecting an inside threat, you want to restrict a user's access to the Blob Storage for only a limited duration.

- Which Azure feature would you use?
- Azure Policy implementation
- Azure Sentinel incidents
- **Just-In-Time (JIT) VM access**
  - Correct! JIT allows users to request access for a limited time.

3. Question 3
   An organization wants to ensure that all blob storages have Azure Defender enabled.

Which feature should they implement?

- Azure Sentinel deployment
- **Azure Policy implementation**
  - Correct! Azure Policy can be created and enforced to ensure specific conditions, like having Azure Defender enabled on all blob storages.
- Azure Security Center activation

4. Question 4
   Given the scenario provided where a possible inside threat was simulated and detected using Azure Security Solutions:

Which of the following measures and features were implemented to detect and prevent the threat in the Azure environment? Select all that apply.

- **Azure Activity log was connected as a data source to Azure Sentinel.**
  - Correct! The Azure Activity log was indeed connected to Azure Sentinel to enhance the detection capabilities.
- Azure Policy was implemented to ensure that all VMs are encrypted.
- A policy was enforced to require multi-factor authentication (MFA) for all Azure users.
- **Activation of the Standard tier of Azure Security Center for enhanced security capabilities.**
  - That’s correct! The Standard tier of Azure Security Center was activated to provide enhanced security measures and monitor Data Storage Access.
- **Just-In-Time (JIT) VM Access was configured, allowing users limited-time access to the Blob Storage.**
  - Correct! JIT access was set up, providing testuser@company.com with only a 1-hour access window to the Blob Storage
