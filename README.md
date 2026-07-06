# ELK Stack Monitoring with Nginx & Filebeat

## Project Overview

This project demonstrates how to deploy a React portfolio website using Docker and Nginx while collecting and monitoring container logs with Filebeat, Elasticsearch, and Kibana.

The project is deployed on an AWS EC2 instance and provides centralized log monitoring using the ELK Stack.

## Architecture

```
                Internet
                    │
                    ▼
             AWS EC2 Instance
                    │
      ┌─────────────┴─────────────┐
      │                           │
      ▼                           ▼
 Docker Nginx Container      Filebeat Container
      │                           │
      └──────────► Elasticsearch ◄──────────┘
                          │
                          ▼
                       Kibana
```

## Tech Stack

- AWS EC2
- Docker
- Docker Compose
- Nginx
- React + Vite
- Elasticsearch
- Kibana
- Filebeat
- Linux (Ubuntu)

## Features

- Dockerized React application
- Nginx as web server
- ELK Stack for centralized logging
- Filebeat collects Docker container logs
- Elasticsearch stores logs
- Kibana visualizes logs
- Real-time monitoring

## Project Structure

```text
elk-stack-monitoring/
├── docker-compose.yml
├── README.md
├── filebeat/
│   └── filebeat.yml
├── docs/
│   ├── installation.md
│   └── architecture.md
├── screenshots/
└── dist/
```
