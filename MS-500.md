Security Administrator Associate
----------------------------------


MFA
•	If a user is in two groups that enables and disables MFA, then the user doesn’t have to change their password.
•	If MFA is disabled in a group but required overall, the users will be blocked.
•	Required to run Attack Simulator.

•	Enable MFA for user
•	Active user —> MFA —> Service Settings —> 
•	App passwords allow
•	Remember MFA for 30 days
•	Save
•	—> Users —> Select User —> Enable


Password policy
•	Groups will override conditions e.g. user must change password but the Group is excluded, it overrides. Even if user is in another group that includes it.
•	M365 Admin —> Settings —> Org. Settings —> Security & Privacy



Roles


Can view permissions of Role in AAD

•	Principle of least privilege 
•	Eligible 

•	Global Admin 
•	Can Everything
•	Enable and configure Azure AD PIM

•	Privileged Role Admin 
•	can approve Roles

•	Security Admin 
•	CANNOT approve roles
•	Configure user risk policy
•	View user risk report
•	View ATP Reports in Threat management dashboard
•	Can enable Microsoft Defender ATP

•	Security operator
•	View user risk report  
•	Security reader
•	Can view ATP reports
•	

•	Compliance admin
•	CANNOT view user risk report  
•	Service Admin
•	Monitor service health of M365 
•	Organisation Management
•	EXO —> Permissions —> Admin Roles 

•	Portal Admin
•	Can assign Compliance Manager role  
•	Message center reader
•	Reports reader
•	Security reader


Azure AD Connect
•	View Azure AD Connect events?
•	NO
•	System event loh
•	Directory Service event log
•	Security event log

•	YES
•	Application event log



Legacy Authentication

https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/concept-fundamentals-block-legacy-authentication#:~:text=Legacy%20authentication%20is%20a%20term,such%20as%20IMAP%2FSMTP%2FPOP3
Blocking legacy authentication protocols in Azure AD | Microsoft Docs

https://xenit.se/tech-blog/discover-users-running-legacy-authentication-and-why-you-need-to-disable-it/
Discover users running Legacy Authentication and why you need to disable it - Xenit


•	AAD —> Sign-ins —> Client App —> See who is using legacy authentication

•	Directory
•	Office apps
•	Exchange and Sharepoint
•	Skype for Business
•	Apps on iOS (e.g. mail app in iOS <11)
•	On-prem (hybrid solutions)
•	WiFi

 




Modern Authentication

•	Authentication methods: Multi-factor authentication (MFA); smart card authentication; client certificate-based authentication
•	Authorisation methods: Microsoft's implementation of Open Authorisation (OAuth)
•	Conditional access policies: Mobile Application Management (MAM) and Azure Active Directory (Azure AD) Conditional Access

The modern strategy, known as claims-based authentication and authorisation is configuring your application to use tokens that provide the identity and access rules of your users.

Identity token —> its like a drivers license, something you can use to verify your age in a lot of places. 




Advanced Threat Protection


 


•	Microsoft Defender for Identity
•	Formerly Azure ATP
•	Identity security
•	Protecting on-premise AD users
•	Offers recommendation for identity configuration   
•	Office 365 ATP
•	Included in Plan 1
•	Protects users via messaging platform
•	Safe links
•	Anti-phishing
•	Reporting



•	Microsoft Defender ATP
•	Endpoint and detection
•	Comes with Windows
•	Threat & Vulnerability dashboard —> shows vulnerabilities and system misconfigs
•	Security Operations dashboard —> active alerts
•	Detects abd responds to attacks i.e. activities not typical for device
•	Isolates machines
•	Quarantining files

•	XDR
•	Extended detection and response


•	Azure Defender
•	Workspaces
•	AI and Automation
•	Protects RDP brute force attacks
•	Azure and hybrid workload protection
•	Protects hybrid data hosted in Azure
•	Detects unusual attempts to access Azure data


•	Read link… too tired right now


