# 🚀 AWS ECS Fargate Deployment with Terraform

This project demonstrates how to deploy a containerized application on **Amazon ECS (Fargate)** using **Terraform**. It provisions a scalable and secure infrastructure to run an Nginx container behind an Application Load Balancer (ALB), all managed as Infrastructure as Code.

---
### **Author**
- Paul Max Chamblain | 

[Linkedin] (https://www.linkedin.com/in/paulmchamblain/)

### Below is an image showcasing the architecture of the cloud-based application I built.

![Project Image](https://github.com/MaxCH114/terraform-aws-ecs-fargate-demo/blob/master/ecs-demo/Image/ECS.gif)

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


🌐 Internet
This is where external users (like you or your clients) initiate a request to access your app.

🧭 Application Load Balancer (ALB)
Accepts HTTP requests from the internet.

Distributes traffic to your ECS service across multiple Availability Zones (AZs).

Helps with load balancing, scaling, and high availability.

🚢 ECS Service (Fargate)
Manages running tasks (containers) within your ECS Cluster.

Uses Fargate, meaning you don’t have to provision or manage EC2 instances — it’s serverless.

Automatically places containers across available subnets.

📦 Nginx Container
Your containerized web application. In this project, you're running Nginx as a sample app.

You could replace this with any app (Node.js, Python Flask, etc.) in the future.

🌐 Public Subnets
Your ECS service and Load Balancer live in two public subnets across different Availability Zones for high availability.

These subnets are part of a custom VPC.

🏗️ VPC (Virtual Private Cloud)
Isolates your network from others on AWS.

Hosts all the resources: ECS, ALB, subnets, security groups, etc.