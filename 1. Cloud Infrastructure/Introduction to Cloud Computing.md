Delivery of computing services over the internet. Services like IT Infra such as Virtual Machine, Databases, storage, networking.

Allows for rapid scaling. 
On-Demand provisioning.
Offers Global outreach.


Azure VM sizes are grouped in families so you can choose a size based on workload needs.

|Family|Typical focus|Example use|
|---|---|---|
|B-series|Burstable, cost-efficient|Dev/test workloads with occasional CPU spikes|
|D-series|General purpose|Web servers, small-to-medium app servers|
|E-series|Memory optimized|In-memory databases, analytics workloads|
|F-series|Compute optimized|CPU-intensive application tiers|
|M-series|Large memory footprint|Large enterprise databases|
|L-series|Storage optimized|High-throughput storage and data processing|
|N-series|GPU enabled|AI training/inference and graphics workloads|

**Virtual Machine Options** - 

Customizable options for VMs - 
- **vCPU count**: affects compute capacity for concurrent and CPU-bound workloads.
- **RAM**: affects how much working data the VM can keep in memory.
- **Disk configuration**: affects storage capacity, IOPS, and throughput.
- **Network throughput**: affects data transfer performance in and out of the VM.
- **Premium SSD support**: indicates whether the size supports premium managed disks.
- **Hardware generation**: indicates platform generation and can affect baseline performance.

VM names also carry information - 

![Pasted image](../Static/Pasted%20image%2020260923001808.png)

You can also group VMs together. Azure can manage groupings with features like scale sets and availability sets.

**VM Scale Sets** -

This lets you create and manage groups of identical, load-balanced VMs. without this, you need to manually keep configuration consistent, monitor utilization and adjust instance counts. 
This automatically scale out or in based on demand. 
This also has load balancing.

**VM Availability Sets** -

This improves resiliency inside a region. This reduces the chance that all VMs are affected by maintenance or hardware failure.

Availability sets group VMs by:

- **Update domain**: VMs that can be rebooted together during planned maintenance.
- **Fault domain**: VMs that share a potential power or network failure point.

In regions that support Availability Zones, zone-based designs are often preferred because they provide broader failure isolation. Availability sets themselves don't add cost; you pay for the VM instances.
