# Dockerized FastAPI Machine Learning API

## Overview
A production-style Docker project that deploys a data science API using FastAPI.  
The API serves machine learning predictions from a pre-trained model in a containerized environment.

## Tech Stack
- Docker
- Python
- FastAPI
- scikit-learn

## Project Structure
```text
fastapi-ml-api/
├── Dockerfile
├── requirements.txt
├── app.py
└── model.pkl
```
## Docker Design
- Base image: python:3.9-slim
- Service: Single FastAPI application container
- Application server: Uvicorn
- Port mapping: 8000 → 8000
- Model loading at application startup

## How to Run
docker build -t fastapi-app .
docker run -p 8000:8000 fastapi-app
## Access the API at:
http://localhost:8000
## Technical Highlights
- API containerization with FastAPI
- Deploying machine learning models as services
- Lightweight Docker images for production
- Running ASGI applications in containers
