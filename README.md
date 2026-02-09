# 🚀 K8s Project 1 – Kubernetes Deployment & Management

## 📌 Overview
This repository contains **K8s Project 1**, a practical hands-on project focused on **deploying, managing, and scaling applications using Kubernetes**.  
The project demonstrates real-world Kubernetes concepts including deployments, services, namespaces, and cluster management.

---
## 🏗️ Architecture Diagram
![Architecture Diagram](screenshots/Screenshot%202026-02-09%20233754.png)
```bash
K8s-project1_repo/
│── manifests/          # Kubernetes YAML files
│── deployments/        # Deployment configurations
│── services/           # Service definitions
│── namespaces/         # Namespace configs
│── README.md           # Project documentation
kubectl version --client
docker --version
git clone https://github.com/AEisa5/K8s-project1_repo.git
cd K8s-project1_repo
kubectl apply -f namespaces/
kubectl apply -f deployments/
kubectl apply -f services/
kubectl get all -n <namespace-name>
kubectl get pods
kubectl describe pod <pod-name>
kubectl logs <pod-name>
kubectl delete -f <file.yaml>
