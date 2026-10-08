# Reflection

Writing a docker-compose.yml file makes the work of a cloud engineer
much easier compared to manually entering commands. The whole
application setup, including containers, environment variables, ports,
and dependencies, can be placed in one organized file. Instead of
remembering and entering separate docker run commands, one command can
start the entire application. The file can also be used as documentation,
saved in version control, shared with others, and reused in different
environments.

If there is an indentation mistake in a YAML file, such as using a Tab
instead of spaces, Docker Compose may not be able to read the file
properly. It can result in a syntax error and prevent the containers
from starting because YAML uses indentation to determine how different
settings are organized under each service. This is why proper and
consistent spacing is important when creating a Compose file.

We used environment variables such as MYSQL_PASSWORD in the Compose
file to avoid placing sensitive information directly in the application
configuration. This makes credentials easier to manage and allows the
same Docker image to be used in different environments by changing the
environment variables. It also helps prevent sensitive information from
being stored in version control when values are provided through an
external .env file.

Deploying a working enterprise cloud storage system within a few
minutes gave me a better idea of what cloud engineers do in real-world
situations. The process of creating a private "Google Drive" alternative
was made much simpler because most of the setup was handled through the
Compose file. This showed me how Infrastructure as Code can reduce the
complexity of managing infrastructure.

Since Mission 1, my understanding of cloud computing has changed from
simply thinking of it as "someone else's computer" to seeing it as a
system based on repeatable and automated infrastructure. I started with
provisioning a single VM, then worked with storage, and now I can
orchestrate multiple connected containers using code instead of
performing every step manually.
