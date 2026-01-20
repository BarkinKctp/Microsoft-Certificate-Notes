# Azure Storage and Data

## Azure Blob Storage
Azure Blob Storage is an object storage solution that you can use to store massive amounts of unstructured data, such as text or binary data.

### Data Tiers (Blob Storage)
- **Archive Tier**  
  Stores data offline and offers the lowest storage costs, but has the highest costs to rehydrate and access data.

- **Hot Tier**  
  Optimized for storing data that is accessed frequently.

- **Cool Tier**  
  Data in the Cool access tier can tolerate slightly lower availability, but still requires high durability, retrieval latency, and throughput characteristics similar to hot data.

Low storage costs and unlimited file formats make Blob Storage a good location to store backups and archives.  
Blob Storage can be reached from anywhere by using an internet connection.

---

## Azure Disk Storage
Azure Disk Storage provides disks for Azure virtual machines.

---

## Azure Files
Azure Files supports mounting file storage shares.
