# 🐳 Docker Practice

Just me learning and experimenting with Docker — containerizing different kinds of apps and figuring out how to run them anywhere.

## 📌 What’s Inside

- **hello-docker/**  
  My very first Docker container. Simple and just to get the basics right.

- **react-docker/**  
  React app running inside a container.

- **next-docker/**  
  Next.js project with an optimized Dockerfile for development and production.

- **mern-docker/**  
  Full MERN stack (MongoDB + Express + React + Node) using Docker Compose so frontend, backend, and database all run in separate containers.

- **vite-project/**  
  Trying out a Vite app in Docker.

## 🛠 What I’m Learning
- Writing `Dockerfile` for Node.js, React, and Next.js apps.
- Using **Docker Compose** for multi-container setups.
- Optimizing builds to make images smaller & faster.
- Understanding volumes, ports, and networks in Docker.

##For the MERN stack:

cd mern-docker
docker-compose up --build


## 🚀 How to Run
Example for `hello-docker`:
```bash
cd hello-docker
docker build -t hello-docker .
docker run -p 3000:3000 hello-docker
