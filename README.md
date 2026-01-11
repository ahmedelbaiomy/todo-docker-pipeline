# 📝 Todo App – Dockerized Node.js Application

A **Todo application** built with **Node.js** and fully containerized using **Docker**. This project demonstrates modern DevOps practices including containerization, automated CI/CD pipelines, and container registry management.

[![Docker Image CI](https://github.com/ahmedelbaiomy/todo-docker-pipeline/actions/workflows/docker-image.yml/badge.svg)](https://github.com/ahmedelbaiomy/todo-docker-pipeline/actions/workflows/docker-image.yml)
[![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)](https://www.docker.com/)
[![Node.js](https://img.shields.io/badge/Node.js-18-339933?logo=node.js&logoColor=white)](https://nodejs.org/)

---

## 🎯 Project Overview

This project showcases:

- ✅ **Docker Containerization** - Application packaged in a portable container
- ✅ **CI/CD Pipeline** - Automated builds using GitHub Actions
- ✅ **Container Registry** - Images published to GitHub Container Registry (GHCR)
- ✅ **Development Workflow** - Easy local development with Docker

---

## 🛠 Technologies Used

- **Node.js 18** - JavaScript runtime
- **Docker** - Containerization platform
- **GitHub Actions** - CI/CD automation
- **GHCR** - Container image registry

---

## 🚀 Quick Start

### Prerequisites

- Docker installed on your machine [Download here](https://www.docker.com/get-started)

---

### Option 2: Build from Source

Clone and build the image yourself:

```bash
# Pull the image
docker pull ghcr.io/ahmedelbaiomy/todo-docker-pipeline:latest

# Run the container
docker run -d -p 3000:3000 --name todo-app ghcr.io/ahmedelbaiomy/todo-docker-pipeline:latest

# Access the application
# Open your browser: http://localhost:3000

```
### Option 1: Run Pre-built Image (Fastest)

Pull and run the latest image from GitHub Container Registry:
```bash
# Clone the repository
git clone https://github.com/ahmedelbaiomy/todo-docker-pipeline.git
cd todo-docker-pipeline

# Build the Docker image
docker build -t todo-app .

# Run the container
docker run -d -p 3000:3000 --name todo-app todo-app

# Access the application
# Open your browser: http://localhost:3000

```

```markdown
---

## 🔄 CI/CD Pipeline

This project uses **GitHub Actions** to automate the build and deployment process.

### How It Works
Code Push → GitHub Actions → Build Image → Push to GHCR → Ready to Deploy


### Pipeline Triggers

- ✅ Push to `master` branch
- ✅ Pull requests to `master`

### What Happens Automatically

1. Checks out code from repository
2. Builds Docker image
3. Logs in to GitHub Container Registry
4. Tags image with `latest` and commit SHA
5. Pushes image to GHCR

[View Pipeline Status →](https://github.com/ahmedelbaiomy/todo-docker-pipeline/actions)

```

## 🧪 Development Mode

Run the application with live code reload:

```bash
# For Linux/macOS
docker run -it \
  -p 3000:3000 \
  -v $(pwd):/app \
  -v node_modules:/app/node_modules \
  -w /app \
  node:18-alpine sh

# For Windows PowerShell
docker run -it `
  -p 3000:3000 `
  -v ${PWD}:/app `
  -v node_modules:/app/node_modules `
  -w /app `
  node:18-alpine sh

  ```

  ```bash 
  npm install
  npm run dev
  ```

  
