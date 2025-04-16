# Cloud Exit: Seamless Migration from AWS to Azure

This repository provides a comprehensive guide to understanding and implementing Cloud Exit strategies. Cloud Exit refers to the process of migrating workloads, applications, and data from one cloud provider to another, or even to an on-premises environment. This guide covers key concepts, best practices, and tools to help IT professionals execute a secure, efficient, and cost-effective cloud migration.
Terraform code is included as a demonstration of the detailed steps involved in implementing a Cloud Exit strategy.


## Diagram
![Cloud Exit by Example](https://github.com/user-attachments/assets/e9f6c682-041d-4be6-8c66-ef7accc2908f)

## Scenario: Tiger Bank Cloud Exit Use Case
Tiger Bank Ltd., a financial institution, currently operates its IT systems on AWS. Concerned about rising costs and eager to leverage Azure's integration with OpenAI features for enhanced customer experience, Tiger Bank Ltd. decides to migrate its workloads and applications from AWS to Azure.

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

Below is a comparison of equivalent services between AWS and Azure to assist with the migration process:

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

#Databckup
Data backup ensures data integrity, prevents loss, and enables seamless recovery during cloud exit, reducing migration risks significantly.
Below is how Tiger bank perform on Database, S3 and VM for databackup.

#Backup Frequency:
1. Database:
   - Perform full backups at beginning and daily incremental backup to ensure data integrity.
   - Enable **Point-in-Time Recovery (PITR)** for continuous backups, allowing you to restore to any specific time within the retention period.
   - Retain backups for at least 30 days or as per compliance requirements.

2. S3 (Object Storage):
   - Use **continuous replication** for critical data to Azure Blob Storage using Azure Data Box or AWS S3 Replication.
   - Schedule weekly backups for less frequently accessed data.
   - Enable versioning in S3 to maintain historical versions of objects.

3. VM (EC2 Instances):
   - Schedule daily snapshots of EC2 instances and attached volumes to capture the VM state.
   - Retain snapshots for at least 7-14 days, depending on recovery objectives.
