Core data services are - 
![](../Static/Pasted%20image%2020260925003922.png)


**Benefits of Azure Storage**

Durable and Highly Available
Secure
Scalable
Managed - azure manages updates and maintenance for you
Accessible - can be accessed from anywhere using HTTP or HTTPS 

**Azure Blobs** -

**Storage Tiers -** 

Hot Access Tier - For data that is accessed frequently
Cool Access Tier - For data that is accessed infrequently and stored for at least 30 days
Cold Access Tier -  For data that is accessed infrequently and stored for at least 90 days
Archive Access Tier - For data rarely accessed. Stored for at least 180 days.

![](../Static/Pasted%20image%2020260928224926.png)

**Azure Files** 

Azure Files offer fully managed file shares in cloud that are accessed via Server Message Block (SMB) or Network File System (NFS) protocols. 
SMB for Windows, Linux and MacOs
NFS for Linux and MacOS
SMB can be cached on windows servers for fast access.

**Benefits of Azure Files** -

Shared Access
Fully Managed
Scripting and Tooling - Manage shares with Azure CLI, PowerShell, Azure Portal or Storage Explorer
Resilience - High Availability
Familiar Programmability - Applications can use standard I/O APIs plus Azure SDKs and REST APIs


**Azure Queues**

Stores large number of messages for asynchronous processing. Queues are accessed by HTTP/HTTPS calls. supports messages up to 64 KB.

**Azure Disks**

Provides block-level volumes for Azure VMs. Virtualized and managed by Azure

**Azure Tables**

NoSQL store for large amounts of structured, non-relational data. 


