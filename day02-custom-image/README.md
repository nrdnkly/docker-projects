# Day 02 - Custom Docker Image

## 📌 Project Overview

In this project, I learned how to create a custom Docker image using a Dockerfile.

Instead of using a pre-configured container directly from Docker Hub, I built my own image based on Nginx and served a custom HTML page.

## 🎯 Learning Objectives

- Understand Dockerfile structure
- Build custom Docker images
- Use the `FROM`, `COPY`, and `EXPOSE` instructions
- Run containers from custom images
- Publish container ports to the host machine

## 📂 Project Structure

```
day02-custom-image/
├── Dockerfile
├── index.html
└── README.md
```

## 🐳 Dockerfile

```dockerfile
FROM nginx:latest

COPY index.html /usr/share/nginx/html/index.html

EXPOSE 80
```

## 🚀 Build the Image

```bash
docker build -t day02-container .
```

## ▶️ Run the Container

```bash
docker run -d -p 8081:80 --name nurdan-day02 day02-container
```

## 🌐 Access the Application

Open your browser and visit:

```text
http://localhost:8081
```

## 📝 What I Learned

- How Docker images are built layer by layer
- How to customize an existing image
- How files are copied into containers
- The difference between Docker images and containers
- How port mapping works

## 📚 Commands Used

```bash
docker build -t day02-container .

docker images

docker run -d -p 8081:80 --name nurdan-day02 day02-container

docker ps

docker stop nurdan-day02

docker rm nurdan-day02
```

## ✅ Status

Completed successfully.

Day 02 of my Docker Learning Journey 🚀
