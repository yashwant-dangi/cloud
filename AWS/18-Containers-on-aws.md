## Amazon ECR

- Amazon Elastic Container Registry
- Store and manage docker images on AWS
- To host private Registry

## Amazon ECS

- Amazon Elastic Container Service
- Container platform

## Amazon EKS

- Amazon Elastic Kubernetes Service
- Amazon managed Kubernetes
- 2 modes
  EC2 mode - if you want to deploy worker nodes
  Fargate mode - if you want to deploy serverless containers
- Node types
  Managed node groups - creates and manages nodes for you, Nodes are part of ASG (auto scaling group) managed by EKS
  Self Managed - Nodes created by you and registered to the EKS cluster
  Fargate - No maintance required

## AWS Fargate

- Amazon's own Serverless Container Platform
