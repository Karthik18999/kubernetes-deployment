🚀 Kubernetes Nginx Deployment (Minikube)

This project demonstrates a hands-on Kubernetes deployment using Minikube and Docker driver. It includes creating a Deployment, managing replicas, and applying declarative configuration using YAML.

📌 Project Overview

In this project:

Minikube cluster was created using Docker driver

Deployment YAML was written manually

Nginx container deployed with multiple replicas

Resources configured with CPU and memory limits

Deployment applied using kubectl apply

Rolling update mechanism verified

YAML structure and indentation issues debugged

This project focuses on understanding Kubernetes fundamentals through practical implementation.

🛠 Tech Stack

Kubernetes (v1.35.x)

Minikube

Docker

kubectl

YAML

🚀 How to Run
1️⃣ Start Minikube
minikube start --driver=docker
minikube update-context
2️⃣ Apply Deployment
kubectl apply -f deployment.yml
3️⃣ Verify
kubectl get deployments
kubectl get pods
kubectl describe deployment nginx-deployment
🔄 Scaling

To scale replicas:

kubectl scale deployment nginx-deployment --replicas=5

🔍 Key Learnings:

Importance of correct YAML indentation

Difference between kubectl create and kubectl apply

How Kubernetes manages replicas

How kubeconfig context affects kubectl behavior

Understanding control plane components (kubelet, apiserver)

📈 Next Improvements

Add Service (ClusterIP / NodePort)

Implement Rolling Updates

Add Liveness & Readiness Probes

Deploy using Helm

Integrate with CI/CD pipeline

🧠 Author

Karthik Chitikela
Aspiring DevOps & Cloud Engineer
