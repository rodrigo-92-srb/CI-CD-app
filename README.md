# CI-CD Node.js Application

Este projeto implementa uma aplicação Node.js com deploy em dois cenários:

- **Docker**: Deploy em um contêiner Docker.
- **Kubernetes**: Deploy em um cluster Kubernetes na GCP.

## Estrutura das Branches

- **docker-deploy**: Configuração para deploy em Docker.
- **kubernetes-deploy**: Configuração para deploy em Kubernetes (GCP).

### Instruções para Executar Localmente

Para executar a aplicação localmente usando Docker:
```bash
docker build -t my-node-app .
docker run -p 3000:3000 my-node-app

### CI/CD com GitHub Actions

Este repositório usa GitHub Actions para construir e implementar a aplicação automaticamente:

- Deploy Docker: Configurado na branch `docker-deploy`.
- Deploy Kubernetes: Configurado na branch `kubernetes-deploy`.
