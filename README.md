# 🚀 DevOps Capstone Project

This project demonstrates the implementation of a complete DevOps lifecycle including infrastructure provisioning, configuration management, CI/CD pipeline, and containerization.

---

## 📌 Project Overview

The goal of this project is to automate the deployment of a web application using DevOps tools and best practices. The system provisions infrastructure, configures nodes, builds and deploys applications, and ensures continuous integration and delivery.

---

## 🛠️ Tools & Technologies Used

- AWS EC2
- Terraform (Infrastructure as Code)
- Ansible (Configuration Management)
- Jenkins (CI/CD Pipeline)
- Docker (Containerization)
- GitHub (Version Control)

---

## ⚙️ Project Architecture

### 1. Infrastructure Setup
- Provisioned multiple EC2 instances using **Terraform**
- Created separate nodes for:
  - Jenkins Server
  - Application Server(s)

---

### 2. Configuration Management
- Used **Ansible** to:
  - Install required software on all nodes
  - Configure environments automatically

---

### 3. CI/CD Pipeline
- Implemented a **Jenkins Pipeline** to:
  - Clone code from GitHub
  - Build Docker image
  - Deploy application container
- Pipeline triggers automatically on code push

---

### 4. Containerization
- Application is containerized using **Docker**
- Used base image: `hshar/webapp` forked
- Application code is deployed to: /var/www/html


---

## 🔄 Workflow

1. Developer pushes code to GitHub
2. Jenkins pipeline is triggered
3. Docker image is built using Dockerfile
4. Container is deployed to the application server
5. Updated application goes live automatically

---

The following were captured and documented:

- ✅ Nodes created and configured
- ✅ Infrastructure setup using Terraform
- ✅ Ansible execution logs
- ✅ Jenkins pipeline stages
- ✅ Console output of builds
- ✅ Code changes tracking

---


---

## 💡 Key Features

- Fully automated infrastructure provisioning
- Configuration management with Ansible
- Continuous Integration & Deployment
- Docker-based application deployment
- Scalable and reproducible setup

---

## 📈 Outcome

- Successfully built an end-to-end DevOps pipeline
- Reduced manual intervention in deployment
- Achieved faster and reliable delivery process

---

## 🧠 Learnings

- Hands-on experience with real-world DevOps tools
- Understanding CI/CD pipeline design
- Infrastructure automation using Terraform
- Configuration management using Ansible
- Containerization using Docker

---

## 📬 Author

**Supradeepan K**

---
