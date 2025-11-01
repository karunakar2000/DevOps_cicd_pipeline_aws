# Multi-Stage CI/CD Pipeline using Jenkins, Terraform, Ansible & AWS:-

# Overview
This project demonstrates a full end-to-end CI/CD workflow that provisions infrastructure on AWS, builds and deploys a sample web application, and manages configuration using Ansible — all orchestrated via Jenkins.

It reflects a real-world DevOps setup integrating Infrastructure-as-Code (IaC), configuration management, and continuous delivery.

---------------------------------------

# Architecture
**Tools & Technologies**
- **AWS** – EC2, VPC, S3, IAM, Security Groups  
- **Terraform** – Infrastructure provisioning  
- **Packer** – AMI creation with pre-installed dependencies  
- **Ansible** – Configuration management & deployment  
- **Jenkins** – CI/CD pipeline orchestration  
- **GitHub** – Source-code & pipeline storage  
- **Docker** – Jenkins agents & build containers  

**Workflow**:-
1. Developer pushes code to GitHub.  
2. Jenkins (webhook-triggered) starts the pipeline.  
3. Terraform provisions AWS resources (VPC, EC2).  
4. Packer builds AMIs used by Terraform.  
5. Ansible configures instances & deploys app.  
6. Jenkins verifies deployment and sends build summary.

-------------------------------------

# Pipeline Stages
1. **Checkout Code (GitHub)**  
2. **Build Application (Docker)**  
3. **Provision Infrastructure (Terraform)**  
4. **Configure Servers (Ansible)**  
5. **Deploy Web App (Ansible)**  
6. **Notify & Cleanup**

----------------------------

# Folder Structure
