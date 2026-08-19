# Cloud Infrastructure Components

## Compute Resources
**Purpose:** Compute resources provide the processing power needed to run
applications, execute calculations, and operate the operating system itself.
They are commonly delivered as virtual machines, containers, or serverless
functions.

**Why it matters in cloud computing:** Compute is the foundation of any
cloud workload — without processing power, no application can run. Cloud
providers let organizations scale compute vertically (more CPU/RAM) or
horizontally (more VMs) on demand, instead of purchasing physical servers.

**Relation to KillerCoda:** The KillerCoda playground itself is a virtual
machine — a compute resource provisioned on demand, giving me a full Linux
environment without owning any physical hardware.

## Storage Resources
**Purpose:** Storage resources provide space to store the operating system,
application files, and data. Cloud storage comes in different types: object,
block, and file storage.

**Why it matters in cloud computing:** Storage needs to be reliable,
scalable, and available from anywhere. Cloud storage removes the limits of
physical disks by distributing data across multiple systems for durability.

**Relation to KillerCoda:** The disk space shown by `df -h` in my playground
is a block storage allocation attached to my virtual machine, similar to how
a cloud VM's root volume works in AWS, Azure, or GCP.

## Networking Resources
**Purpose:** Networking resources allow communication between virtual
machines, storage systems, cloud services, and end users — this includes
virtual networks, routers, firewalls, and load balancers.

**Why it matters in cloud computing:** Without networking, isolated compute
and storage resources couldn't work together or be reached by users. Proper
network design also protects systems against unauthorized access.

**Relation to KillerCoda:** My playground has its own hostname and IP
address (found using `hostname` and `hostname -I`), representing how it's
networked within KillerCoda's underlying cloud infrastructure so I can
access it remotely through my browser.

## Operating System
**Purpose:** The operating system manages hardware resources, runs
applications, and provides the interface (in this case, a Linux terminal)
through which I interact with the machine.

**Why it matters in cloud computing:** Most cloud servers run Linux
distributions because they're lightweight, stable, and widely supported.
The OS is the layer where cloud engineers configure, secure, and manage
everything else.

**Relation to KillerCoda:** My playground runs Ubuntu 24.04.4 LTS,
confirmed using `cat /etc/os-release` — this is the same type of Linux
distribution commonly deployed on real cloud virtual machines in AWS EC2,
Azure VMs, or Google Compute Engine.
