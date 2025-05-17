# WordPress Deployment on AWS with Disaster Recovery

This project demonstrates how to deploy a **WordPress application** on **AWS infrastructure** using a scalable and secure architecture. It includes a disaster recovery (DR) strategy to ensure high availability and data protection.

## Tools & Services Used

- **EC2** – For hosting WordPress with Apache HTTPD
- **RDS (MySQL)** – Managed database service
- **S3** – Static content storage and backup
- **IAM** – Secure access management
- **Route 53** – Domain registration and routing
- **Elastic Load Balancer (ELB)** – Distributes incoming traffic
- **AWS Certificate Manager** – Provides SSL certificates for HTTPS
- **CloudWatch** – Basic monitoring and logs
- **VPC, Subnets, Security Groups** – Network configuration

## Architecture Overview

- Apache Web Server runs WordPress on EC2
- MySQL runs on Amazon RDS (multi-AZ enabled)
- S3 bucket stores media and backups
- Route 53 routes DNS requests to the ELB
- SSL certificate is used to enable HTTPS access
- Backups are automated and stored securely

## Key Features

- **Scalable Setup** – Separate components for web, DB, and storage
- **DR Strategy** – Backup & restore approach using automated snapshots
- **Security** – IAM roles, Security Groups, HTTPS enabled
- **Monitoring** – CloudWatch metrics and logs for EC2 and RDS

## Outcomes

- Learned how to use AWS to deploy a multi-tier web application
- Implemented a basic DR plan with backups
- Gained experience in configuring Route 53 and SSL

## Future Improvements

- Automate infrastructure using **Terraform**
- Add auto scaling group for EC2
- Use CloudFront for CDN

---

