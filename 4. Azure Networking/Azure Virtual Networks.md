Azure Virtual networks and Virtual Subnets allow Azure resources like VMs, Web Apps etc to communicate with each other, with users on internet and with on-prem computers.

Azure virtual networks provide the following key networking capabilities:

- Isolation and segmentation
- Internet communications
- Communicate between Azure resources
- Communicate with on-premises resources
- Route network traffic
- Filter network traffic
- Connect virtual networks

Supports both private and public endpoints for communication with internal or external resources.

- Public endpoints have a public IP address and can be accessed from anywhere in the world.
- Private endpoints exist within a virtual network and have a private IP address from within the address space of that virtual network.

**Isolation and Segmentation** -

Azure lets you create multiple isolated virtual networks. To set up, a private IP address space is defined by using a public or private address ranges.
This IP range is not internet routable. 
You can allocate part of the IP address space into subnets. 

**Internet Communications** -

Can enable incoming connections from internet by assigning a public IP address to an Azure resource. Or put the resource behind a public load balancer.

**Communication between Azure Resources** -

Azure resources communicate with each other through -

- Virtual networks can connect not only VMs but other Azure resources, such as the App Service Environment for Power Apps, Azure Kubernetes Service, and Azure virtual machine scale sets.
- Service endpoints can connect to other Azure resource types, such as Azure SQL databases and storage accounts. This approach lets you link multiple Azure resources to virtual networks to improve security and provide optimal routing between resources.

**Communicate with on-prem resources** -

3 ways to achieve this connectivity 

- Point-to-site virtual private network connections are from a computer outside your environment back into your private network. In this case, the client computer initiates an encrypted VPN connection to connect to the Azure virtual network.
- Site-to-site virtual private networks link your on-premises VPN device or gateway to the Azure VPN gateway in a virtual network. In effect, the devices in Azure can appear as being on the local network. The connection is encrypted and works over the internet.
- Azure ExpressRoute provides a dedicated private connectivity to Azure that doesn't travel over the internet. ExpressRoute is useful for environments where you need greater bandwidth and even higher levels of security.

**Route Network Traffic** -

- Route tables let you define rules about how traffic should be directed. You can create custom route tables that control how packets are routed between subnets.
- Border Gateway Protocol (BGP) works with Azure VPN gateways, Azure Route Server, or Azure ExpressRoute to propagate on-premises BGP routes to Azure virtual networks.
- User-defined routes (UDR) let you control the routing tables between subnets within a virtual network or between virtual networks, giving you greater control over network traffic flow.

**Filter Network Traffic** -

- Network security groups are Azure resources that can contain multiple inbound and outbound security rules. You can define these rules to allow or block traffic, based on factors such as source and destination IP address, port, and protocol.
- Network virtual appliances are specialized VMs that can be compared to a hardened network appliance. A network virtual appliance carries out a particular network function, such as running a firewall or performing wide area network (WAN) optimization.
![](../Static/Pasted%20image%2020260924234042.png)

**Connect Virtual Networks** -

Can link virtual networks together by using virtual network peering. Allows 2 virtual networks to connect directly. Network traffic is private and travels on Microsoft network, never on public network. 
These VNets can be in separate regions, which lets you create a global interconnected network through Azure.

![](../Static/Pasted%20image%2020260924234259.png)


