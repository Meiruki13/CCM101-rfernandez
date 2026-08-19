# Laboratory Activity 2: Mission 2 – Build the Cloud Infrastructure Blueprint

## Mission Overview
This activity focused on investigating a cloud-based Linux server,
identifying the core components of cloud infrastructure, comparing major
cloud providers, and designing a simple cloud architecture diagram.

## Objectives
- Explain the major components of cloud infrastructure
- Investigate hardware and software resources in a Linux environment
- Differentiate compute, storage, networking, and identity resources
- Interpret the relationship between cloud infrastructure components
- Create professional technical documentation using Markdown
- Continue building a structured GitHub Cloud Computing Portfolio

## Cloud Infrastructure Components
- **Compute:** processing power (VMs, containers, serverless functions)
- **Storage:** object, block, and file storage for data
- **Networking:** virtual networks, routers, firewalls, load balancers
- **Identity and Access Management (IAM):** controls who can access what

## Tools Used
- KillerCoda Playground (Ubuntu Linux environment)
- GitHub (portfolio repository)
- Draw.io (cloud architecture diagram)
- Official AWS, Azure, and GCP documentation

## Linux Commands Executed
- `cat /etc/os-release` – check OS version
- `uname -r` – check kernel version
- `lscpu` – check CPU information
- `nproc` – check number of CPU cores
- `free -h` – check total memory
- `df -h` – check disk space and mounted file systems
- `hostname` / `hostname -I` – check hostname and IP address

## Skills Learned
- Investigating and documenting Linux server specifications
- Understanding core cloud infrastructure components
- Comparing services across AWS, Azure, and GCP
- Designing a basic cloud architecture diagram
- Writing professional technical documentation in Markdown

## Challenges Encountered
One challenge I ran into was accidentally pasting an entire reference table
(with labels and command descriptions) directly into the terminal instead
of running each Linux command individually. This caused a string of "command
not found" errors since the shell tried to interpret the extra text as
commands. It taught me to slow down and copy only the exact command syntax
one line at a time, rather than copying formatted notes wholesale. I also
found it took some extra thought to clearly separate networking resources
from IAM when documenting the components, since both deal with controlling
access and connectivity in slightly overlapping ways — reviewing Chapter 2
again helped clarify that networking is about connectivity itself, while
IAM is specifically about permissions and identity.
