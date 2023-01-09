BASICS
---------------------------------------------------------

Conditional Access
	- Control access to your organization's resources
	- Grant or block access to resources based on factors such as location, device, and user identity
	- MFA



Identity Protection when you want to:
	- Risky sign-ins and user actions
	- Protect against identity-based attacks
	- Receive alerts and take action when risky activity is detected
	- ML to identify and mitigate potential threats



Azure Blueprints
	- Not responsive
	- New resources
	- Desired resources and policies
	- Deploy them as a package



Azure Bastion
	- 



APPLICATIONS
---------------------------------------------------------

Application registrations
	- Application that needs to access resources protected by Azure AD.


Service principals 
	- Application that needs to access resources (Azure or On-Prem)


Managed identities
	- Application that needs credentials (for another app or service)



Azure Landing Page
	- Site URL for a registered App
	- Webpage for information and resources about the app
	- Can also track user engagement and usage of the application through analytics and metrics



Azure Landing Zone
	- Used to host and manage applications and resources.
	- Supports the deployment and management of large-scale, complex applications.
	- Typically self-contained, isolated environment that is separate from other Azure resources.
	- May include a landing page




DEFENDER
---------------------------------------------------------

Microsoft Defender for Cloud
	- Standalone security solution
	- Protection against cyber threats, such as malware and ransomware. 
	- Real-time threat detection
	- Behavioral analysis
	- Machine learning-based protection


Microsoft Defender for Cloud apps
	- A set of security tools and services that work together to provide comprehensive protection for cloud-based systems and data.
	- Security and Compliance tools
	- Monitoring and response capabilities to detect and respond to threats and incidents




COMPLIANCE
---------------------------------------------------------

Azure Policy
	- Responsive service
	- Existing resources
	- Enforce rules and take action on non-compliant resources
	- Policy assignments: These are used to apply policy definitions to specific resources or resource groups.
	- Uses built-in Initiatives (e.g. scope of the subscription)



Azure Initiatives
	- Groups *multiple* Azure Policy Definitions together (e.g. NIST) as a *single* unit
	- Collection of policy definitions
	- A way to group and manage multiple policies for specific goals or compliance requirements
	- Resources
	- Visualize data
	- Define goals
	- Track goals
	- Basically a "dashboard"



Azure Benchmarks
	- Collection of guidelines and suggestions
	- No technical "function"
	- Basically like CIS benchmark PDFs




PLAYBOOKS
---------------------------------------------------------
Azure Playbooks
	- Azure Automation
	- Allow you to automate processes and tasks in Azure (also 3rd party tools)
		- deploying resources
		- backing up data
		- security incidents response
	- Triggered by events, schedules, or manually
	- Use a graphical interface to build and test the playbook
	- PowerShell or Graphical Automation workflows
	- Can be used to run tasks across Azure, on-premises, and other cloud environments
	- YAML



Sentinel Playbooks
	- (Basically Logic Apps)
 	- Specifically designed for security scenarios 
 		- Threat detection
 		- Investigation
 		- Visibility and insights (not quite single pane)
	- Allow you to automate processes and tasks in Azure (also 3rd party tools via data connectors)
 		- escalating incidents
 		- quarantining resource
 		- Updating security configurations
	- Triggered by events, schedules, or manually
	- Use a graphical interface to build and test the playbook
	- PowerShell or Graphical Automation workflows
	- Run tasks across Azure, on-premises, and other cloud environments
	- AGA (Azure Automation Graphical Authoring)
		- Based on Function Apps




WORKBOOKS
---------------------------------------------------------

Azure Workbooks
	- Azure Monitor
	- Not Responsive
	- Allow you to create interactive documentation for your Azure resources
	- Use a graphical interface to build and customize the workbook
	- Can be used to document processes and tasks, as well as display data from Azure resources in a visual format
	- Can be shared with others, making it a useful tool for collaboration
	- MD





Sentinel Playbooks
	- Like a custom dashboard
	- 
	- KQL
