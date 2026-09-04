# Docker Web Server

## Project Overview

A simple web server deployed inside a Docker container using Nginx.
## Architecture

Client Browser
      |
      v
localhost:8080
      |
      v
Docker Container
      |
      v
Nginx Web Server
      |
      v
index.html

## Technologies Used


- Linux / Ubuntu
- Docker
- Nginx
- HTML
- CSS
- Git
- GitHub

## Docker Concepts Practiced

- Docker images
- Docker containers
- Dockerfile
- Docker build
- Docker run
- Port mapping
- Container lifecycle
- Container logs
- Container monitoring
- Troubleshooting

## Dockerfile

The Dockerfile uses the Nginx image as the base image and copies the
HTML webpage into the Nginx web directory.

## Build the Image

```bash
docker build -t docker-web-server .
