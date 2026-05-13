# Flask DevOps Project 🚀

A production-style DevOps project demonstrating the deployment of a Flask web application using modern DevOps tools and cloud infrastructure automation.

This project showcases containerization, CI/CD automation, Infrastructure as Code (IaC), and cloud deployment practices used in real-world DevOps environments.

---

# 📌 Project Overview

The Flask DevOps Project was designed to implement a complete DevOps workflow from development to deployment.

The project includes:

* Flask web application development
* Docker containerization
* Jenkins CI/CD pipeline automation
* GitHub Actions workflow integration
* Terraform Infrastructure as Code (IaC)
* AWS cloud deployment
* Linux-based development environment using WSL Ubuntu

The objective of this project is to automate software delivery, infrastructure provisioning, and deployment workflows using industry-standard DevOps practices.

---

# 🏗️ Project Architecture

```text
                    ┌────────────────────┐
                    │      Developer     │
                    │   Pushes Code to   │
                    │       GitHub       │
                    └─────────┬──────────┘
                              │
                              ▼
                    ┌────────────────────┐
                    │       GitHub       │
                    │ Source Code Repo   │
                    └─────────┬──────────┘
                              │ Webhook Trigger
                              ▼
                    ┌────────────────────┐
                    │      Jenkins       │
                    │    CI/CD Server    │
                    └─────────┬──────────┘
                              │
          ┌───────────────────┼───────────────────┐
          │                   │                   │
          ▼                   ▼                   ▼
 ┌────────────────┐  ┌────────────────┐  ┌────────────────┐
 │ Build Pipeline │  │ Run Tests      │  │ Build Docker   │
 │                │  │                │  │ Image          │
 └────────────────┘  └────────────────┘  └────────┬───────┘
                                                   │
                                                   ▼
                                        ┌──────────────────┐
                                        │ Docker Container │
                                        │ Flask App Image  │
                                        └────────┬─────────┘
                                                 │
                                                 ▼
                                        ┌──────────────────┐
                                        │ Terraform        │
                                        │ Infrastructure   │
                                        │ Provisioning     │
                                        └────────┬─────────┘
                                                 │
                                                 ▼
                                        ┌──────────────────┐
                                        │ AWS EC2 Instance │
                                        │ Cloud Deployment │
                                        └────────┬─────────┘
                                                 │
                                                 ▼
                                        ┌──────────────────┐
                                        │ Flask Web App    │
                                        │ Running Live     │
                                        └──────────────────┘
```

---

# ⚙️ Tech Stack

| Category               | Technologies            |
| ---------------------- | ----------------------- |
| Programming Language   | Python                  |
| Backend Framework      | Flask                   |
| Containerization       | Docker                  |
| CI/CD Automation       | Jenkins, GitHub Actions |
| Infrastructure as Code | Terraform               |
| Cloud Platform         | AWS EC2                 |
| Version Control        | Git & GitHub            |
| Operating System       | Linux (WSL Ubuntu)      |
| Automation             | Shell Scripting         |

---

# 🚀 Key Features

* Automated CI/CD Pipeline
* Dockerized Flask Application
* Infrastructure as Code (IaC)
* Automated Cloud Deployment
* Continuous Integration Workflow
* Continuous Delivery Pipeline
* Reproducible Deployment Environment
* Version Controlled Infrastructure
* Cloud Infrastructure Provisioning

---

# 🔄 DevOps Workflow

## 1. Development Phase

The developer writes and updates the Flask application locally.

## 2. Source Code Management

Code is pushed to GitHub for version control and collaboration.

## 3. CI/CD Automation

Jenkins and GitHub Actions automatically trigger build and deployment pipelines.

## 4. Docker Containerization

The Flask application is packaged into a Docker container to ensure consistency across environments.

## 5. Infrastructure Provisioning

Terraform automates AWS infrastructure creation including EC2 instances and networking resources.

## 6. Cloud Deployment

The Dockerized Flask application is deployed to AWS EC2.

## 7. Application Access

Users can access the live application using the EC2 public IP.

---

# 📂 Project Structure

```text
flask-devops-project/
│
├── app.py
├── requirements.txt
├── Dockerfile
├── Jenkinsfile
├── README.md
│
├── templates/
│   └── index.html
│
├── static/
│
├── terraform/
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
│   └── provider.tf
│
├── scripts/
│   └── deploy.sh
│
└── .github/
    └── workflows/
        └── main.yml
```

---

# 🐳 Docker Setup

## Build Docker Image

```bash
docker build -t flask-devops-app .
```

## Run Docker Container

```bash
docker run -p 5000:5000 flask-devops-app
```

---

# ☁️ Terraform Deployment

## Initialize Terraform

```bash
terraform init
```

## Validate Terraform Files

```bash
terraform validate
```

## Apply Infrastructure

```bash
terraform apply
```

---

# 🔧 Jenkins CI/CD Pipeline

The Jenkins pipeline automates:

* Source code checkout
* Dependency installation
* Build process
* Docker image creation
* Deployment workflow
* Continuous Integration and Delivery

---

# ☁️ AWS Services Used

* AWS EC2
* AWS Security Groups
* AWS Networking

---

# 📈 Future Improvements

* Kubernetes Deployment
* Docker Hub Integration
* Prometheus & Grafana Monitoring
* HTTPS & SSL Integration
* AWS Load Balancer Setup
* Auto Scaling Configuration
* Advanced CI/CD Stages

---

# 📚 Learning Outcomes

This project helped implement and understand:

* CI/CD Pipeline Automation
* Infrastructure as Code (IaC)
* Docker Containerization
* Cloud Infrastructure Management
* AWS Deployment Workflows
* DevOps Automation Practices
* GitHub Version Control
* Jenkins Pipeline Management

---


# 👩‍💻 Author

Areeba Waqas
DevOps & Cloud Enthusiast
