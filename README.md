# React DevOps Project

A React (Vite) application containerized with Docker and built through a Jenkins CI/CD pipeline.

## Tech Used
React, Vite, Docker, Jenkins, Git/GitHub

## Project Structure
- `src/`, `public/`, `index.html` – React (Vite) application
- `Dockerfile` – container image definition
- `Jenkinsfile` – CI/CD pipeline definition

## Pipeline Flow
Git push → Jenkins pipeline → Docker image build → <push / run container>

Pipeline stages: <Checkout, Build image, ...>

## Run Locally
```bash
git clone https://github.com/cloud-wazid/react-devops-project.git
cd react-devops-project
npm install
npm run dev
```

## Run with Docker
```bash
docker build -t react-devops-project .
docker run -d -p <PORT>:<PORT> react-devops-project
```

## Issues Solved
- Fixed Docker build configuration for the Vite app
- Fixed the Jenkins pipeline configuration
