# Dockerized Full Stack App (Node.js + Express + MongoDB)

## 🚀 Project Overview
This project is a Dockerized backend application built using Node.js, Express.js, and MongoDB.  
It is deployed on an AWS EC2 instance using Docker Compose and runs on port 3000.

MongoDB data is persisted using a local `data` folder mounted as a Docker volume.

---

## 🛠️ Tech Stack
- Node.js
- Express.js
- MongoDB
- Docker
- Docker Compose
- AWS EC2

---

## ☁️ Deployment Platform
Deployed on Amazon Web Services (AWS EC2 instance).



## 🐳 Docker Setup

### Build and Run Containers

cmd:- docker-compose up -d --build

Stop Containers
cmd:- docker-compose down

After deployment, access the application using:
http://<EC2-PUBLIC-IP>:3000

Custom network used:

my-network

This allows communication between Node.js and MongoDB containers.

MongoDB data is stored using:

./data:/data/db

This ensures data persistence even after container restart or rebuild.
