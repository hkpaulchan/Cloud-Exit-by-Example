# Cloud-Exit-by-Example
Cloud Exit: Learn how to migrate workloads, applications, and data seamlessly from AWS to Azure. This guide covers key concepts, best practices, and tools to help IT professionals implement a secure and efficient cloud exit strategy

# Azure and AWS Infrastructure for Webapp with CI/CD

Infrastructure as Code for both Amazon Web Services and Microsoft Azure written in Terraform. 
```

## Terraform Structure

According to best practices, the terraform structure is as follows:
```
├── environments
│   ├── dev
│   │   ├── main.tf
│   │   ├── terraform-dev.tfvars
│   │   └── variables.tf
│   ├── prod
│   │   ├── main.tf
│   │   ├── terraform-prod.tfvars
│   │   └── variables.tf
│   └── readme.md
├── modules
│   └── {LIST_OF_ALL_MODULES}
└── Readme.md
```


# AWS to Azure Migration Services 

| AWS | AZURE |
| --- | --- |
| Virtual Private Cloud (VPC) | Virtual Network (VNET) |
| Accounts | Subscriptions |
| CloudWatch | Monitor |
| CloudFront | Content Delivery Network |
| Route 53 | DNS |
| Codedeploy | Azure DevOps |
| EC2 | VM |
| Application Load Balancer | Application Gateway |
| Auto Scaling | Virtual Machine Scale Sets |
| S3 | Blob storage |
| RDS | Database for MySQL | 
| DynamoDB | Cosmos DB |
| Lambda | Functions |
| Certificate Manager | Key Vaults  |
| Web Application Firewall | Application Gateway |
| SNS | Event Grid |
