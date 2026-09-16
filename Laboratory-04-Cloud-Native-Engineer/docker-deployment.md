# Docker Deployment Log

## Commands Used to Deploy Nginx

- `docker pull nginx` – Downloaded the official Nginx image from Docker Hub.
- `docker run -d -p 8080:80 nginx` – Created and started an Nginx container in the background, mapping host port `8080` to container port `80`.
- `docker ps` – Displayed the currently running Nginx container.

## Container Lifecycle Commands

- `docker stop d647d02db78f` – Attempted to stop the Nginx container.
- `docker ps -a` – Listed all containers and checked the container status.
- `docker stop <container_id>` – Attempted to use the placeholder command, which resulted in a syntax error.
- `docker stop <container_id> d647d02db78f` – Attempted to stop the container but resulted in an error.
- `docker stop d647d02db78f` – Successfully stopped the Nginx container.
- `docker ps -a` – Confirmed that the container status changed to `Exited (0)`.
- `docker rm d647d02db78f` – Permanently removed the stopped Nginx container.

## Final Container Information

- **Container ID:** `d647d02db78f`
- **Image:** `nginx`
- **Container Name:** `eloquent_hellman`
- **Port Mapping:** `0.0.0.0:8080 → 80/tcp`
- **Final Status:** Container stopped and removed successfully.

## Technologies Used

- Docker
- Nginx
- Ubuntu Linux
- Docker Hub

## Deployment Summary

The Nginx Docker container was successfully created, started, stopped, and removed using Docker commands. The deployment also demonstrated basic Docker container lifecycle management.
