**Nginx Deployment with Minikube**

**Overview**

This repository contains the configuration files and deployment setups for running Nginx on Minikube. The project aims to explore Minikube, port forwarding, and Ingress configurations from scratch.

Getting Started

**Requirements**

Minikube: A running Minikube cluster.
kubectl: Command-line tool to interact with Kubernetes.
Docker: For building and managing container images.
Setup Instructions

**Clone the Repository:**

_git clone https://github.com/<your-github-username>/nginx-deployment.git_

_cd nginx-deployment_

**Deploy Nginx: Apply the deployment files to your Minikube cluster:**

_kubectl apply -f nginx-deployment.yml_

**Port Forwarding:** To access application locally, set up port forwarding:

_kubectl port-forward service/nginx-service 8080:80_

This command maps port 8080 on the local machine to port 80 of the Nginx service.

Check Ingress (if applicable): Ensure your Ingress controller is set up and your Ingress resource is properly configured.

Check Status: Verify the status of your pods:

_kubectl get pods_

**Notes**

Feel free to review the files and provide any feedback or suggestions. Your insights would be greatly appreciated.
