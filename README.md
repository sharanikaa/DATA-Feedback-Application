# DATA Feedback Application using AWS Hybrid Architecture, High Availability and CI/CD Pipeline

A scalable, highly available web application built on AWS for collecting feedback from members and participants of the **DATA (Data Science and Artificial Intelligence Technical Association)**. The application combines traditional server-based infrastructure with modern serverless services to provide a secure, reliable, and highly available feedback management system with optional image uploads and automated deployment using a complete CI/CD pipeline.

## 🏗️ Architecture Overview

This project demonstrates a **hybrid cloud architecture** by integrating traditional infrastructure with serverless AWS services.

### Traditional Infrastructure
- Amazon EC2 Instances
- Auto Scaling Groups
- Application Load Balancer (ALB)

### Serverless Components
- AWS Lambda
- Amazon API Gateway
- Amazon DynamoDB

### Storage
- Amazon S3 for storing uploaded event images

### DevOps Pipeline
- Automated CI/CD using AWS CodeCommit, CodeDeploy, and CodePipeline

## 🏛️ Architecture Diagram

![Architecture](/architecture.png)

- **Frontend:** Static web application hosted on EC2 instances
- **Load Balancing:** Application Load Balancer for high availability
- **Backend API:** Serverless API using API Gateway and Lambda
- **Data Layer:** DynamoDB for structured data, S3 for image storage

## 🚀 Features

- **High Availability:** Multi-AZ deployment with Auto Scaling.
- **Hybrid Architecture:** EC2-based frontend with a serverless backend.
- **Event Feedback:** Collects feedback for DATA club events.
- **Image Upload:** Secure image storage in Amazon S3.
- **Data Persistence:** Feedback stored in Amazon DynamoDB.
- **Automated Deployment:** End-to-end CI/CD pipeline.
- **Network Security:** Custom VPC with public/private subnets.
- **Health Monitoring:** CloudWatch metrics and SNS notifications.

## 🛠️ Technology Stack

### AWS Services

- **Compute:** Amazon EC2, AWS Lambda, Auto Scaling Groups
- **Networking:** Amazon VPC, Application Load Balancer, NAT Gateway, Internet Gateway
- **Storage:** Amazon S3, Amazon DynamoDB
- **API:** Amazon API Gateway
- **DevOps:** AWS CodeCommit, AWS CodeDeploy, AWS CodePipeline, AWS CloudShell
- **Monitoring:** Amazon CloudWatch, Amazon SNS
- **Security:** IAM Roles, Security Groups

### Development Stack

- **Frontend:** HTML5, CSS3, JavaScript
- **Backend:** Python 3.9 (AWS Lambda)
- **Version Control:** Git, GitHub
- **Deployment:** AWS CodePipeline, AWS CodeDeploy

## 📋 Prerequisites

- AWS Account with appropriate permissions
- Basic knowledge of AWS Cloud Services
- Understanding of VPC, EC2, IAM, and Networking
- Familiarity with Git version control

## 📈 Monitoring & Alerts

- **CloudWatch Metrics:** CPU utilization, request counts, error rates
- **SNS Notifications:** Auto Scaling events, deployment status
- **Health Checks:** Application Load Balancer health monitoring
- **Logging:** Lambda function logs, EC2 system logs

## 🔒 Security Considerations

- **Network Security:** Custom VPC with isolated private subnets
- **Access Control:** IAM roles with least privilege principles
- **Data Security:** Encrypted data transmission, secure S3 bucket policies
- **API Security:** API Gateway with proper CORS configuration

## 💰 Cost Optimization

- **Compute:** t2.micro instances for cost-effective hosting
- **Serverless:** Pay-per-request Lambda pricing
- **Storage:** S3 Standard for frequently accessed images
- **Auto Scaling:** Automatic capacity adjustment to optimize costs

## 📝 Lessons Learned

- Hybrid architectures combine the scalability of serverless services with the flexibility of traditional infrastructure.
- Auto Scaling and Load Balancers improve application availability and fault tolerance.
- CI/CD pipelines simplify deployment and reduce manual effort.
- Proper IAM policies and network segmentation significantly improve application security.
- AWS managed services reduce operational overhead while improving scalability and reliability.
