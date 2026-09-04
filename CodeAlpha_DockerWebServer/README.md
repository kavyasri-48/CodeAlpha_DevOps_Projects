# CodeAlpha Docker Web Server

## Project Overview

This project demonstrates how to deploy a custom web page inside a **Docker container using the Nginx web server**.

A Docker image is created using an Nginx base image, the custom HTML/CSS webpage is copied into the Nginx web directory, and the application is exposed through port mapping.

## Architecture

```text
Client Browser
      |
      | localhost:8081
      v
Docker Container
      |
      v
Nginx Web Server
      |
      v
Custom HTML/CSS Webpage
```

## Technologies Used

* Docker
* Nginx
* Linux / Ubuntu
* HTML
* CSS
* Git
* GitHub

## Implementation

1. Created a custom HTML/CSS webpage.
2. Created a `Dockerfile` using the official Nginx image.
3. Copied the webpage into the Nginx web directory.
4. Built the Docker image.
5. Created and started a Docker container.
6. Configured port mapping from the host to the Nginx container.
7. Verified the running container using Docker commands.
8. Accessed the webpage through the browser.

## Dockerfile

The Dockerfile uses the official **Nginx image** as the base image and copies the custom webpage into the Nginx web root directory.

Example:

```dockerfile
FROM nginx:latest

COPY index.html /usr/share/nginx/html/index.html
```

## Build the Docker Image

```bash
docker build -t docker-web-server .
```

This command creates a Docker image named `docker-web-server`.

## Run the Container

```bash
docker run -d -p 8081:80 --name docker-web-server docker-web-server
```

Here:

* `-d` runs the container in detached mode.
* `-p 8081:80` maps host port `8081` to container port `80`.
* `--name docker-web-server` assigns a name to the container.

## Check the Running Container

```bash
docker ps
```

This command displays the running Docker containers and their port mappings.

## Access the Web Server

Open the following URL in a browser:

```text
http://localhost:8081
```

The custom HTML/CSS webpage is served by Nginx from inside the Docker container.

## Useful Docker Commands

```bash
docker images
docker ps
docker logs docker-web-server
docker stop docker-web-server
docker start docker-web-server
docker rm docker-web-server
```

## Screenshots

### Docker Webpage

![Docker Webpage](screenshots/docker-webpage.png)

### Docker Commands

![Docker Commands](screenshots/docker-commands.png)

## Result

Successfully deployed and accessed a custom HTML/CSS webpage through an **Nginx web server running inside a Docker container**.

## Key DevOps Concepts

* Containerization
* Docker images
* Docker containers
* Dockerfile
* Docker build
* Docker run
* Port mapping
* Nginx web server
* Container lifecycle
* Linux command-line operations
* Basic troubleshooting
* Git and GitHub

## Learning Outcome

This project provided hands-on experience with **Docker containerization, Nginx web servers, Docker image creation, container management, port mapping, and Linux command-line operations**.

## Internship Project

**CodeAlpha — DevOps Internship**

**Project:** Docker Web Server

