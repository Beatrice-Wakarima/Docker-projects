# Dockerized TensorFlow Model

## Overview
A Docker project that containerizes a TensorFlow machine learning model to provide a portable and reproducible execution environment.

## Tech Stack
- Docker
- Python
- TensorFlow
## Project Structure
```text
tensorflow-model/
├── Dockerfile
└── model.py
```
## Docker Design
- Base image: tensorflow/tensorflow:latest
- Service: Single TensorFlow container
- Working directory: /app
- Model: Pre-trained MobileNetV2

## How to Run
docker build -t tensorflow-model .
docker run tensorflow-model
## Technical Highlights
- Machine learning model containerization
- Use of official TensorFlow Docker images
- Reproducible ML environments
- Running ML workloads in containers
