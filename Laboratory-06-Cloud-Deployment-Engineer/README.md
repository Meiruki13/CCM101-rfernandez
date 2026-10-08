# Laboratory Activity 6: Mission 6 – The Cloud Deployment Engineer

## Mission Overview
This laboratory introduces Infrastructure as Code (IaC) through Docker Compose,
where a two-tier private cloud storage application (Nextcloud + MariaDB) is
deployed using a single YAML configuration file instead of setting up each
container manually.

## Objectives
- Explain the basic concept of multi-tier application architecture
- Understand the purpose and structure of a docker-compose.yml file
- Use nano to create and edit configuration files through the command line
- Deploy a multi-container application using Docker Compose
- Document the deployment process and IaC concepts in Markdown

## Commands Executed
- `mkdir nextcloud-deployment`, `cd nextcloud-deployment`
- `nano docker-compose.yml`
- `docker-compose up -d`
- `docker-compose ps`
- `docker-compose down`

## Skills Learned
- Creating a properly formatted and correctly indented YAML configuration file
- Deploying multiple connected containers using a single command
- Understanding how Docker Compose uses internal networking and DNS resolution
  to allow containers to communicate using their service names
- Documenting Infrastructure as Code in a clear way for other developers and engineers
