- Read Replica are used for the read scalability

- Application must update the connection string to leverage the read replicas

- can be used for reporting and analytics

- in the same region, if we replicate the data from one AZ to another AZ then there is not cost

- RDS multi AZ

  - sync replication
  - one DNS name, automatically app failover to standby

- create a new database
  - db.t2.micro
  - gp2 (general purpose SSD)

## Encryption

- if master is not encrypted, then read replica can not be encrypted

## Aurora

- Aurora can have 15 read replicas, while MySQL has 5
- has high availability, 6 copies across 3 AZ
- one aurora takes writes (known as master)
- Aurora DB Cluster (shared storage volume), there is one writer endpoint and there is one writer endpoint
