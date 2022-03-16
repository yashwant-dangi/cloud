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
