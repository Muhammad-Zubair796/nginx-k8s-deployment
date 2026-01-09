# Scalable Nginx Deployment on Kubernetes
## 📌 Project Overview
This project demonstrates the deployment of a highly available, self-healing Nginx web server cluster using **Kubernetes**. It transitions from a basic single-pod setup to a production-ready **Deployment** with 10 replicas, showcasing the core strengths of container orchestration.

---

## 📸 Architecture & Verification
![Kubernetes Pod Cluster Visualization]("C:\Users\M. Zubair\Desktop\deployment.PNG")
*Above: A visual representation of the 10-replica Nginx army running within the Minikube cluster.*

---

## 🚀 Key Features Demonstrated
- **Declarative Configuration**: Used YAML manifests to define the desired state of the cluster.
- **Scalability**: Demonstrated the ability to scale from 1 to 10 instances instantly using `kubectl scale`.
- **Self-Healing**: Verified that Kubernetes automatically detects and replaces failed or deleted pods to maintain the desired replica count.
- **Resource Inspection**: Utilized `kubectl describe` and `kubectl logs` for deep-dive debugging and health monitoring.

---

## 🛠️ Technology Stack
- **Cloud**: AWS EC2 (Ubuntu 22.04 LTS)
- **Orchestration**: Kubernetes (Minikube)
- **Container Runtime**: Docker
- **Tools**: kubectl, Git

---

## 📖 Step-by-Step Implementation

### 1. Environment Setup
The cluster was initialized using Minikube with a Docker driver on an AWS EC2 instance.
```bash
minikube start --driver=docker
