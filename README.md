# 🚀 Self-Healing Canary DevOps Pipeline on AWS

This project demonstrates a production-style DevOps pipeline using AWS, Terraform, Docker, and GitHub Actions.

---

## 📌 Overview

This system automates infrastructure provisioning and application deployment using CI/CD.

Every code push triggers an automated pipeline that:

- Connects to EC2
- Pulls latest code
- Builds Docker image
- Deploys updated application

---

## 🏗️ Architecture

User → Application Load Balancer → EC2 Instances → Docker Containers

CI/CD Flow:
GitHub Push → GitHub Actions → SSH → EC2 → Docker Deploy

---

## ⚙️ Tech Stack

- **Cloud:** AWS (EC2, ALB, VPC)
- **IaC:** Terraform
- **Containerization:** Docker
- **CI/CD:** GitHub Actions
- **Version Control:** GitHub

---

## 🚀 Features

- Infrastructure provisioning using Terraform
- Multi-tier architecture with VPC and subnets
- Dockerized application deployment
- Automated CI/CD pipeline using GitHub Actions
- SSH-based deployment to EC2
- Canary-style deployment architecture (ALB)

---

## 🔄 CI/CD Workflow

1. Developer pushes code to GitHub
2. GitHub Actions pipeline triggers
3. Pipeline connects to EC2 via SSH
4. Pulls latest repository
5. Builds Docker image
6. Runs container on port 80
7. Application updates automatically

---

## 📁 Project Structure


self-healing-canary-devops-aws/

├── app/

│   ├── Dockerfile

│   └── index.html

│

├── infra/

│   ├── main.tf

│   └── provider.tf

│

├── .github/workflows/

│   └── deploy.yml

│

└── .gitignore


---
## 🧪 How to Test

1. Update `index.html`
2. Push changes to GitHub
3. Wait for GitHub Actions to run
4. Access application via EC2 public IP
---
## 📈 Key Learning

- End-to-end DevOps pipeline implementation
- CI/CD automation
- Docker-based deployments
- Infrastructure as Code using Terraform
- Debugging real-world pipeline failures

---

## 🔥 Future Improvements

- Auto Scaling (self-healing infrastructure)
- CloudWatch monitoring & alerts
- Blue-Green deployments
- Kubernetes (EKS) integration
- Docker image push to AWS ECR

---

## 👨‍💻 Author

Akshay
