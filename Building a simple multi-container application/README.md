# Dockerized Flask + MySQL Application

## Overview
A multi-container Docker project using Flask as a web application and MySQL as the backend database.  
Docker Compose is used to orchestrate and manage the services.
## Tech Stack
- Docker
- Docker Compose
- Flask
- MySQL
## Project Structure
```text
flask-mysql-app/
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── app.py
```
## Docker Design

- Services:
  - web: Flask application
  - db: MySQL database

- Base images:
  - Flask: python:3.9-slim
  - MySQL: mysql:5.7

- Ports:
  - Flask: 5000 → 5000
  - MySQL: 3306 → 3306

- Volumes:

  - db_data → /var/lib/mysql

  - Application code mounted to /app

## How to Run
docker-compose up --build


## Access the application at:

http://localhost:5000

## Technical Highlights
- Multi-container applications
- Docker Compose orchestration
- Container networking
- Service dependencies
- Persistent volumes
