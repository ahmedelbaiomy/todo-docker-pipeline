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

### Option 1: Run Pre-built Image (Fastest)

Pull and run the latest image from GitHub Container Registry:

```bash
# Pull the image
docker pull ghcr.io/ahmedelbaiomy/todo-docker-pipeline:latest

# Run the container
docker run -d -p 3000:3000 --name todo-app ghcr.io/ahmedelbaiomy/todo-docker-pipeline:latest

# Access the application
# Open your browser: http://localhost:3000



