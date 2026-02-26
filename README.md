Kubernetes Nginx Deployment using Minikube
Overview

This project demonstrates the deployment of a containerized Nginx application on a Kubernetes cluster using Minikube with the Docker driver. The objective was to understand core Kubernetes workload management concepts including Deployments, replica management, and declarative configuration.

The project follows Kubernetes best practices by using YAML-based manifests and a declarative deployment model.

Architecture

Local Kubernetes Cluster: Minikube

Container Runtime: Docker

Workload Type: Deployment

Application: Nginx (multi-replica)

Configuration Management: Declarative YAML

The Deployment ensures high availability by maintaining multiple replicas of the Nginx pod.

Features Implemented

Cluster initialization using Minikube

Deployment creation using apps/v1

Replica configuration for high availability

Label selectors and pod template configuration

Container port exposure

Rolling update capability

Resource verification using kubectl commands

Project Structure
.
└── deployment.yml

Setup Instructions
1. Start Minikube
minikube start --driver=docker
minikube update-context
2. Deploy Application
kubectl apply -f deployment.yml
3. Verify Deployment
kubectl get deployments
kubectl get pods
kubectl describe deployment nginx-deployment
Scaling the Deployment
kubectl scale deployment nginx-deployment --replicas=5

Kubernetes automatically manages pod creation and ensures the desired state is maintained.

Key Learnings

Importance of YAML structure and indentation in Kubernetes manifests

Difference between imperative (create) and declarative (apply) approaches

Understanding Kubernetes control plane components

ReplicaSet behavior and rolling updates

Managing kubeconfig contexts

Future Enhancements

Add Service (ClusterIP / NodePort)

Implement health probes (liveness and readiness)

Configure resource limits and requests

Integrate with CI/CD pipeline

Extend to production-grade architecture

Author

Karthik Chitikela
DevOps & Cloud Engineering Enthusiast
