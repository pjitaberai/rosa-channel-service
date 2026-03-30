# 🧱 Tech Stack

![Python](https://img.shields.io/badge/Python-3.11+-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-Framework-009688)
![Docker](https://img.shields.io/badge/Docker-Containerization-2496ED)
![CI](https://img.shields.io/badge/CI-GitHub_Actions-2088FF)

Este projeto utiliza uma arquitetura moderna, escalável e orientada a processamento assíncrono, visando alta performance, confiabilidade e desacoplamento.

---

## 🔙 Backend
- **FastAPI** – Framework web de alta performance para APIs  
- **Pydantic** – Validação e serialização de dados  
- **SQLAlchemy** – ORM (Mapeamento Objeto-Relacional)  
- **Alembic** – Migrations de banco de dados  

---

## 📨 Mensageria
- **RabbitMQ** – Broker de mensagens para gerenciamento de filas  
- **Celery** – Processamento assíncrono de tarefas  

---

## ⚙️ Processamento
- **Celery Worker** – Execução de tarefas em background  
- **Celery Beat** – Agendamento de tarefas periódicas  

---

## 🗄️ Banco de Dados
- **PostgreSQL** – Banco relacional para persistência  

---

## ⚡ Backend de Tarefas / Cache
- **Redis** – Utilizado como backend do Celery e camada de cache  

---

## 🐳 Infraestrutura
- **Docker** – Containerização das aplicações  
- **Docker Compose** – Orquestração local para desenvolvimento  
- **Docker Swarm** – Orquestração para ambiente de produção  

---

## 🚀 CI/CD
- **GitHub Actions** – Integração e entrega contínua  

---

## 🧪 Testes
- **Pytest** – Testes unitários e de integração  
- **Pytest-Cov** – Cobertura de código  
- **Playwright** *(opcional)* – Testes end-to-end  

---

## 📚 Documentação *(opcional)*
- **MkDocs** – Geração de documentação estática  

---

## 🎯 Qualidade de Código
- **Black** – Formatação automática de código  
- **Isort** – Organização de imports  

---

# 📦 Containers

A aplicação é composta por múltiplos containers executando a partir do mesmo código:

- **API** – Aplicação FastAPI (camada HTTP)  
- **Worker** – Processamento assíncrono (Celery)  
- **Beat** – Agendador de tarefas  
- **RabbitMQ** – Broker de mensageria  
- **Redis** – Backend de tarefas / cache  
- **PostgreSQL** – Banco de dados  

---

## 🧠 Nota de Arquitetura

Apesar de ser um único repositório, o sistema é executado como múltiplos serviços:

- A **API** recebe requisições e envia tarefas para a fila  
- O **Worker** processa essas tarefas de forma assíncrona  
- A comunicação entre eles ocorre via **RabbitMQ**

Esse modelo garante:
- Escalabilidade  
- Desacoplamento  
- Resiliência  
- Melhor performance (não bloqueante) 
