| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Data is divided into fixed-size blocks, with each block having its own identifier. It is provided to a VM as a raw storage volume, while the operating system manages the file system and formatting. | Boot drives and high-performance workloads such as transactional databases that require fast and low-latency read/write operations | Amazon EBS, Azure Disk Storage, Google Persistent Disk |
| File Storage | Data is organized as files within folders and directories. It can be accessed over a network using protocols such as NFS or SMB. | Shared storage that can be accessed by multiple users or VMs, such as applications that require a common network drive | Amazon EFS, Azure Files, Google Cloud Filestore |
| Object Storage | Data is stored as individual objects inside a bucket. Each object includes its data, metadata, and a unique identifier, and can be accessed through HTTP/HTTPS and APIs such as S3. | Managing large amounts of unstructured data such as images, videos, backups, and archived files | Amazon S3, Azure Blob Storage, Google Cloud Storage |

Why Object Storage Is Best for the Client's Photos
For a photo-sharing application that may receive millions of uploaded
images, Object Storage is the most suitable option. It can handle large
amounts of unstructured data without relying on complicated folder
structures or file locking. Unlike block storage, which is mainly designed
for fast and structured workloads, Object Storage can scale to very large
amounts of data such as photos and other media files.
Object Storage can also be accessed through HTTP/HTTPS and simple APIs,
which makes it easier to connect with a web application. It is also a
practical and cost-effective option for storing large collections of
photos that do not change frequently.
