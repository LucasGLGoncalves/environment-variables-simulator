# 🌱 Environment Variables Simulator

A simple Node.js + Express application that reads and displays environment variables. Built for learning and practicing **environment variable management** best practices with `.env`, Docker, Docker Compose, and Kubernetes.

---

## 📘 Português (PT-BR)

### 🎯 Objetivo

Esta aplicação foi criada para servir como laboratório prático para o gerenciamento de variáveis de ambiente em diferentes contextos. Ela permite explorar:

- Leitura de variáveis a partir de arquivos `.env`
- Injeção de variáveis via linha de comando (Docker CLI)
- Uso de `ENV` e `ARG` no Dockerfile
- Definição de variáveis no `docker-compose.yml`
- Uso de variáveis em shells (Linux/macOS)
- Mapeamento com `ConfigMaps` e `Secrets` no Kubernetes
- Injeção de variáveis via manifestos Kubernetes
- Outros cenários comuns de configuração dinâmica

O objetivo é praticar **boas práticas no gerenciamento de variáveis de ambiente**, considerando diferentes ferramentas e ambientes.

### ⚙️ Tecnologias Utilizadas

- Node.js
- Express
- EJS
- dotenv
- Docker

### 🚀 Como Executar Localmente

1. Instale as dependências:

   ```bash
   npm install
   ```

2. Crie um arquivo `.env` com o seguinte conteúdo:

   ```env
   APP_NAME=Minha Aplicação
   APP_VERSION=1.0.0
   APP_AUTHOR=Seu Nome
   ```

3. Execute o servidor:

   ```bash
   node server.js
   ```

4. Acesse `http://localhost:3000` no navegador.

### 🐳 Usando com Docker

1. Build da imagem:

   ```bash
   docker build -t environment-variables-simulator .
   ```

2. Executando o container:

   ```bash
   docker run -p 3000:3000 --env-file .env environment-variables-simulator
   ```

---

## 🇺🇸 English

### 🎯 Purpose

This application was created as a practical lab for managing environment variables in different contexts. It allows you to explore:

- Reading variables from `.env` files
- Injecting variables via CLI (Docker command line)
- Using `ENV` and `ARG` in Dockerfiles
- Setting variables in `docker-compose.yml`
- Exporting variables from shell environments (Linux/macOS)
- Mapping with Kubernetes `ConfigMaps` and `Secrets`
- Injecting variables through Kubernetes manifests
- Other common dynamic configuration scenarios

The goal is to practice **best practices for environment variable management** across multiple tools and deployment environments.

### ⚙️ Technologies Used

* Node.js
* Express
* EJS
* dotenv
* Docker

### 🚀 How to Run Locally

1. Install the dependencies:

   ```bash
   npm install
   ```

2. Create a `.env` file with the following:

   ```env
   APP_NAME=My Application
   APP_VERSION=1.0.0
   APP_AUTHOR=Your Name
   ```

3. Start the server:

   ```bash
   node server.js
   ```

4. Open your browser and go to `http://localhost:3000`.

### 🐳 Using Docker

1. Build the image:

   ```bash
   docker build -t environment-variables-simulator .
   ```

2. Run the container:

   ```bash
   docker run -p 3000:3000 --env-file .env environment-variables-simulator
   ```

---

## 📁 Project Structure / Estrutura do Projeto

```
environment-variables-simulator/
│
├── .github/           # GitHub configurations
├── src/
│   ├── Dockerfile     # Docker container
│   ├── server.js      # Main application code
│   ├── package.json   # Project dependencies
│   ├── .env           # Environment variables file (DO NOT commit this)
│   └── views/         # EJS templates
│
└── README.md
```
