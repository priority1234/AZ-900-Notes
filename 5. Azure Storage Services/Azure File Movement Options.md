Azure has tools to move or interact with individual files or small file groups.
Tools like AzCopy, Azure Storage Explorer, Azure File Sync
![[Pasted image 20260928230518.png]]

**AzCopy**

Command line utility that you can use to copy blobs or files to or from your storage account. You can upload files, download files, copy files b/w storage accounts and event synchronize files. 
Can be configured to work with other cloud providers to help move files back and forth b/w clouds.
Synchronizing files with AzCopy is one direction sync. When you sync, you designate the source and destination and AzCopy will copy files or blobs in that direction. It doesn't sync bi-directionally based on timestamps or other metadata.

**Azure Storage Explorer**

App with GUI to manage files or blobs in Azure Storage Account. Uses AzCopy in backend. 

**Azure File Sync** 

Tool to centralize file shares in Azure Files and keep flexibility, performance and compatibility like a Windows File Server. It automatically bi-directionally syncs files with Azure. 

Features - 
1. Use any protocol available on Windows Server to access data locally like SMB, NFS and FTPS
2. have as many caches as you need across the world
3. Replace a failed local server by installing Azure File Sync on a  new server in the same datacenter.
4. Configure cloud tiering so most frequently accessed files are replicated locally while infrequently are kept in cloud until requested.