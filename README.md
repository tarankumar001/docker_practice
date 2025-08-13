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

## 🚀 How to Run

### For `hello-docker`
```bash
cd hello-docker
docker build -t hello-docker .
docker run -p 3000:3000 hello-docker
```

### For `react-docker`
```bash
cd react-docker
docker build -t react-docker .
docker run -p 3000:3000 react-docker
```

### For `next-docker`
```bash
cd next-docker
docker build -t next-docker .
docker run -p 3000:3000 next-docker
```

### For `vite-project`
```bash
cd vite-project
docker build -t vite-docker .
docker run -p 5173:5173 vite-docker
```

### For the `mern-docker` stack
```bash
cd mern-docker
docker-compose up --build
```

## 📅 Next Steps
- Push these images to **Docker Hub**.
- Try deploying a Dockerized app to the cloud.
- Automate builds using **GitHub Actions** or other CI/CD tools.

---

💬 *Feel free to fork, try them out, or drop me suggestions!*
