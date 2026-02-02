## Automating Data Pipelines with Apache Airflow & Docker
An advanced data engineering project focused on setting up and containerizing a multi-service Apache Airflow environment. This setup orchestrates complex data workflows using a local executor and a persistent PostgreSQL backend, all managed through Docker Compose.

## Tech Stack
Docker & Docker Compose
Apache Airflow
Python
PostgreSQL

## Project Structure
```text
airflow-docker/
├── dags/                # Directory for Python DAG definitions
├── docker-compose.yml   # Orchestration for Airflow services
└── README.md            # Project documentation
```
## Docker Design
Base Image: apache/airflow:latest
Database: Dedicated PostgreSQL container for metadata storage.
Executor: LocalExecutor for parallel task execution.
Port Mapping: 8080:8080 (Web UI) and 5432:5432 (Postgres).
Volumes: Local ./dags mapping for seamless pipeline development.

## How to Run
1. Initialize and Start
Run the following command from the project root to bring up the database, scheduler, and webserver:

```Bash
docker-compose up
```
2. Access the Airflow UI
Once the containers are healthy, open your browser and navigate to:

http://localhost:8080

## Concepts Demonstrated
Service Orchestration: Coordinating multiple containers (DB, Webserver, and Scheduler) to work as a unified system.
Workflow Automation: Scheduling and monitoring data tasks via Directed Acyclic Graphs (DAGs).
Environment Parity: Using Docker to ensure the pipeline runs identically across different development environments.
Infrastructure as Code: Defining the entire data engineering environment within a single docker-compose.yml file.
Persistent Storage: Managing database volumes to prevent data loss across container restarts.
