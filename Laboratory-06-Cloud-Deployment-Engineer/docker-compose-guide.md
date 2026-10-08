# Docker Compose Guide — Nextcloud + MariaDB

## What does the `services:` block do?
It contains all the containers needed for the application stack. Each
service under `services:` such as `database` and `app` runs as its own
container with its own image, environment variables, and configuration.
Docker Compose uses this section to create and start all the services
together.

## How did the Nextcloud app container find the database container?
The Nextcloud app connects to the database using the
`MYSQL_HOST=database` environment variable. Docker Compose automatically
creates a private network for the services and allows each service name,
such as `database`, to work as a hostname. This allows the `app`
container to connect to the database without using a specific IP address.

## Difference between `docker run` and `docker-compose up -d`
The `docker run` command is used to create and start a single container,
with its configuration provided through command-line options. On the
other hand, `docker-compose up -d` reads the YAML configuration file and
starts all the services defined in it, including their networking and
environment settings. This makes it easier to manage applications that
use multiple containers.
