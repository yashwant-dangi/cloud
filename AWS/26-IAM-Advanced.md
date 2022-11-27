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

## 285 - Cognito

- Give users an identity to interact with our web or mobile application
- Cognito User Pools (CUP)
  - Sign in functionality for all users
  - Integrate with API gateway and Application Load Balancer
- Cognito Identity Pools (Federated Identity)
  - Provide AWS Credentials to users so they can access AWS Resources directly

## 286 - AWS IAM Identity Center

- One Login for all your
  - AWS accounts in AWS Organizations
  - Business cloud applications
  - SAML 2.0 enabled applications

## 287 - AWS Directory Services

- Create Your own AD in AWS
- Establish "trush" connections with your on-premise AD

## 288 - AWS Control Tower

- Easy way to set up and govern a secure and compliant multi-account AWS environment based on best practices
- Benefits
  - Automate the set up of your env in few clicks
  - Automate ongoing policy management using guardrails
  - defect policy violations and remediate them
  - Moniter compliance through an interactive dashboard
