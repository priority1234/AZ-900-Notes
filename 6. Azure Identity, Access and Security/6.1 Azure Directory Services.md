Microsoft Entra ID is cloud based identity and access management service. Helps you sign in and access both Microsoft cloud apps and apps that you develop.
You control the identity accounts while Microsoft ensures the service is available globally.
Similar to on-premises Active Directory.

**Who uses Microsoft Entra ID**

IT Admin - to control access to apps and resources.
App Devs - to provide a standards based approach for adding functionality to applications that they develop like adding SSO functionality.
Users - To manage their identity and update their own passwords

**What does Entra ID do?**

Authentication - Verifies identity to grant access. Includes self-service password reset, multifactor authentication, banned passwords list and smart lockout
Single Sign-on (SSO) - Allows one identity to access multiple apps. 
Application Management - Manages cloud and on-prem apps through application proxy, SaaS app integration and My Apps portal.
Device Management - Device registration and management through Microsoft Intune. Enables conditional access policies that restrict access to known devices.

![](../Static/Pasted%20image%2020260928231951.png)


**Connecting On-Prem AD with Microsoft Entra ID**

Microsoft Entra Connect connects them. 
Synchronizes identity b/w on-prem Active Directory and Microsoft Entra ID. Changes flow between both systems so users get a consistent experience whether they access on-prem or cloud resources

**Microsoft Entra Domain Services**

Provides managed domain services. domain join, group policy, LDAP, Kerberos/NTLM authentication - without requiring you to deploy or maintain controllers in the cloud.

useful for legacy apps that can't use modern authentication. 

Microsoft Entra Domain Services integrate with existing Microsoft Entra Tenant, allowing existing groups and user accounts to carry over smoothly.

**How does Microsoft Entra Domain Services Work**

When you create a managed domain, you define a unique namespace. This is domain name. Two Windows Server Domain controllers are deployed in your selected region. This is called a replica set.

These DCs are part of managed domain and are handled by Azure. Like backups, encryption at rest using Azure Disk Encryption.

A managed domain is configured to perform a one way sync from Entra ID to Entra Domain Services. You can create resources directly in the managed domain, but they aren't synchronized back to Entra ID. 
In a hybrid env with on-prem AD DS environment, Microsoft Entra Connect syncs identity information with Microsoft Entra ID which is then synced to managed domain. 


![](../Static/Pasted%20image%2020260928233336.png)


Applications, services and VMs in Azure that connect to the managed domain can then use common Microsoft Entra Domain Services features such as domain join, group policy, LDAP and Kerberos/NTLM authentication.