Azure uses pay as you go model. 
Rent what's needed and release when done.
Consumption scales with actual usage.

![[Pasted image 20260930003253.png]]

**Resource Type**

Type of resource, settings, Azure Region all have an impact on this. 
When you provision a resource, Azure tracks how much of each resource you use.

Example - 

In a storage account, you choose type of data like blob. How fast you need to access. How many copies to keep. Which region to use. 
With VMs, you have to consider licensing cost for OS, software, processor, no of cores, attached storage, network interface, region etc.

**Consumption**

Pay-as-you-go model. 
Azure also offers discount options for predictable workloads. 
With Reservations, you can commit to specific resources for one or three year terms to reduce cost. Applies to resources like DB, VMs, Storage.

For flexibility in which compute resources you use, Azure savings plan for compute is also an option. You commit to an hourly spend amount on eligible compute services for one or three years and azure applies best available price as usage occurs.
For workload that can handle interruptions, Azure Spot Virtual Machines can reduce cost. It uses unused Azure capacity at lower prices, but those resources are evicted when azure needs them.

![[Pasted image 20260930003800.png]]


**Maintenance**

Every time you provision a VM, additional resources such as networking and storage are also provisioned, but when you deprovision it, those resources might not deprovision at same time. 
Keeping an eye on your resources and making sure you're not keeping resources you don't need.

**Geography**

Azure infra is distributed globally, this causes global pricing differences. 
Network traffic is also impacted based on geography. Ex - it's less expensive to move information within Europe than to move information from Europe to Asia or South Africa

**Network Traffic**

Billing zones also determine the cost of some Azure Services. Billing zones are geographical grouping of Azure Regions used specifically for data-transfer pricing.
Bandwidth refers to data moving in and out of Azure datacenters. Some inbound data transfers are free. Outbound data transfer pricing are based on zones.

**Subscription Type**

Subscriptions also include allowances.

**Azure Marketplace**

It lets you purchase Azure based solutions and services from third party vendors. This includes preconfigured web server, a VM with specialized software already installed etc. 
When purchasing products through this, you may pay for both the Azure services and The expertise of the third party.
All solutions in Marketplace are certified and compliant with Azure policies and standards.

