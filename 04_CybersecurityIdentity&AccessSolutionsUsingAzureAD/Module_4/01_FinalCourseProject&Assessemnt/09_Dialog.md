# IT administrator for Sam’s Scoops

[IT administrator for Sam’s Scoops 🔗](https://www.coursera.org/learn/cybersecurity-identity-and-access-solutions-with-azure-ad/ungradedWidget/8d203/it-administrator-for-sams-scoops)

Coach
Hello! I am your Coursera Coach for this activity. We will be working together to improve the security of Sam's Scoops using Azure AD. We will achieve this by going through a series of checkpoints, focusing on practical solutions for everyday situations.

Checkpoint 1: Managing Unauthorized Access (Weight = 20%).
Checkpoint 2: Securing Login Attempts (Weight = 25%).
Checkpoint 3: Ensuring Device Compliance (Weight = 25%).
Checkpoint 4: Managing Former Employee Accounts (Weight = 15%).
Checkpoint 5: Protecting Privileged Access (Weight = 15%).
You can pause this session at any time and return to it later. Your progress will be tracked as we go. Let me know when you are ready to start.

Win
Let's get started

1. Coach
   Let's tackle the first challenge: Sam's Scoops experienced unauthorized access to its payroll application. How can you leverage Azure AD's Role-Based Access Control (RBAC) to prevent this from happening again?

### Answer

You can use Azure AD Role-Based Access Control (RBAC) to stop unauthorized access by:

Giving access only to the right people – Assign roles only to employees who need them.

Using the "Least Privilege" rule – Don’t give more permissions than necessary.

Removing unused roles – Check and remove access from people who no longer need it.

Using Conditional Access – Require extra security (like MFA) for sensitive apps.

This way, only the right people can access the payroll system!

2. question
   > That's a great start! You correctly identified key RBAC principles and their importance in securing access. You understand that it's crucial to grant access based on job roles and responsibilities, adhering to the principle of least privilege. You also highlighted the importance of regularly reviewing and revoking unnecessary access. You can further strengthen security by implementing Conditional Access policies. For example, requiring multi-factor authentication for accessing the payroll application adds an extra layer of security. Now, let's dive a bit deeper. How would you implement RBAC specifically for the payroll application in Azure AD, considering there might not be a pre-defined "Payroll Manager" role? What would you do in such a scenario?

### Answer

If there's no pre-defined "Payroll Manager" role, I would:

Create a Custom Role – In Azure AD, I would make a new role called "Payroll Manager" with only the permissions needed for the payroll app.

Define Permissions – Allow only what’s necessary, like viewing and managing payroll data.

Assign the Role – Give the Payroll Manager role to the right employees.

Use Conditional Access – Require MFA and only allow sign-ins from trusted devices or locations.

Review Access Regularly – Check who has the role and remove it if they don’t need it anymore.

This keeps payroll data safe while making sure the right people can do their jobs!

3. Question
   > Excellent! You've demonstrated a solid understanding of how to implement RBAC in Azure AD, even when dealing with specific access needs. Creating a custom "Payroll Manager" role with granular permissions is the right approach. By defining permissions for viewing and managing payroll data and assigning this role only to authorized employees, you effectively restrict access to those who need it. Combining this with Conditional Access policies like MFA and location-based restrictions further strengthens security. Regularly reviewing access ensures that permissions stay aligned with job responsibilities. You are 20% complete.

### Answer

Great! Ready for the next checkpoint. Let’s secure those login attempts! 🚀🔐

4. Question
   > Sam's Scoops is facing multiple failed login attempts from unfamiliar IP addresses. What Azure AD tools and features would you employ to detect and address these potentially suspicious activities?

### Answer

To protect Sam’s Scoops from suspicious login attempts, I would use these Azure AD security features:

1. Azure AD Sign-In Risk Policies
   Detects unusual sign-in behavior (e.g., logins from unfamiliar locations or impossible travel scenarios).

Automatically prompts for Multi-Factor Authentication (MFA) or blocks access based on risk level.

2. Conditional Access Policies
   Requires MFA for high-risk sign-ins.

Blocks access from untrusted or unfamiliar IPs.

Restricts logins to trusted locations (e.g., office network).

3. Azure AD Identity Protection
   Uses machine learning to analyze login patterns and detect compromised accounts.

Provides real-time alerts for risky sign-ins.

4. Named Locations & IP Restrictions
   Defines trusted IP ranges to block logins from unknown locations.

5. Log Monitoring with Azure AD Sign-In Logs
   Tracks failed login attempts to investigate unusual activity.

Can be integrated with Microsoft Sentinel for security insights.

Would you like a step-by-step guide on setting up these policies? 🚀

5. Question
   > That's a comprehensive list of Azure AD security features and their applications in securing login attempts! You clearly understand how to leverage these tools to enhance Sam's Scoops' security posture. You correctly identified Azure AD Identity Protection, Conditional Access Policies, and Sign-in risk policies as valuable tools for detecting and responding to suspicious login activities. Defining trusted locations and IP restrictions adds another layer of protection. Regularly monitoring Azure AD Sign-in logs helps identify trends and potential threats. Integrating these logs with Microsoft Sentinel allows for more advanced threat analysis and response. You are now 45% complete. Are you ready to move on to the next checkpoint?

### Answer

Yes! I'm ready to move on to the next checkpoint. Let's continue securing Sam’s Scoops!

6. Question
   > Sam's Scoops has devices with outdated security settings trying to access its network. What steps would you take using Azure AD to ensure device compliance and secure access to company resources?

### Answer

To ensure device compliance and secure access to Sam's Scoops' network, I would take the following steps using Azure AD:

1. Implement Conditional Access Policies
   Require compliant devices to access company resources.

Enforce Multi-Factor Authentication (MFA) for non-compliant or unmanaged devices.

2. Enable Microsoft Intune for Device Compliance
   Use Intune Compliance Policies to ensure devices meet security standards (e.g., OS version, encryption, antivirus).

Block or restrict access for non-compliant devices.

3. Require Device Enrollment in Azure AD
   Enforce Azure AD Join or Hybrid Azure AD Join for company-owned devices.

Use Mobile Device Management (MDM) to monitor and manage security settings.

4. Monitor & Enforce Security Baselines
   Use Microsoft Defender for Endpoint to assess security compliance.

Regularly review Azure AD Sign-in logs to detect risky devices.

5. Implement Access Restrictions for Unmanaged Devices
   Use App Protection Policies for BYOD (Bring Your Own Device).

Restrict access to sensitive data from unmanaged or jailbroken devices.

By applying these steps, only secure and compliant devices will be able to access company resources, reducing the risk of security breaches.

Would you like to dive deeper into any of these areas?

7. Question
   > That's an excellent strategy for ensuring device compliance at Sam's Scoops! You've effectively combined several Azure AD features to create a robust security posture. Requiring compliant devices through Conditional Access policies and enforcing MFA for non-compliant ones is a great start. Leveraging Microsoft Intune for device compliance management and enforcing device enrollment ensures that only devices meeting security standards can access company resources. Monitoring security baselines and implementing access restrictions for unmanaged devices adds another layer of protection. You are now 70% complete. Are you ready to move on to the next checkpoint?

### Answer

Yes! I'm ready to move on to the next checkpoint. Let’s tackle the next challenge!

8. Question
   > Sam's Scoops discovered that former employees still have active accounts. How would you leverage Azure AD Identity Governance to automate account deactivation and ensure proper access management?

### Answer

To automatically deactivate former employees' accounts and ensure proper access management, I would use Azure AD Identity Governance with the following steps:

1. Implement Access Reviews
   Regularly review user access to detect inactive or unnecessary accounts.

Configure automatic removal of access when employees leave.

2. Use Lifecycle Workflows
   Automate deactivation of accounts based on HR data or employment status changes.

Set up workflows to revoke access and disable accounts when an employee exits.

3. Leverage Entitlement Management
   Assign access packages that automatically expire when an employee leaves.

Require periodic re-approval for continued access to sensitive resources.

4. Conditional Access Policies
   Block sign-ins from inactive accounts.

Restrict access for accounts not meeting security conditions (e.g., non-company devices).

5. Automate Offboarding with Power Automate
   Integrate with HR systems to trigger account disablement upon termination.

Automatically revoke licenses and remove group memberships.

This approach ensures that former employees lose access immediately, reducing security risks at Sam’s Scoops.

Would you like to explore more automation options?

9. Question
   > That's a well-defined plan for managing former employee accounts using Azure AD Identity Governance! You've effectively combined automated processes and access reviews to mitigate security risks associated with inactive accounts. Implementing access reviews with automatic removal, leveraging lifecycle workflows for account deactivation, and using entitlement management for time-bound access are excellent strategies. Integrating Conditional Access policies to block inactive accounts and automating offboarding with Power Automate further strengthens security. You are now 85% complete. Are you ready for the final checkpoint?

### Answer

Yes! I'm ready for the final checkpoint. Let's move forward and secure privileged access at Sam’s Scoops!

10. Question
    > Sam's Scoops wants to enhance the security of its privileged roles. How would you implement Privileged Identity Management (PIM) in Azure AD to manage and secure these sensitive accounts, and what role does just-in-time (JIT) access play in this strategy?

### Answer

To enhance the security of privileged roles at Sam’s Scoops, I would implement Azure AD Privileged Identity Management (PIM) with the following strategies:

1. Implement Just-In-Time (JIT) Access
   Require on-demand activation for privileged roles instead of permanent assignments.

Set time-limited access (e.g., 1 hour) to reduce exposure to attacks.

Require users to justify access when activating a privileged role.

2. Use Role-Based Access Control (RBAC)
   Assign only necessary roles to users following the principle of least privilege.

Use custom roles if default roles don’t fit specific needs.

Regularly review and update role assignments.

3. Require Multi-Factor Authentication (MFA) for Role Activation
   Enforce MFA every time a user requests elevated access.

Prevent unauthorized users from activating privileged roles.

4. Enable Access Reviews
   Schedule regular reviews of privileged role assignments.

Automatically remove access if no longer needed.

Require manager or security team approval before extending access.

5. Set Up Approval Workflows
   Require manager or security admin approval before activating high-risk roles.

Notify security teams when privileged roles are activated.

6. Monitor and Audit Privileged Access
   Track all role activation events in Azure AD logs.

Use Microsoft Sentinel for advanced threat detection.

Set up alerts for unusual privileged access activities.

By using PIM with Just-In-Time (JIT) access, Sam’s Scoops minimizes risk by reducing standing privileges, ensuring only authorized users can access sensitive resources when needed.

Would you like to explore additional security automation for privileged access?

11. Question
    > That's a fantastic plan for securing privileged access at Sam's Scoops using PIM! You've clearly outlined a comprehensive strategy that combines JIT access, RBAC, MFA, access reviews, approval workflows, and robust monitoring. By implementing these measures, Sam's Scoops can significantly reduce the risk of unauthorized access to sensitive resources and strengthen its overall security posture. You have successfully completed this activity! Congratulations on reaching 100% completion! Let me know if you have any questions or if there's anything else I can assist you with.

During today's session covering Managing Unauthorized Access, Securing Login Attempts, Ensuring Device Compliance, Managing Former Employee Accounts, and Protecting Privileged Access, our goal was to improve the security of Sam's Scoops using Azure AD. Your responses show an Advanced level.
The strengths I saw in your responses are:

Comprehensive understanding of Azure AD security features.
Detailed and practical solutions tailored to the scenarios. Keep up the good work! If you want to continue practicing, start a new chat.
