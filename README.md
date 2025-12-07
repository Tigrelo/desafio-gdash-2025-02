# ⚡ Desafio Técnico GDASH 2025/02 — Monitoramento de Dados Climáticos

Este projeto implementa um sistema completo de **coleta, processamento e visualização de dados climáticos**, usando microsserviços que se comunicam por eventos.  
A aplicação atende 100% dos requisitos do desafio.

---

## 🚀 Arquitetura

O fluxo principal funciona assim:

**Python (Coletor) → RabbitMQ → Go (Worker) → NestJS (API) → MongoDB → React (Dashboard)**

Cada parte tem uma função específica e roda em containers via Docker.

---

## 🧩 Tecnologias Utilizadas

| Componente | Tecnologia |
|-----------|------------|
| Coletor de dados | Python |
| Fila de mensageria | RabbitMQ |
| Processamento | Go |
| API principal | NestJS (TypeScript) |
| Banco de dados | MongoDB |
| Interface | React + Vite + Tailwind + Shadcn |
| Orquestração | Docker Compose |

---

## 🌟 Funcionalidades

- Coleta automática de dados climáticos pela API Open-Meteo  
- Envio e consumo de mensagens via RabbitMQ  
- API REST com CRUD de usuários e autenticação JWT  
- Dashboard com visualização dos dados em tempo real  
- Exportação de dados em CSV  
- Integração opcional com PokéAPI  
- Alertas inteligentes no frontend

---

## 💡 Destaques

- **Worker em Go** para maior desempenho no processamento.  
- **Swagger** disponível para testar a API.  
- **Serviços independentes**, fáceis de escalar.  

---

## 🛠️ Como Rodar o Projeto

### 1. Requisitos
- Docker Desktop instalado

### 2. Subir tudo

docker compose up -d --build

### 3. Ver logs do coletor e worker

docker compose logs -f collector worker

Acessos
Serviço	URL
Frontend	http://localhost:5173

Documentação da API	http://localhost:3000/api/docs
Credenciais padrão:

Email: admin@example.com

Senha: 123456
---
### link de vídeo: https://youtu.be/66YJEW7yaFE

