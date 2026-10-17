Supports both real time migration using Azure Migrate as well as asynchronous migration using Azure Data Box

![[Pasted image 20260928225546.png]]

**Azure Migrate** 

Service to help migrate from on-premises env to cloud. It provides the following -

Unified Migration Platform - Single portal to run, start and track your migration to Azure
Range of Tools - Tools for assessment and migration. Includes -
1. Azure Migrate: Discovery and assessment
2. Azure Migrate: Server Migration
This also integrates with other Azure services and with Independent software vendors (ISV) offerings


**Azure Data Box** 

Physical Migration Service. Quick, Inexpensive and reliable. Uses a device with maximum storage capacity of 80 terabytes. 
Device transported via a regional carrier. 
Tracked using the Data Box service in Azure Portal

Used when - 
1. When moving large data sets with limited network bandwidth
2. One time bulk migration of on-prem data to Azure
3. Periodic large data uploads in low network bandwidth situations
4. Exporting large data sets from Azure for recovery or regulatory needs.

Once the data from your import order is uploaded to Azure, the disks on the device are wiped clean in accordance with **NIST 800-88r1** standards. For an export order, the disks are erased once the device reaches the Azure datacenter.