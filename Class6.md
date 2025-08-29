# Date: 28/Aug/2025
# Simple Storage Service (S3) - Amazon

## Overview
- Amazon S3 is a **blob/object storage service**.
- Storage units called **Buckets** are the containers for objects (files).
- Each Bucket:
  - Belongs to a specific **AWS region**.
  - Must have a **globally unique name across AWS**.
- Buckets are used to **store and organize data**.

## Bucket Features
- Buckets allow creation of **folders** to organize objects.
- Objects are files of any type stored inside buckets or folders.
- Every object receives two types of URLs:
  - **HTTPS URL:** Accessible via web browser (if permissions allow).
  - **S3 URL:** Used to access via AWS SDK, CLI, or APIs.

## Access Control
- Buckets have **Access Control Lists (ACLs)** which manage permissions.
- By default, **block all public access** is enabled for security.
- To share an object publicly, unblock public access and grant **public read access**.
- Public objects can be accessed by anyone with the HTTPS URL.

## Example Flow
- Create a bucket with a **unique name**.
- Enable ACLs but unselect the option to block all public access.
- Upload files (objects) to the bucket.
- Grant public access for these files to make them accessible via HTTPS URL.

***

# Azure Storage Account

## Overview
- A **Storage Account** is an Azure service providing various storage types:
  - Disk storage
  - File storage
  - Blob storage
  - Archive storage
  - Table and Queue storage (for NoSQL and message queuing)

## Azure Blob Storage Types
- **Page Blob:** Used for virtual hard disk files.
- **Block Blob:** General-purpose blob for any file type (similar to AWS S3 objects).
- **Append Blob:** Designed for append operations like logging data.

## Resource Management
- Every Azure resource must belong to a **Resource Group** (a logical container).
- To store blobs, create a **container** inside a storage account.
- Containers organize blobs similar to buckets in AWS.

## Access Control in Azure Blob Storage
- By default, containers have **private access**.
- To allow public anonymous access, container access level needs to be changed.
- Example: Create a container named "shared" and configure public access if needed.

***

# Key Differences and Analogies

| Feature            | Amazon S3                          | Azure Blob Storage               |
|--------------------|----------------------------------|---------------------------------|
| Storage unit       | Bucket                           | Container                       |
| Blob types         | Object (general)                 | Block Blob, Page Blob, Append Blob |
| Access default     | Block all public access enabled   | Private by default              |
| URL for access     | HTTPS URL and S3 URL             | HTTPS URL                      |

**Analogy:** Think of an Amazon S3 Bucket or Azure Container like a big storage locker. Inside, you have files (objects/blobs). You can arrange files into folders for neatness. Lockers are private by default, but you can give a copy of your key (public access) to others if needed.

