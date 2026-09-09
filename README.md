# Laboratory Activity 3: Mission 3 – Become a Multi-Cloud Explorer

## Mission Overview
In this activity, I explored the world's three leading public cloud
platforms — AWS, Microsoft Azure, and Google Cloud Platform — compared
their core services and strengths, and practiced recommending the right
platform for different business scenarios, much like a real Cloud
Solutions Architect would.

## Objectives
- Explore the major public cloud platforms
- Identify the core services offered by AWS, Microsoft Azure, and GCP
- Compare cloud services across different providers
- Analyze business requirements and recommend appropriate cloud solutions
- Create professional technical documentation using Markdown
- Continue developing a well-organized GitHub Cloud Computing Portfolio

## Tools Used
- KillerCoda Playground (Ubuntu Linux environment)
- GitHub (portfolio repository)
- Official AWS, Microsoft Azure, and Google Cloud Platform documentation

## Linux Investigation & Cloud Migration Recommendation (Checkpoint 7)

Findings from my KillerCoda environment:
- **Operating System:** Ubuntu 24.04.4 LTS (Noble Numbat)
- **CPU Information:** Intel Xeon E312xx (Sandy Bridge, IBRS update), BIOS model HVAG-9.6.0 PC (Q35 + ICH9, 2009), CPU @ 2.0GHz
- **Memory:** 1.9Gi total, 416Mi used, 823Mi free, 1.5Gi available
- **Disk Space:** 19G total on `/`, 5.4G used, 13G available (30% used)

**If this Linux server were migrated to the cloud, which AWS, Azure, and GCP services could host it?**

Given this is a lightweight, single-core Ubuntu server with modest RAM
and disk space, it maps closely to each provider's smallest
general-purpose virtual machine tier:
- **AWS:** Amazon EC2 (e.g., a `t3.micro` or `t2.micro` instance), with
  Amazon EBS for disk storage
- **Azure:** Azure Virtual Machines (e.g., a `B1s` burstable-tier VM),
  using Azure Managed Disks for storage
- **GCP:** Google Compute Engine (e.g., an `e2-micro` instance), using
  Persistent Disk for storage

All three providers offer free-tier or low-cost VM options well-suited
to a small workload like this one, since its specs comfortably fit
within each provider's entry-level instance types.

## Skills Learned
- Researching and comparing public cloud platforms using official documentation
- Matching equivalent services across AWS, Azure, and GCP
- Recommending cloud solutions based on business requirements
- Relating a real Linux environment's specs to equivalent cloud VM offerings
- Writing structured, professional technical documentation in Markdown
