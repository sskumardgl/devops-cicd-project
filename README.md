#  DevOps CI/CD Pipeline with Docker & Kubernetes

##  Project Overview
This project demonstrates an end-to-end CI/CD pipeline that automates application build, containerization, and deployment to Kubernetes.

---

## Tech Stack
- Python (Flask)
- Docker
- Jenkins
- Kubernetes
- GitHub

---

##  Architecture Diagram

Developer → GitHub → Jenkins → Docker Build → Docker Image → Kubernetes Cluster → Application


Detailed Flow:

1. Developer pushes code to GitHub
2. Jenkins triggers pipeline
3. Docker image is built
4. Image is deployed to Kubernetes
5. Application becomes accessible via service

---

## ⚙️ Setup Instructions

### 1. Clone Repo
```bash
git clone https://github.com/yourusername/devops-cicd-project.git
cd devops-cicd-project

2. Build Docker Image
docker build -t devops-app .

3. Run Locally
docker run -p 5000:5000 devops-app

4. Deploy to Kubernetes
kubectl apply -f k8s/
