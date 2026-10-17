Security model that  assumes worst case scenario and protects resources with that assumption.

Based on principles - 

Verify Explicitly - Always authenticate and authorize based on all available data points.
Use least privilege access - Limit user access with Just-in-Time and Just-Enough-Access (JIT/JEA) policies.
Assume Breach - Verify end-to-end encryption. use analytics to get visibility, drive threat detection and improve defenses

![[Pasted image 20260929235012.png]]


**Defense in depth**

Protect information and prevent it from being stolen by those not authorized to access it.
Uses series of mechanisms to slow down an attack.

**Layers of Defense in Depth**

![[Pasted image 20260929235205.png]]

Here's a brief overview of the role of each layer:

Physical Security - Secure building and access to computing hardware in data centers. 

Identity and Access - Grant access to only what's needed and sign-in events and changes are logged.
Control access to infra and change control
Use SSO or MFA
Audit events and changes

Perimeter - Protects from network based attacks against resources.
Use DDoS protection to filter large scale attacks
Use perimeter firewalls to identify and alert on malicious attacks

Network - Limit network connectivity across all your resources to allow only what's required. Limit access to reduce risk of spreading attack to other systems.
Limit communication
Deny by default
Restrict inbound internet access and limit outbound access where appropriate

Compute - Make sure compute resources are secure and controls are in place to minimize security issues. 
Secure access to virtual machines
Implement endpoint protection on devices and keep systems patched and current

Application - Follow development best practices to reduce vulnerability in code. Ex - Store secrets in Azure Key Vault 

Data - Protect data with encryption at rest and encryption in transit. 


