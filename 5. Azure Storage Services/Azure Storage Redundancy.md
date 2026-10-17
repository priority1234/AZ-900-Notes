Keeps multiple copies of data. 

**Redundancy in primary region** -
Data in Azure Storage is replicated 3 times in primary region. Primary region options are locally redundant storage (LRS) and zone redundant storage (ZRS)

Locally Redundant Storage(LRS) - 

Replicates data 3 times in a single data center in primary region. provides 11 nines of durability.
Lowest cost option. Protects against failure in one datacenter. Although a datacenter level disaster can still cause data loss.

Zone Redundant Storage(ZRS) -

Replicates data synchronously across 3 Azure Availability zones in the primary region. Offers 12 nines of durability.
Data is available for read/write even if one zone is unavailable. 

**Redundancy in a secondary region** - 

For more durability, you can replicate data to a secondary region that is distant from primary. Replicated Asynchronously.

Azure assigns secondary region based on region pairs.

Secondary region options are geo-redundant storage(GRS) and get-zone-redundant storage(GZRS). GRS uses LRS in both regions. while GZRS uses ZRS in primary region and LRS in secondary region.

Secondary region data isn't readable unless failover occurs. 

Geo-redundant Storage(GRS) -

copies data synchronously 3 times in primary region(LRS), then asynchronously to the secondary region (LRS). provides 16 nines of durability.

![[Pasted image 20260925003335.png]]

Geo-zone-redundant storage -

GZRS combines zone-level resilience in primary region with geo-replication to a secondary region. Data is copied across 3 zones in primary region and then to the Secondary region using LRS. 16 nines of durability.

![[Pasted image 20260925003508.png]]


**Read access to data in Secondary region** -

To read secondary-region data before failover, enable read-access GRS or read-access GZRS

**Note** - The data in secondary region may not be up to date because of RPO.
Because data is replicated to the secondary region asynchronously, a failure that affects the primary region may result in data loss if the primary region can't be recovered. The interval between the most recent writes to the primary region and the last write to the secondary region is known as the recovery point objective (RPO). The RPO indicates the point in time to which data can be recovered. Azure Storage typically has an RPO of less than 15 minutes, although there's currently no SLA on how long it takes to replicate data to the secondary region.