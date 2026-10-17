It is a service that allows you to create, assign and manage policies that control or audit your resources. 
This enforces different rules across your resource configurations so that those configurations stay compliant with your standards.

![](../Static/Pasted%20image%2020260930015246.png)


It allows you to define both individual policies and groups of related policies known as initiatives.  Azure Policy evaluates your resources and highlights resources that aren't compliant with the policies you've created. Azure Policy can also prevent noncompliant resources from being created.
Can be set on resource, resource group, subscription and so on. 
Inherited from high levels to low levels.
Comes with built in policy and initiative definitions for Storage, Networking, Compute, Security Center and Monitoring
In some cases, Azure Policy can automatically remediate noncompliant resources and configurations. For example, you can require an `AppName` tag and have Azure Policy add it when missing. You still retain full control of your environment because resources can be marked as exceptions.
Azure Policy also integrates with Azure DevOps by applying any continuous integration and delivery pipeline policies that pertain to the pre-deployment and post-deployment phases of your applications.

**Policy Guardrails for AI-assisted changes**

If teams use copilot recommendations or agent-like automation, Azure policy still enforces your standards.

**Azure Policy Initiatives**

Way of grouping related policies together. 
Initiative definition contains all of the policy definitions to help track your compliance state for a larger goal.

Example - 
An initiative like Enable Monitoring in Azure Security Center. Its goal is to monitor all available security recommendations for all Azure resource types in Azure Security Center.

Under this initiative, the following policy definitions are included:

- **Monitor unencrypted SQL Database in Security Center** This policy monitors for unencrypted SQL databases and servers.
- **Monitor OS vulnerabilities in Security Center** This policy monitors servers that don't satisfy the configured OS vulnerability baseline.
- **Monitor missing Endpoint Protection in Security Center** This policy monitors for servers that don't have an installed endpoint protection agent.