•	Look at more details here….
https://azure.microsoft.com/en-us/services/azure-defender/#:~:text=Azure%20Defender%20is%20a%20built,premises%2C%20and%20in%20other%20clouds.
Azure Defender | Microsoft Azure


Azure ATP
•	When adding Azure ATP sensors on DCs, in order to view memberships changes, you must
•	Policy Default Domain Controllers Policy
•	Audit Setting Audit Security Group Membership
•	https://docs.microsoft.com/en-us/defender-for-identity/configure-windows-event-collection 
•	How to minimise email delivery but still screen for malware?
•	Set the action to Dynamic Delivery

•	Enable delayed deployment of updates for an ATP sensor. 
•	How long before ATP cloud service is updated? 72 hours to update 
•	Detect when sensitive groups are modified on-prem
•	Event Forwarding on domain controllers 
•	ATP sensor
•	Standalone sensor in Server1
•	How to monitor DC1? Configure port mirroring for DC1
•	Event subscription —> for monitoring 



Microsoft Defender ATP
•	https://docs.microsoft.com/en-us/microsoft-365/security/office-365-security/office-365-atp?view=o365-worldwide
•	Only Windows devices can be evaluated with ATP risk level 
•	Custom network indicators

•	Microsoft Monitoring Agent (tool to download)

•	Machine groups?




Identity Protection

•	Anonymous IP adress
•	Atypical travel (weird location)
•	Malware linked IP address
•	Leaked credentials
•	Password spray
•	Suspicious inbox forwarding
•	Etc.




Conditional Access

Block legacy authentication
Require MFA for administrators
Require MFA for Azure management
Require MFA for all users


Sign-in risk-based Conditional Access (Requires Azure AD Premium P2)
User risk-based Conditional Access (Requires Azure AD Premium P2)
Require trusted location for MFA registration
Block access by location
Require compliant device
Block access except specific apps
Can e.g. prevent users downloading, sharing, etc. 
Require multi-factor authentication (Azure AD Multi-Factor Authentication)
Require device to be marked as compliant (Intune)
Require Hybrid Azure AD joined device
Require approved client app
Require app protection policy


Administrators can choose to require one of the previous controls or all selected controls using the following options. The default for multiple controls is to require all.

•	Require all the selected controls (control and control)
•	Require one of the selected controls (control or control)


•	Report only mode


Session control

•	Supported Cloud Apps
•	Exchange Online
•	SharePoint Online

•	Prevents
•	Downloads
•	Uploads (e.g. unlabelled files)
•	Blocks e.g. certain users from certain apps
•	Monitor e.g. risky users

•	Sign-in frequency 
•	Persistent browser session



Sentinel
•	SIEM that uses A.I. to analyse large volumes of data
•	Hunts for suspicious activities
•	Workspace
•	Playbook


Microsoft Office 365 Threat Protector
•	xxx



Azure Information Protection
•	xxx


Bitlocker
•	BitLocker to Go —> All devices
•	Auto-unlock —> Requires BitLocker Drive Encryption on C:



Security Groups
•	Windows Workspace —> Security Group in Azure AD and M365 Admin
•	Dynamic
•	Assigned
•	Policy 
•	Scope


Security
•	Security —> Threat management —> Policy —> Safe Links —> Block
•	To store information where users click on unsafe link, uncheck “Do not track” 
•	


Cloud Apps
•	Monitor apps in realtime
•	Register App1
•	Create CA policy
•	Create access policy 
•	Can be used to e.g. see which OneDrive files were modified by which users



DLP
•	


Windows Defender Exploit Guard




Exchange Online
•	How to quarantine unmanaged mobile devices
•	EXO —> Mobile —> Edit —> Quarantine

•	Organisation Management Admin
•	EXO —> Permissions —> Admin Roles


Intune
•	Attack surface reduction policy
•	Enforce components, Store Apps, and Smartlocker
•	Member will receive security warning (enabled) or site will just open (disabled.
