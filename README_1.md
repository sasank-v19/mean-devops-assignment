# MEAN Stack DevOps Deployment

This project demonstrates containerization, CI/CD automation, and cloud deployment of a MEAN (MongoDB, Express, Angular, Node.js) application using Docker, GitHub Actions, and AWS EC2.

---

## 🚀 Project Architecture

User → Nginx Reverse Proxy → Frontend → Backend → MongoDB

---

## 🐳 Docker Setup

### Backend
Located in backend/Dockerfile

### Frontend
Located in frontend/Dockerfile

### Reverse Proxy
nginx-proxy/nginx.conf

---

## ⚙️ Docker Compose Deployment

Run:

docker compose up -d

Services:
- MongoDB
- Backend API (Node.js)
- Frontend (Angular)
- Nginx Reverse Proxy

---

## ☁️ Cloud Deployment (AWS EC2)

1. Launch Ubuntu EC2 instance
2. Install Docker & Docker Compose
3. Pull images from DockerHub
4. Run docker compose up -d
5. Access app via:

http://<EC2_PUBLIC_IP>

---

## 🔁 CI/CD Pipeline (GitHub Actions)

On every push to main:

1. Build Docker images
2. Push to DockerHub
3. Pull latest images on EC2

Workflow file:
.github/workflows/deploy.yml

---

## 📸 Screenshots

See screenshots/ folder for:

- CI/CD execution
- Docker image build & push
- Application deployment
- Working UI
- Nginx setup

---

## 👨‍💻 DockerHub Images

Backend:
https://hub.docker.com/r/sasi777/mean-backend

Frontend:
https://hub.docker.com/r/sasi777/mean-frontend

---

## 📌 Author

DevOps Internship Assignment – Discover Dollar