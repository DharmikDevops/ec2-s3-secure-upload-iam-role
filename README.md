# 🔐 Secure EC2 to S3 File Upload using IAM Role

## 📌 Overview

This project demonstrates a secure method for enabling an EC2 instance to upload files to an S3 bucket using IAM Roles, without storing any access keys or credentials.

It follows AWS best practices such as **least privilege access** and **temporary credential usage**.

---
<br/>

## 🏗️ Architecture

EC2 Instance → S3 Bucket
_(IAM Role attached to EC2 enables secure, credential-free access)_

---
<br/>

## 🚀 Key Features

- 🔒 No hardcoded AWS credentials
- ⏳ Uses temporary credentials via IAM Role
- 🛡️ Implements least privilege principle
- ⚙️ Uses AWS CLI for file upload
- 📁 Clear separation of compute (EC2) and storage (S3)

---
<br/>

## 🧠 How It Works

1. An IAM Role is created with S3 access permissions
2. The role is attached to an EC2 instance
3. EC2 automatically receives temporary credentials
4. A file is created inside EC2
5. AWS CLI is used to upload the file to S3
6. The file is securely stored in the S3 bucket

---
<br/>

## 🛠️ Services Used

- AWS EC2
- AWS S3
- AWS IAM (Roles & Policies)
- AWS CLI

---
<br/>

## 📸 Screenshots

### EC2 Upload Command

"EC2 Upload" (screenshots/ec2-upload.png)

### File in S3 Bucket

"S3 File" (screenshots/s3-file.png)

### IAM Role Configuration

"IAM Role" (screenshots/iam-role.png)

---
<br/>

## 🔐 Security Best Practices

- No access keys or passwords used
- IAM Role used instead of IAM User credentials
- Temporary credentials automatically managed by AWS
- Minimal required permissions applied (least privilege)

---
<br/>

## 🚀 What This Project Demonstrates

- Implementation of IAM Roles for secure service access
- Use of temporary credentials instead of hardcoded keys
- Application of least privilege principle
- Secure interaction between AWS services (EC2 and S3)
- Understanding of real-world cloud architecture patterns

---
<br/>

## 💼 Real-World Use Case

This architecture is commonly used in production systems where applications running on EC2 need to securely upload logs, images, backups, or other files to S3 without exposing credentials.

---
