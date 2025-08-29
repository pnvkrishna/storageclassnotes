# Date: 26/Aug/2025
# Cloud Computing Overview

## Types of Cloud

### Public Cloud
- **Definition:** Cloud services provided by companies owning large data centers worldwide.
- **Users:** Anyone can create accounts and use cloud resources (virtual hardware, services).
- **Resources:** What users create in the cloud (e.g., virtual machines, databases).
- **Examples of Providers:**
  - Amazon Web Services (AWS)
  - Microsoft Azure
  - Google Cloud Platform (GCP)
  - Alibaba AliCloud

### Private Cloud
- **Definition:** Cloud infrastructure owned and operated by an enterprise for internal use.
- **Users:** Different Business Units (BUs) within the enterprise use private cloud resources.
- **Implementation:** Commonly built using open-source software like **OpenStack** (https://www.openstack.org/)
    - **Example:** A company hosting its own cloud instead of using public cloud vendors.

***

# Cloud Infrastructure Organization

## Regions and Availability Zones

- **Region:** A geographical data center location (e.g., Hyderabad, Mumbai, Singapore).
- Every cloud provider assigns a unique **region code** for identification.
  
  | Cloud | Example Regions               |
  |-------|------------------------------|
  | AWS   | us-east-1 (N. Virginia), ap-south-1 (Mumbai) |
  | Azure | southindia, centralindia, eastus           |

- **Availability Zones (AZs):** Separate data centers within a region, usually 30-60 km apart.
  - Provide fault isolation and high availability.
  - Users can deploy resources across AZs to ensure resilience.

- **Region Pairs (Azure Specific):** Some providers, like Azure, pair regions for disaster recovery.

***

# Cloud Storage Basics

## Virtual Storage in Cloud

- Cloud storage appears virtually infinite to users (especially blob storage).
- Individual blob file size limits exist (e.g., ~5 TB max per file).

## Blob Storage Explained

- **Blob Storage:** Object storage accessed over URLs without a traditional filesystem.
- **How it works:** Each file is stored as a unique "blob" or binary large object.
  
### Examples of Blob Storage Services
- **AWS:** Amazon S3 (Simple Storage Service)
- **Azure:** Azure Storage Account

### Pricing Model
- Storage cost and access cost are separate.
  - Some storage types:  
    - **Cheap storage cost but high access cost** (good for archived data rarely accessed).  
    - **High storage cost but cheap access cost** (good for frequently accessed data).

### Key Characteristics
- Blob names must be unique across the entire service (similar to a unique URL).
- Blob storage is ideal for large-scale unstructured data like videos, images, backups.

***

# Real-World Analogies

- Think of **Public Cloud** as renting an apartment in a big building where many tenants share resources.
- **Private Cloud** is like owning your own house where just your family lives and manages everything.
- **Blob Storage** is like storing files in a massive online locker, accessed with a unique URL—you don’t worry about organizing files into folders.
- **Availability Zones** are like multiple branches of a bank in a city; if one branch closes, you can still access your money at another branch nearby.


# Note: 
- **Resilience** in cloud computing means the ability of a cloud system, application, or service to resist, withstand, and quickly recover from disruptions or failures. These disruptions could be due to hardware failures, power outages, network issues, cyberattacks, or even natural disasters.
    - Key points about resilience:
      - It is not about avoiding failure completely (failures are inevitable), but about minimizing    downtime and impact during failures.
      - In simple terms, resilience means the cloud system can bounce back and keep running smoothly despite problems.

