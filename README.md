AI Home Lab with Docker
This repository provides a comprehensive setup for deploying an AI home lab environment using Docker. It includes two primary services:

Ollama: A conversational AI and language model API.
Text Generation WebUI: A web-based interface for running and interacting with text generation models.
The setup is designed with modularity and ease of use in mind, allowing you to spin up both services quickly in isolated Docker containers. The structure mirrors a microservices lab environment, similar to the OpenTelemetry demo, facilitating a scalable and flexible approach for experimenting with AI models on your local machine.

Key features:

Dockerized Deployment: Each service is containerized, ensuring isolated environments and easy management.
Configurable Settings: Environment variables and configuration files allow for customizable setups and integrations.
Persistence & Data Management: Persistent storage for model data and logs, maintaining state between sessions.
This repository is ideal for AI enthusiasts and developers looking to experiment with and run AI-powered applications on their local machines.

# AI Home Lab

This repository sets up an AI home lab with Ollama and Text Generation WebUI, running in a Docker environment. 

## Requirements

- Docker and Docker Compose
- Git

## File Structure

```plaintext
ai-home-lab/
├── README.md
├── docker-compose.yml
├── ollama/
│   ├── Dockerfile
│   ├── config/
│   │   └── ollama_config.yaml
│   ├── data/
│   └── scripts/
│       └── ollama_start.sh
├── textgen-webui/
│   ├── Dockerfile
│   ├── config/
│   │   └── textgen_config.json
│   ├── data/
│   └── scripts/
│       └── textgen_start.sh
└── .env
