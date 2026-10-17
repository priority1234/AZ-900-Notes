This lets you extend your on-prem networks into Microsoft cloud over a private connection. This is called ExpressRoute Circuit. 
Each location has its own ExpressRoute Circuit.

![](../Static/Pasted%20image%2020260924235812.png)

ExpressRoute connections don't go over public internet. 

**Features and Benefits** -

- Connectivity to Microsoft cloud services across all regions in the geopolitical region.
- Global connectivity to Microsoft services across all regions with the ExpressRoute Global Reach.
- Dynamic routing between your network and Microsoft via Border Gateway Protocol (BGP).
- Built-in redundancy in every peering location for higher reliability.

ExpressRoute enables direct access to the following services in all regions:

- Microsoft Office 365
- Microsoft Dynamics 365
- Azure compute services, such as Azure Virtual Machines
- Azure cloud services, such as Azure Cosmos DB and Azure Storage

**Global Connectivity** -

You can enable ExpressRoute Global Reach to connect two or more offices by connecting their ExpressRoute Circuits. This allows communication without sending data over public internet.

**Dynamic Routing** -

Used Border Gateway Protocol (BGP) to exchange routes between on-prem networks and resources running in Azure. This enabled dynamic routing between them.

**Built in redundancy** -

Uses redundant devices to ensure high availability. Can also configure multiple circuits to complement this feature.

**Connectivity Model Options** -

Offers several options based on provider and network design. 
Provider-based connectivity
Point-to-Point Ethernet
Direct Connectivity at ExpressRoute Locations

**Use this when** -

- You need private, consistent connectivity between on-premises networks and Azure.
- Your team has strict compliance or data-transfer requirements.
- You need predictable latency and high-throughput network performance.
- You want to avoid sending critical traffic over the public internet.

**Security Consideration** -

While your data doesn't travel over public internet, DNS Queries, certificate revocation list checking and Azure Content Delivery Network request are still sent over the public internet