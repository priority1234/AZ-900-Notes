The management infrastructure includes Azure resources and resource groups, subscriptions, and accounts. Understanding this hierarchy helps you organize resources, control who can access what, and manage costs as your Azure usage grows.

**Azure Resources and Resource Groups** -

Resource is the basic building block of Azure. Anything created, provisioned or deployed is a resource ex - VMs, virtual networks, database etc.

![](../Static/Pasted%20image%2020260922235044.png)

A resource is only associated with one group at a time.
Can't be nested.
Can't be renamed after creation.
Actions applied to a resource group affect all the resources inside it.


**Azure Subscriptions** - 

Subscriptions are a unit of management, billing and scale. It lets you organize resource groups and billing separately from access.

![](../Static/Pasted%20image%2020260922235253.png)

An azure subscription links to an Azure Account. An account can have multiple subscriptions. 

![](../Static/Pasted%20image%2020260923000654.png)

There are 2 types of Subscription Boundaries -
- **Billing boundary**: Determines how an Azure account is billed. You can create multiple subscriptions for different billing requirements. Azure generates separate billing reports and invoices for each subscription.
- **Access control boundary**: Azure applies access-management policies at the subscription level. For example, you might create one subscription for your development work and another for production, each with different spending limits and access rules.

Additional Subscriptions are used to separate - 
- **Environments**: Subscriptions for lifecycle stages such as sandbox, development, test, and production. Access control occurs at the subscription level, making this a natural boundary.
- **Team and workload boundaries**: Give each project its own subscription so costs are easy to track, or separate sandbox environments from production.
- **Billing**: Create subscriptions to track costs separately — for instance, one for production workloads and another for development and testing.

**Azure Management Groups** - 

Management Groups sit above subscriptions. Subscriptions are organized into management groups and governance policies like access or compliance rules are applied on the group.
All subscriptions within a management group automatically inherit those conditions like resources inherit settings from resource groups.

Management groups can be nested up to 6 levels deep not counting the root level. 

Every Microsoft Entra tenant has a top level Tenant Root Group. All management groups fold up to this root group, which lets you apply governance policies globally.

Important facts about management groups:

- A single directory supports up to 10,000 management groups.
- Each management group and subscription can have only one parent.

![](../Static/Pasted%20image%2020260923000747.png)

Examples of how you could use management groups:

- **Apply a policy across subscriptions**. You could limit VM locations to the US West Region in a group called Production. This policy inherits to all subscriptions under that management group and applies to all VMs in those subscriptions. The resource or subscription owner can't override it, which strengthens governance.
- **Grant access to multiple subscriptions at once**. By placing subscriptions under a management group, you can create one Azure RBAC assignment on the group. All sub-management groups, subscriptions, resource groups, and resources underneath inherit those permissions — no need to script Azure RBAC across individual subscriptions.
