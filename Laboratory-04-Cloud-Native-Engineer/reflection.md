# Reflection

### 1. How does the boot time and setup process of a Docker container compare to installing an operating system on a Virtual Machine?
It's dramatically faster. A VM has to boot an entire guest operating
system from scratch, which can take minutes, and installing/configuring
software like a web server on top of that could add even more time. A
Docker container skips all of that — since it shares the host's kernel
instead of booting its own OS, running `docker run` and having Nginx
fully up and serving requests took seconds, not minutes.

### 2. Why is port mapping (-p 8080:80) necessary when running a web server inside a container?
Nginx listens on port 80 *inside* the container by default, but that
container has its own isolated network namespace — port 80 inside it
isn't automatically reachable from outside. The `-p 8080:80` flag creates
a bridge, forwarding traffic that hits port 8080 on the actual host
machine into port 80 inside the container. Without it, the container
would be running, but there'd be no way to actually reach it from
`localhost`.

### 3. What happens to the data inside a container when you use the docker rm command?
Any data inside the container's writable layer is permanently deleted
once `docker rm` runs — a container's filesystem only exists as long as
the container itself does. This is why persistent data (databases, user
uploads, etc.) shouldn't be stored only inside a container's own
filesystem; it should live in something like a Docker volume that exists
independently of any single container's lifecycle.

### 4. How do you think containerization changes the way software developers and IT operations teams work together (DevOps)?
It removes a huge source of friction between the two: the classic "it
works on my machine" problem. Since a container packages the application
together with everything it needs to run, a developer's container behaves
identically whether it's tested locally, in staging, or deployed to
production. This means operations teams aren't stuck troubleshooting
environment differences, and containers fit naturally into automated
CI/CD pipelines — which is a big part of why containerization and DevOps
practices tend to go hand in hand.

### 5. How is your GitHub portfolio evolving?
Four labs in now, and the portfolio's covering real ground — Linux basics
in Lab 1, infrastructure investigation in Lab 2, multi-cloud comparison in
Lab 3, and now actual container deployment in Lab 4. It's starting to look
less like a stack of separate assignments and more like a genuine record
of hands-on cloud engineering skills building on each other.
