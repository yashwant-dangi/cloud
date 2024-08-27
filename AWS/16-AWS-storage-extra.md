## Amazon FSx

- Launch 3rd party high performance file system on AWS

## Storage Gateway - 176

- Block level storage like EBS and EC2 instance store
- File level storage like EFS and FSx
- Object level storage like S3 and Glacier

- file gateway - accessible using NFS and SMB protocol

## 179 - AWS DataSync

- Move large amount of data to and from
  on Premises/ other cloud to AWS (agent needed)
  AWS to AWS (no agent needed)
- replication task can be scheduled hourly, daily and weekly
- File permission and metadata are reserved
  example is NFS/SMB to AWS (S3, EFS, FSx)
- AWS snowcone can also be used

## 180 - Storage Options Compared

- S3: Object Storage
- S3 Glacier: Object Archival
- EBS Volumes: Network storage for one EC2 instance at a time
- Instance Storage: Physical storage for your EC2 instance (high IOPS)
- EFS: Network file system for linux instances
- FSx for Windows: Network file system for windows servers
- FSx for Lustre: High Performance computing Linux file system
