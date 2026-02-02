 Dockerized Nginx Web Server

## Overview
A simple Docker project that runs an Nginx web server to serve static HTML content.  
This project demonstrates basic containerization, image creation, and port mapping using Docker.

## Tech Stack
- Docker
- Nginx (Alpine)
## Project Structure
```text
nginx-web-server/
├── Dockerfile
└── index.html

## Docker Design
Base image: nginx:alpine

Service: Single Nginx container

Web root: /usr/share/nginx/html

Port mapping: 80 (container) → 8080 (host)

## How to Run
docker build -t nginx-web-server .
docker run -d -p 8080:80 nginx-web-server

## Technical Highlights
- Dockerfile creation
- Official Docker images
- Static content serving
- Port mapping
