🚀 Kubernetes Nginx Deployment (Minikube)

📌 Overview

This project demonstrates the deployment of a containerized Nginx application on a local Kubernetes cluster using Minikube and Docker.

The objective was to gain hands-on experience with Kubernetes workload management using a declarative approach and to understand how Kubernetes maintains application state automatically.

🎯 Objectives

Set up a local Kubernetes cluster using Minikube

Deploy an application using a Deployment resource

Configure multiple replicas for high availability

Understand label selectors and pod templates

Apply changes using a declarative workflow

Monitor rollout and verify deployment health

⚙️ What Was Implemented

Kubernetes cluster initialization with Docker driver

Deployment creation using the apps/v1 API

Multi-replica configuration

Rolling update validation

Deployment scaling via kubectl

Troubleshooting kubeconfig and API server issues

🧠 Key Concepts Practiced

Declarative vs imperative Kubernetes management

Deployment and ReplicaSet relationship

Desired state reconciliation

Pod lifecycle management

Cluster context and configuration handling

Debugging real-world Kubernetes errors

✅ Outcome

The application was successfully deployed with multiple replicas running in the cluster. Kubernetes automatically maintained the desired state and ensured workload availability.

This project strengthened practical understanding of Kubernetes core components and deployment workflows.

🔮 Next Steps

Expose the application using a Service

Implement health checks (liveness & readiness probes)

Configure resource requests and limits

Add ingress configuration

Integrate with CI/CD pipeline

👤 Author

Karthik Chitikela
DevOps & Cloud Engineering Enthusiast
