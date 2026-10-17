Tags help you understand your cloud usage and helps manage costs.

other than subscriptions or resource groups for related resources. You can also use Resource Tags to organize resources.
Tags provide extra information or metadata about resources. 

![](../Static/Pasted%20image%2020260930005438.png)

- **Resource management** Tags enable you to locate and act on resources that are associated with specific workloads, environments, teams, and owners.
- **Cost management and optimization** Tags enable you to group resources so that you can report on costs, allocate internal cost centers, track budgets, and forecast estimated cost.
- **Operations management** Tags enable you to group resources according to how critical their availability is to your operations. This grouping helps you formulate service-level agreements (SLAs). An SLA is an uptime or performance guarantee between you and your users.
- **Security** Tags enable you to classify data by its security level, such as public or confidential.
- **Governance and regulatory compliance** Tags enable you to identify resources that align with governance or regulatory compliance requirements, such as ISO 27001. Tags can also be part of your standards enforcement efforts. For example, you might require that all resources be tagged with an owner or department name.
- **Workload optimization and automation** Tags can help you visualize all of the resources that participate in complex deployments. For example, you might tag a resource with its associated workload or application name and use software such as Azure DevOps to perform automated tasks on those resources.

**How to manage Resource Tags**

you can add, modify or delete resource tags through the Azure portal, PowerShell or Azure CLI, Azure Resource Manager Templates or REST API

You can use Azure Policy to enforce tagging rules and conventions. Resources don't inherit tags from subscriptions and resource groups, meaning that you can apply tags at one level and not have those tags automatically show up at a different level, allowing you to create custom tagging schemas that change depending on the level (resource, resource group, subscription, and so on).

Example - 

![](../Static/Pasted%20image%2020260930005753.png)

