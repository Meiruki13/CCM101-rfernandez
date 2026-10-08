# Laboratory Activity 7: Mission 7 – The Cloud Operations Engineer

## Mission Overview
This lab focuses on observability — establishing a host server's baseline
health, deploying a containerized Nginx web server, generating both normal
and error traffic against it, and using Docker's logging and metrics tools
to prove the infrastructure is healthy and ready for a traffic surge.

## Objectives
- Use native Linux CLI tools to monitor host CPU, memory, and disk capacity
- Deploy a web container and track its real-time performance
- Generate web traffic and extract application access logs for analysis
- Translate raw performance data into a readable technical report

## Monitoring Commands Executed
- `free -h` — checked memory usage (1.9Gi total, 417Mi used, 1.5Gi available)
- `df -h` — checked root (/) disk storage (19G total, 5.5G used, 13G available, 30% used)
- `top` — viewed live CPU load and running processes
- `docker run -d --name client-website -p 8080:80 nginx` — deployed the Nginx container
- `curl http://localhost:8080` (x3) — simulated 3 successful visits (HTTP 200)
- `curl http://localhost:8080/hidden-admin-page` — simulated a broken request (HTTP 404)
- `docker logs client-website` — retrieved application logs, confirming the 200s and the 404
- `docker stats` — viewed real-time resource usage (CPU 0.00%, Memory 2.73MiB / 1.859GiB)

## Skills Learned
- Establishing a host-level performance baseline before deployment
- Generating and reading HTTP access logs, including error codes
- Reading live container resource metrics (CPU, memory, network I/O)
- Understanding the difference between monitoring (metrics) and logging (events)
