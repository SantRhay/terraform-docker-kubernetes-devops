# 🚀 DevOps Project - Docker + Kubernetes + CI/CD

![CI/CD](https://github.com/SantRhay/terraform-docker-kubernetes-devops/actions/workflows/docker-image.yml/badge.svg)
![Docker](https://img.shields.io/badge/Docker-Container-blue)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-blue)
![Terraform](https://img.shields.io/badge/Infrastructure-Terraform-purple)

Este projeto demonstra um fluxo completo de DevOps utilizando Docker, Kubernetes e CI/CD com GitHub Actions.

---

# 📌 Arquitetura

GitHub → GitHub Actions → Docker Build → DockerHub → Kubernetes Deploy

---

# 🛠 Tecnologias utilizadas

- Docker
- Kubernetes
- Minikube
- GitHub Actions
- DockerHub
- Linux
- HTML

---

# 📂 Estrutura do projeto

app/
index.html

docker/
Dockerfile

k8s/
deployment.yaml
service.yaml

.github/workflows/
docker-image.yml

README.md

---

# 🐳 Build da imagem Docker

docker build -t devops-app .

---

# 📤 Push para DockerHub

docker tag devops-app usuario/devops-app:latest

docker push usuario/devops-app:latest

---

# ☸ Deploy Kubernetes

kubectl apply -f k8s/deployment.yaml

kubectl apply -f k8s/service.yaml

kubectl get pods

---

# 🔄 CI/CD Pipeline

A pipeline com GitHub Actions executa:

1. Checkout do código  
2. Login no DockerHub  
3. Build da imagem Docker  
4. Push da imagem para DockerHub

---

# 🌐 Acesso à aplicação

minikube service devops-service

---

# 👩‍💻 Autor

Rayane Santana  
DevOps | Cloud | Infrastructure as Code


---
