# Azure_Learning_Basics


| Azure Blobs | Azure Files | Azure Disks |
|----------|----------|----------|
| Object Storage | Files | Disk |
| Containers and Folder | Folder(Files) | Virtual Hard Disk |

### Account Type:

| Standard | Premium | 
|----------|----------|
| Containers<br>File Share<br>Tables<br>Queue | Specified Storage |

#### Premium Account Type :

| Page Blobs | Block Blobs | Append Blobs | File Share |
|----------|----------|----------|----------|
| OS/Virtual Hard Disk | Object Stoage (High performance) | Log , Evnets | Files Only (High Performance) |

#### Replication :
- 1.LRS

![LRS](https://learn.microsoft.com/en-us/azure/storage/common/media/storage-redundancy/locally-redundant-storage.png)
- 2.ZRS

![ZRS](https://learn.microsoft.com/en-us/azure/storage/common/media/storage-redundancy/zone-redundant-storage.png)
- 3.GRS 

![GRS]()
- 4.RA-GRS

![RA-GRS](https://learn.microsoft.com/en-us/azure/storage/common/media/storage-redundancy/geo-redundant-storage.png)
- 5.RA-GZRS

![RA-GZRS](https://learn.microsoft.com/en-us/azure/storage/common/media/storage-redundancy/geo-zone-redundant-storage.png)

| Performance | Account Type | Replication|
|----------|----------|----------|
| Standard |  | |
| Premium | Block Blob | LRS / ZRS |
| |File Share | LRS / ZRS |
| |Page Blob| LRS |

###### Standard
- Can be changed LRS to ZRS , GRS after created
- Cannot be changed performance type after created
###### Premium 
- Cannot be changed replication type and performnce type after created

