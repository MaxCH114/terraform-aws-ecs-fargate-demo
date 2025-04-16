# 🚀 AWS ECS Fargate Deployment with Terraform

This project demonstrates how to deploy a containerized application on **Amazon ECS (Fargate)** using **Terraform**. It provisions a scalable and secure infrastructure to run an Nginx container behind an Application Load Balancer (ALB), all managed as Infrastructure as Code.

---

## 📦 Features

- ✅ ECS Cluster (Fargate)
- ✅ Nginx container via ECS Task Definition
- ✅ Application Load Balancer (ALB)
- ✅ VPC with public subnets (using Terraform AWS VPC Module)
- ✅ Security Group for HTTP access
- ✅ Fully automated with Terraform

---

## 📁 Project Structure

 ├── main.tf # Main Terraform configuration ├── variables.tf # Variable definitions (optional) ├── outputs.tf # Output values ├── README.md 

