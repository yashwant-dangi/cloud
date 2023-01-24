# 291 - Encrypted AMI sharing process

- AMI in source account is encrypted with KMS key
- Must modify the image attribute to add a launch permission which corresponds to the specific target AWS account
- Must share the KMS keys used to encrypt the snapshot the AMI references with the target account

## 292 - SSN Parameter store

- Secure storate for configuration and secrets
- Optional Seamless Encryption with KMS

## 298 - AWS Secrets Manager

- Newer service, meant for storing secret
- Capability to force rotation of secrets every X days

## 300 - AWS Certificate Manager (ACM)

- Easily provision, manage and deploy TLS certificate
- Integrations with
  - Elastic Load Balancer
  - CloudFront Distributions
  - APIs on API Gateway

## 301 - Web Application Firewall (WAF)

- Protects web application from common web exploits (Layer 7)
- Layer 7 is HTTP (vs Layer 4 is TCP/UDP)
- Deploy on
  - Application Load Balancer
  - API gateway
  - Cloudfront
  - AppSync GraphQL API
  - Cognito User Pool
- Define Web ACL Rules using IP Set, HTTP Header, size constraints or rate-based rules
- To Achieve fixed IP with the WAF, we can use Global Accelerator and WAF on the ALB

## 302 - Shield - DDoS Attack

- Provides protection from attacks such as SYN/UDP floods, Reflection attacks and other layer 3/layer 4 attacks

## 303 - Firewall Manager

- Manages all security rules at one place
  - WAF rules, AWS sheild Advanced
  - Security Group for EC2, ALB and ENI resources on VPC
  - AWS Network Firewall
  - Route 53 Resolver
