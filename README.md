# Projeto DevOps: Prática de Kubernetes com Kind e Docker 🚀

Este projeto foi criado para consolidar o entendimento prático da arquitetura do Kubernetes (K8s) utilizando o **Kind** para rodar um cluster local e o **Kubectl** para gerenciar os objetos.

##  Entendendo a Estrutura (Camadas)

O projeto foi estruturado em 3 camadas principais, trabalhando de fora para dentro:

1. **O Cluster (O Condomínio):** Criado via Kind. É o ambiente isolado que gerencia as máquinas (nós) no PC.
2. **O Pod (O Apartamento):** Criado via Kubectl. É a cápsula de rede que protege e roda o nosso container.
3. **O Container (O Morador):** Criado via Dockerfile. É a nossa aplicação frontend rodando dentro do Nginx.

---

## 🛠️ Guia de Comandos (Para Amanhã)

### Passo 1: Construir a Imagem Docker (na pasta do front)
```bash
docker build -t meu-frontend:v2 .
