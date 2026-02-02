# Docker Projects Portfolio
## Overview
This repository contains a curated collection of Docker projects demonstrating practical containerization skills across beginner, intermediate, and advanced levels.  
The projects progress from single-container setups to multi-container applications, data science environments, and production-style data engineering workflows.

Each project is self-contained and documented individually.

## Skills & Concepts Demonstrated
- Dockerfile design and best practices
- Use of official and minimal base images
- Container networking and port mapping
- Volume management and persistence
- Multi-container orchestration with Docker Compose
- Multi-stage builds and image optimization
- Containerized data science and machine learning workflows
- Workflow orchestration with Apache Airflow
- API deployment with FastAPI

## Beginner Projects

| Project | Description | Key Concepts |
|------|------------|--------------|
| [Nginx Web Server](./nginx-web-server) | Static website served via Nginx in a Docker container | Dockerfile, Port Mapping |
| [Python Script Container](./python-script) | Containerized Python script for CSV data processing | Dependencies, Volumes |
| [Flask + MySQL App](./flask-mysql-app) | Simple multi-container web app using Docker Compose | Compose, Networking |

## Intermediate Projects

| Project | Description | Key Concepts |
|------|------------|--------------|
| [Node.js Multi-Stage Build](./node-multi-stage) | Optimized Node.js app using multi-stage builds | Image Optimization |
| [TensorFlow Model Container](./tensorflow-model) | Portable TensorFlow model execution environment | ML Containerization |
| [Jupyter Data Science Environment](./jupyter-ds-env) | Reproducible Jupyter environment with Docker | Data Science Setup |

## Advanced Projects

| Project | Description | Key Concepts |
|------|------------|--------------|
| [Optimized Python Image](./optimized-python-app) | Reduced Docker image size using Alpine and multi-stage builds | Performance Optimization |
| [PyTorch Pipeline](./pytorch-pipeline) | Containerized deep learning inference pipeline | GPU-ready Images |
| [Airflow Data Pipelines](./airflow-docker) | Dockerized Apache Airflow with PostgreSQL backend | Workflow Orchestration |
| [FastAPI ML API](./fastapi-ml-api) | Production-style data science API deployment | API Containerization |

## Repository Structure
```text
docker-projects/
├── nginx-web-server/
├── python-script/
├── flask-mysql-app/
├── node-multi-stage/
├── tensorflow-model/
├── jupyter-ds-env/
├── optimized-python-app/
├── pytorch-pipeline/
├── airflow-docker/
├── fastapi-ml-api/
└── README.md
