# Laboratory Activity 4: Mission 4 – The Cloud-Native Engineer

## Mission Overview

In this activity, I explored the difference between traditional virtualization and containerization. I also learned about the architectural differences between Virtual Machines (VMs) and containers. Using the KillerCoda environment, I deployed and managed a containerized Nginx web server with Docker.

## Objectives

- Differentiate between traditional Virtual Machines (VMs) and Containers
- Access a Docker-enabled cloud environment using KillerCoda
- Execute fundamental Docker CLI commands
- Pull, run, manage, and terminate a containerized Nginx application
- Create professional technical documentation using Markdown
- Continue developing a well-organized GitHub Cloud Computing Portfolio

## Docker Commands Executed

- `docker version` – checked the installed Docker version
- `docker info` – checked the current status of the Docker environment
- `docker pull nginx` – downloaded the official Nginx image from Docker Hub
- `docker run -d -p 8080:80 nginx` – created and started the Nginx container in the background
- `curl http://localhost:8080` – verified that the Nginx web server was responding
- `docker ps` – listed the currently running containers
- `docker stop d647d02db78f` – stopped the running Nginx container
- `docker ps -a` – listed all containers and verified that the container had stopped
- `docker rm d647d02db78f` – removed the stopped Nginx container

## Container Information

- **Container ID:** `d647d02db78f`
- **Image:** `nginx`
- **Container Name:** `eloquent_hellman`
- **Port Mapping:** `8080:80`
- **Final Status:** Container stopped and removed successfully

## Skills Learned

- Understanding the architectural difference between VMs and containers
- Checking the Docker installation and environment status
- Pulling images from Docker Hub
- Creating and running Docker containers
- Mapping a host port to a container port
- Viewing running and stopped containers
- Managing the Docker container lifecycle
- Using Markdown to document technical activities

## Challenges Encountered

One challenge I encountered was understanding how to properly stop the Docker container. I initially used `<container_id>` as a placeholder in the command, which caused a syntax error. I then learned that I needed to use the actual container ID, which was `d647d02db78f`. After using the correct ID, I successfully stopped and removed the container.

Another challenge was understanding port mapping. The command `-p 8080:80` connects port `8080` on the host machine to port `80` inside the Nginx container. This allowed me to access the Nginx web server through port `8080`.

## Deployment Summary

The activity successfully demonstrated the basic Docker container lifecycle. I pulled the Nginx image, created and ran a container, checked its status, stopped it, and finally removed it from the Docker environment.

## Technologies Used

- Docker
- Nginx
- Ubuntu Linux
- KillerCoda
- Docker Hub
- Markdown
- GitHub
