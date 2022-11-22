## 280 - Organizations

- Allows to manage multiple AWS Accounts
- The main account is the management account and other accounts are member accounts
- OU (Organizational Units)
- Advantages
  - MultiAccount vs One Account MultiVPC

## 282 - IAM - Advanced Policies

- aws:SourceIp - restrict the client IP from which the API calls are being made
- aws:RequestedRegion - restrict the region the API calls are made to
- aws:ResourceTags - restrict based on tags
- aws:MultiFactorAuthPresent - to force MFA

## 283 - IAM Roles vs Resource Based Policy

- When a assume a role(user, application or service), you give up your original permission and take the permissions assigned to the role.
- When using a resource based policy, the Principal doesn't have to give up his permissions
- Amazon EventBridge
  - Resource Based Policy - Lambda, SNS, SQS, Cloudwatch Logs, API Gateway
  - IAM Role - Kinesis Stream, System Manager Run Command, ECS task
