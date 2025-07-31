# 🗳️ Kubernetes Voting App using Deployments

This project demonstrates the deployment of a microservices-based **Voting App** using **Kubernetes Deployments**, running on **Docker Desktop** with `kubectl`.

## 🛠️ Tech Stack

- **Frontend**: Python Flask (Vote)
- **Backend**: .NET Core (Worker)
- **Database**: PostgreSQL + Redis
- **Orchestration**: Kubernetes (with YAML manifests using Deployments)
- **Containerization**: Docker

## 📦 Components

| Service  | Description                       |
|----------|-----------------------------------|
| vote     | Frontend Flask app                |
| result   | Node.js app to show results       |
| worker   | .NET Core app for vote processing |
| redis    | Redis queue                       |
| db       | PostgreSQL database               |

## 🖼️ App Preview

> "Cats vs Dogs!" voting app that lets users cast votes and see live results.

---

## 🚀 Deployment

### Prerequisites

- Kubernetes cluster (e.g., Docker Desktop, Minikube, etc.)
- `kubectl` installed and configured
- Docker images already built and pushed (or use public ones)

### Deploy to Kubernetes

To deploy :

kubectl create -f .

### to check your deployments
kubectl get deployments

### to increase or decrese the scaling in deployments
kubectl scale deployment <deployment-name> --replicas=<number>


```bash
kubectl apply -f .
