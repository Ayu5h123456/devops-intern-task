DevOps Intern Task

## Project Overview
This project demonstrates containerization, CI/CD automation, and cloud deployment using Docker and AWS.

The application is a simple Node.js server that displays:

Hello from DevOps Intern

---

## Tech Stack
- Node.js
- Docker
- GitHub Actions (CI/CD)
- AWS EC2
- AWS CloudWatch
- AWS SNS

---

## Application Structure
.
├── app.js
├── package.json
├── Dockerfile
└── README.md

## 🐳 Docker Setup

### Build Image
```bash
docker build -t devops-intern-task .
```

### Run Container
```bash
docker run -p 3000:3000 devops-intern-task
```

Access:
http://localhost:3000

---

## 🔄 CI/CD Pipeline

GitHub Actions automatically builds the Docker image on every push to the main branch.

Workflow file:
```
.github/workflows/docker.yml
```

---

## ☁️ Cloud Deployment

The application is deployed on AWS EC2 with:

- Docker container runtime
- CloudWatch CPU monitoring
- SNS alert notification when CPU exceeds 70%
