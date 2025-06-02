# Flask CI/CD with Jenkins + Helm + Kubernetes

## Prerequisites
- Minikube
- Jenkins
- Docker
- Helm
- kubectl

## Setup Credentials in Jenkins
1. **DockerHub**: Add username/password credential with ID `dockerhub-creds`
2. **Kubeconfig**: Add secret file credential with ID `minikube-kubeconfig`

## Run Pipeline
1. Create new Jenkins pipeline
2. Set pipeline definition to "Pipeline script from SCM"
3. Point to this repository

## Access Application
```bash
minikube service flask-app-service --url