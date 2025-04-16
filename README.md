# Cloud Exit: Learn how to migrate workloads, applications, and data seamlessly from AWS to Azure.

This repository offers a detailed guide to understanding and implementing Cloud Exit strategies. 
Cloud Exit refers to the process of migrating workloads, applications, and data from one cloud provider to another, or even to an on-premises environment
This guide covers key concepts, best practices, and tools to help IT professionals implement a secure and efficient cloud migration strategy.

Terrafrom code included as an demostrative purpose on detailed step how a cloud exit is. 


## Diagram
![Cloud Exit by Example](https://github.com/user-attachments/assets/e9f6c682-041d-4be6-8c66-ef7accc2908f)


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
| CloudWatch | Azure Monitor |
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
| Certificate Manager | Key Vault  |
| Web Application Firewall | Application Gateway |
| SNS | Event Grid |
