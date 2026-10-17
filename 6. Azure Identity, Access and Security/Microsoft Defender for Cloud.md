Threat protection service. Monitors cloud, on-prem, hybrid and multicloud resources and provides alerts to improve security posture.
Helps track risks and respond to threats. Natively Enabled.

**Coverage across cloud and hybrid env**

Azure native, so many azure services can be monitored without extra deployment. 
For hybrid and multicloud, it extends visibility so security teams can work from one control plane.
Can deploy data collection components for security insights.
Azure Arc can extend Microsoft Defender plants to non-Azure machines 
Cloud Security Posture Management (CSPM) can assess multicloud resources agentlessly.

**Azure Native Protections**

Azure PaaS Services - Detects threats across services such as App Service, Azure SQL and Azure Storage
Azure Data Services - Provides security assessments and recommendations for Azure SQL and Storage
Networks - Reduce brute-force exposure through controls such as just-in-time VM access and restrictive port policies.

**Defend Resource on Other clouds**

Can protect resources in other clouds including AWS and GCP

For connected AWS environments, it can - 

Extend CPSM recommendations and compliance assessments to AWS resources
Extend Defender for Containers protections to Amazon EKS Clusters
Extend Defender for Servers protections to EC2 instances

**Assess, Secure and Defend**

Continuously Assess - Know your security posture, identify and track vulnerabilities
Secure - Harden resources and services with Microsoft cloud security benchmark (MCSB)
Defend - Detect and resolve threats to resources

![[Pasted image 20260930002345.png]]

**Continuously Assess**

Defender for Cloud vulnerability assessment for virtual machines, container registries and SQL Servers
Microsoft Defender for Servers includes automatic integration with Microsoft Defender for Endpoint. With this, you have access to findings from Microsoft Defender Vulnerability Management

Together these provide visibility across compute, data and infrastructure from a unified experience.

**Secure**

Defender for cloud builds on Azure Policy so controls can be scope at management group, subscription or tenant levels.

Defender for cloud evaluates new resources against best practices and provides recommendations. These align with Microsoft Cloud Security Benchmark (MCSB) guidance.

**Defend**

Defends by providing security alerts and advanced threat protection features.

When a threat is detected, it generates security alerts. These alerts - 

Describe details of affected resources
Suggest remediation steps
Provide option to trigger a logic app in response

It also uses kill-chain analysis to automatically correlate related alerts, helping see full story of an attack. where it started, what resources are affected and its impact. 

