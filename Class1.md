# Date:19/08/2025  
### Summarizing key **storage terms**, **disk types**, **performance metrics**, and **unit conventions** in digital storage management.

## Storage Terms Explained
- **Backup**: Backups are copies of data made to recover quickly from failures or accidental loss. They are typically used for short-term recovery, and restoration is fast since the backup is designed for accessibility.
- **Archive**: Archives are long-term copies of data, often kept offsite or on slower, cost-effective storage, for disaster recovery or regulatory compliance. Restoring from archives is slower, as accessibility is less important than durability.

## Disk Types
- **HDD (Hard Disk Drive)**: Uses spinning mechanical platters to read/write data. Best for high-capacity, cost-effective storage. Suited for throughput-focused workloads.
- **SSD (Solid-State Drive)**: Uses flash memory with no moving parts. Provides fast data access and high performance, ideal for IOPS-focused workloads.

## Disk Performance Metrics
- **IOPS (Input/Output Operations Per Second)**: Measures the number of individual read/write operations a disk can handle in one second. Used primarily for SSDs, which excel in many small or random I/O tasks.
- **Throughput**: The total amount of data transferred per second, often expressed in MB/s or GB/s. Used mainly for HDDs, which are better at sustained, large data transfers.

## Unit Conventions
- Decimal (SI) Units:  
  - **KB** (Kilobyte) = $$ 1,000 $$ bytes  
  - **MB** (Megabyte) = $$ 1,000,000 $$ bytes  
  - **GB** (Gigabyte) = $$ 1,000,000,000 $$ bytes  
  - **TB** (Terabyte) = $$ 1,000,000,000,000 $$ bytes
- Binary Units:  
  - **KiB** (Kibibyte) = $$ 1,024 $$ bytes  
  - **MiB** (Mebibyte) = $$ 1,048,576 $$ bytes  
  - **GiB** (Gibibyte) = $$ 1,073,741,824 $$ bytes  
  - **TiB** (Tebibyte) = $$ 1,099,511,627,776 $$ bytes

## Summary Table

| Term      | Purpose                                | Restore Speed         | Example Use Case      |
|-----------|----------------------------------------|-----------------------|-----------------------|
| Backup    | Quick recovery from failure            | Fast           | Server crash recovery     |
| Archive   | Long-term, disaster recovery, compliance| Slow           | Offsite legal storage     |

| Disk Type | Best For            | Performance Metric | Example Unit               |
|-----------|---------------------|-------------------|----------------------------|
| HDD       | Big data, cost      | Throughput        | MB/s, GB/s          |
| SSD       | Fast access, intensive IOPS | IOPS         | Count/sec           |

