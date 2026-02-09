# Docker-in-Strapi-Application
# 🚀 Docker in Strapi Application (Multistage Docker Setup)

This project demonstrates how to dockerize a **Strapi application** using a **Multistage Dockerfile** for production-ready deployment.

---

## 📌 Features
- ✅ Strapi Application Dockerized
- ✅ Multistage Docker Build (Optimized Image Size)
- ✅ Environment file support (`.env.example`)
- ✅ Production build supported
- ✅ Clean folder structure

---

## 🏗️ Project Structure
Docker-in-Strapi-Application/
│── Dockerfile
│── .dockerignore
│── .env.example
│── package.json
│── package-lock.json
│── config/
│── src/
│── public/
│── database/

---

## ⚙️ Prerequisites
Make sure you have installed:

- Docker
- Docker Compose (optional)
- Node.js (only if running locally)

---

## 🐳 Build Docker Image
Run this command inside the project folder:

```bash
docker build -t strapi-app .
▶️ Run Strapi Container
docker run -d -p 1337:1337 --name strapi-container strapi-app

🌍 Access Strapi

Once the container is running, open:

Strapi Admin Panel

http://localhost:1337/admin


Strapi API

http://localhost:1337/api

🧪 Check Running Containers
docker ps

🛑 Stop & Remove Container
docker stop strapi-container
docker rm strapi-container

📦 Push to Docker Hub (Optional)
docker tag strapi-app <your-dockerhub-username>/strapi-app:latest
docker push <your-dockerhub-username>/strapi-app:latest
