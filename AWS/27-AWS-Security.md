# 291 - Encrypted AMI sharing process

- AMI in source account is encrypted with KMS key
- Must modify the image attribute to add a launch permission which corresponds to the specific target AWS account
- Must share the KMS keys used to encrypt the snapshot the AMI references with the target account

## 292 - SSN Parameter store

- Secure storate for configuration and secrets
- Optional Seamless Encryption with KMS
