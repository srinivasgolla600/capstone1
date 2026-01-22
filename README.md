# 🚀 Capstone Project — CI/CD Pipeline with Jenkins, Docker & Kubernetes (Minikube)

This project demonstrates a **full end-to-end CI/CD pipeline** that automates building, pushing, and deploying a web application using **Jenkins**, **Docker**, **Docker Hub**, and **Kubernetes (Minikube)**.

It simulates a real-world DevOps workflow where code changes trigger automated builds and container deployments.

---

## 🧠 Project Overview

### Workflow:




### What happens:
- Developer pushes code to GitHub
- Jenkins pulls the code automatically
- Jenkins builds a Docker image
- Jenkins pushes the image to Docker Hub
- Jenkins deploys the image to Minikube Kubernetes cluster
- Application becomes live via Kubernetes Service

---

## 🛠️ Tech Stack

- Git & GitHub  
- Jenkins (CI/CD automation)  
- Docker (containerization)  
- Docker Hub (image registry)  
- Kubernetes (Minikube)  
- kubectl (cluster management)  
- HTML & CSS (frontend web app)  

---

## 📁 Project Structure
capstone1/
│
├── Dockerfile
├── Jenkinsfile
├── index.html
├── k8s/
│ ├── deployment.yaml
│ └── service.yaml
└── README.md



---

## 🐳 Docker Image

Docker image is built and pushed to Docker Hub:


<img width="1920" height="1080" alt="Screenshot (7)" src="https://github.com/user-attachments/assets/78cbe12c-3a01-49ba-8de3-b0506c83a54c" />

---

## ☸️ Kubernetes Deployment (Minikube)

### Apply Kubernetes manifests:

```bash
kubectl apply -f k8s/


kubectl scale deployment web-app --replicas=3

Access the Webpage:

minikube service web-service

🔄 Jenkins Pipeline Stages
Jenkinsfile includes:

Checkout source code

Build Docker image

Push image to Docker Hub

Deploy to Kubernetes cluster




<img width="1920" height="1080" alt="Screenshot (7)" src="https://github.com/user-attachments/assets/49282a0c-7326-4964-ad45-80740c81a33f" />



