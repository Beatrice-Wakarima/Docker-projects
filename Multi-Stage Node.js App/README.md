# Dockerized Node.js Multi-Stage App

## Overview
A Docker project demonstrating a **multi-stage build** for a Node.js application.  
This approach reduces image size by separating build and runtime environments.
## Tech Stack
- Docker
- Node.js
- Nginx

## Project Structure
```text
node-multi-stage/
├── Dockerfile
├── package.json
├── package-lock.json
└── server.js
```
## Docker Design
Base images:
Build stage: node:14
Run stage: node:14-slim
Single service: Node.js application
Ports: 3000 → 3000
Multi-stage build separates build dependencies from runtime

## How to Run
docker build -t node-multi-stage .
docker run -p 3000:3000 node-multi-stage
## Access the application at:
http://localhost:3000

## Technical Highlights
- Multi-stage Docker builds
- Image size optimization
- Node.js containerization
- Port mapping
