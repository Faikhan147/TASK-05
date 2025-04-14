# TASK-05
Elevate Labs

# 🚀 Kubernetes Cluster with Minikube

## 📌 Objective
Deploy and manage a simple application on a local Kubernetes cluster using Minikube.

---

## 🛠 Tools Used
- **Minikube** – to create a local Kubernetes cluster
- **kubectl** – CLI to interact with Kubernetes
- **Docker** – container runtime used by Minikube

---

## 📁 Project Structure

k8s-minikube-project/ │ ├── nginx-deployment.yaml # Deployment definition ├── nginx-service.yaml # Service definition ├── README.md # Documentation (this file) └── screenshots/ # Folder containing CLI and app screenshots



---

## ⚙️ Steps to Run the Project

### 1️⃣ Install and Start Minikube

```bash
minikube start --driver=virtualbox --memory=4000 --cpus=2 --force 

kubectl apply -f nginx-deployment.yaml

kubectl apply -f nginx-service.yaml

kubectl get pods

kubectl get services

kubectl logs <pod-name>

