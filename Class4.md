# Date: 25/Aug/2025
## Concise notes on **cloud storage needs**, **disk storage types**, and **how hard disks work on Linux** and **Windows**, suitable for interview preparation.

## Cloud Storage Needs

### Blob Storage
- Blob storage is a type of object storage without traditional filesystems, accessible over HTTP/S protocols.
- Files are stored as objects called blobs (Binary Large Objects), enabling easy scalability and accessibility.
- AWS S3 (Simple Storage Service) is a leading example of blob storage used widely for storing unstructured data like images, videos, backups, and logs.

### Disk Storage
- Traditional block storage that behaves like a physical disk, can be attached to cloud virtual machines for OS and application storage.
- Provides consistent low-latency access and supports file systems and partitions.

### File Shares / Network Drives
- File-level storage accessible over a network using protocols like SMB or NFS.
- Useful for shared storage scenarios and collaboration in cloud or on-prem environments.

### Data Lakes
- Large centralized repositories that store structured and unstructured data at any scale.
- Typically use object/blob storage at the backend with added indexing and querying capabilities for analytics.

## How Hard Disks Work on Linux

- Linux supports multiple file systems; popular ones include:  
  - **ext4**: Default and stable ext filesystem widely used for general purposes.  
  - **XFS**: High-performance journaling filesystem, good for large files and parallel I/O.  
  - **ZFS**: Advanced filesystem with built-in volume management, snapshots, and data integrity features.  
  - **Btrfs**: Modern filesystem supporting snapshots, checksums, and pooling features.

- Physical disks can be partitioned into multiple segments.
- Each partition is formatted with a filesystem and then mounted to a directory path, making the storage accessible at that mount point.

## How Hard Disks Work on Windows

- Windows mainly supports the **NTFS** filesystem, which offers journaling, security permissions, and reliability features.
- Disks can be partitioned into multiple volumes, each assigned a drive letter (e.g., C:, D:) for access.
- Network file shares are common for file-level access, often using SMB protocol.

## Summary for Interviews

| Topic                | Key Points                                                                      |
|----------------------|--------------------------------------------------------------------------------|
| Blob Storage         | Object storage, HTTP/S access, files as blobs, e.g., AWS S3                     |
| Disk Storage         | Block storage with filesystems, low latency, VM disk attachment                |
| File Shares          | Network-based shared storage using SMB/NFS                                    |
| Linux Filesystems    | ext4, XFS, ZFS, Btrfs; disks partitioned, formatted, and mounted               |
| Windows Filesystems  | NTFS primarily; disks partitioned into volumes with drive letters              |
| Network Shares       | SMB protocol for shared file access                                            |



## Note: 
Here are clear explanations of the terms:

## Consistent Low-Latency Access
- This means the storage system delivers data access with minimal and predictable delay every time a request is made.
- "Low latency" refers to the short time it takes for a read or write operation to start and complete.
- "Consistent" implies that latency does not vary widely between requests, ensuring reliable and smooth application performance.
- This is critical for applications needing real-time or near real-time data access, such as databases and virtual machines.

## SMB (Server Message Block)
- SMB is a network protocol used for sharing files, printers, and other resources across a network.
- It enables computers to access files or devices on remote servers as if they were local.
- SMB is commonly used in Windows environments for network file sharing (e.g., accessing shared folders or drives).
- It works over TCP/IP and supports features like authentication, access control, and file locking to manage concurrent access.



