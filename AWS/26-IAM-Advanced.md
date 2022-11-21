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
