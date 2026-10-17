Azure architecture can be broken down into 2 groups - Physical infrastructure and management infrastructure. 

**Physical Infrastructure** - 

Datacenters are facilities where servers arranged in racks with dedicated power, cooling and networking infra. Same as on prem datacenter but on a much larger scale.

Datacenters are grouped into Azure regions and Azure Availability zones.

![](../Static/Pasted%20image%2020260922233842.png)


**Regions** - 

A region is an area on the planet that contains at least one datacenter that are nearby and networked together with a low latency network. 
When deploying resources, you need to choose a region where the resource will be deployed.

**Availablity Zones** - 

Availability zones are physically separate datacenters within an azure region. it is set up to be an isolation boundary. If one zone goes down, the other keeps working. Connected through high speed, private fiber optic networks.

![](../Static/Pasted%20image%2020260922234137.png)

Azure services that support availability zones fall into three categories:

- Zonal services: You pin the resource to a specific zone (for example, VMs, managed disks, IP addresses).
- Zone-redundant services: The platform replicates automatically across zones (for example, zone-redundant storage, SQL Database).
- Non-regional services: Services are always available from Azure geographies and are resilient to zone-wide outages as well as region-wide outages.

![](../Static/Pasted%20image%2020260922234258.png)


**Region Pairs** - 

Most Azure Regions are paired with another region within the same geography at least 300 miles away. This allows replication of resources across geography while reducing the likelihood of interruptions due to disasters etc.
For example, if a region in a pair was affected by a natural disaster, services would automatically fail over to the other region in its region pair.
Examples of region pairs in Azure are West US paired with East US and Southeast Asia paired with East Asia.

![](../Static/Pasted%20image%2020260922234447.png)


#### Additional advantages of region pairs:

- If an extensive Azure outage occurs, one region out of every pair is prioritized to make sure at least one is restored as quickly as possible for applications hosted in that region pair.
- Planned Azure updates are rolled out to paired regions one region at a time to minimize downtime and risk of application outage.
- Data continues to reside within the same geography as its pair (except for Brazil South) for data-residency and compliance purposes.

**Note** - Most regions are paired in two directions, meaning they are the backup for the region that provides a backup for them (West US and East US back each other up). However, some regions, such as Brazil South, are paired in only one direction. In a one-direction pairing, the Primary region does not provide backup for its secondary region. Brazil South is unique because it's paired with a region outside of its geography. Brazil South's secondary region is South Central US. The secondary region of South Central US isn't Brazil South. Additionally, some regions (such as Italy North, Poland Central, and Israel Central) don't have a traditional region pair and instead rely on availability zones and geo-redundant storage for resiliency.


**Sovereign Regions** - 

Sovereign regions are instances that are isolated from main instance of Azure. Used for legal or compliance purpose.
Examples -

- US DoD Central, US Gov Virginia, US Gov Arizona, and more: These regions are physical and logical network-isolated instances of Azure for U.S. government agencies and partners. These datacenters are operated by screened U.S. personnel and include additional compliance certifications.
- China East, China North, and more: These regions are available through a unique partnership between Microsoft and 21Vianet, whereby Microsoft doesn't directly maintain the datacenters.



