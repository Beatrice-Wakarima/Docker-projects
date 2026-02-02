# Dockerized Python Script

## Overview
A Docker project that containerizes a Python script for processing CSV data using pandas.  
This setup ensures the script can run consistently in any environment.
## Tech Stack
- Docker
- Python 3.9
- pandas
## Project Structure
```text
python-script/
├── Dockerfile
├── requirements.txt
├── process_data.py
└── data/
    └── data.csv
```
## Docker Design
Base image: python:3.9-slim
Service: Single Python container
Working directory: /app
Volume: Host data/ → Container /app/data

## How to Run
docker build -t python-script .
docker run -v $(pwd)/data:/app/data python-script
Technical Highlights
- Dockerfile creation for Python scripts
- Dependency management with requirements.txt
- Volume mounting for input data


