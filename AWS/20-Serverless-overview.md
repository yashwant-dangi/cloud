## 219 - DynamoDB Advance Features

### DAX - DynamoBB Accelerator

- Fully Managed, highly available, seamless in-memory cache for DynamoDB
- Solve read congestion by caching
- TTL of 5 min (can be changed)
- its different from ElastiCache, DAX is specially designed for DynamoDB

### DynamoDB Stream Processing

- Ordered stream of item-level modifications (create/update/delete) in a table
- Use Case:
  - React to changes on real-time
  - Invoke AWS Lambda on changes to your DynamoDB Table

### DynamoDB TTL

- Automatically delete items after an expiry timestamp
- Use cases are adhere to regulatory obligations, web session handling

### Backups for disaster recovery

- Continuous backups using point-in-time recovery
