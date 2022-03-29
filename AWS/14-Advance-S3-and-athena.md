## S3 MFA Delete

- To use MFA-Delete, we need to enable S3 Versioning

## 145 - S3 Default Encryption

- one way to force encryption is to use a bucket policy and refuse any API call to put an S3 object without encryption headers
- another way is to use "default encryption"

## 146 - S3 Replication

- Cross region replication (CRR)
- Same region replication (SRR)
- Copy is asynchronous
- After activating, only new objects are replicated
- Deletion with a version ID are not replicated
