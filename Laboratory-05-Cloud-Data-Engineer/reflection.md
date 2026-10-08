# Reflection

### 1. Why is object storage better suited for storing millions of photos compared to a traditional block storage hard drive?
Block storage works like a regular hard drive connected to a VM and is mainly designed for fast and structured data. However, it is not the best choice for storing huge amounts of unstructured files. Object storage uses scalable buckets where each photo is stored as an object with its own ID and metadata. This makes it a better option for storing millions of photos that mainly need to be uploaded, stored, and accessed when needed.

### 2. How did using Docker make it easier to deploy the MinIO storage server?
Docker made deploying MinIO easier because I did not need to manually install the software, configure dependencies, or set up the network separately. I was able to run the storage server using a single command. The `-e` flags were used to set the administrator credentials, while the `-p` flags were used to expose the required ports.

### 3. What is a "bucket" in the context of cloud storage?
A bucket is a main container in object storage where files, also called objects, are stored. Unlike a traditional file system that uses folders and subfolders, objects are stored inside the bucket and can be identified using their unique IDs and metadata.

### 4. How do you think large enterprise companies ensure their object storage data is not lost if the physical server crashes?
Large companies can protect their data by keeping multiple copies across different storage drives, servers, or locations. If one physical server fails, another copy can still be used to recover the data. Companies can also maintain separate backups to protect against problems such as accidental deletion, hardware failure, or corrupted files.

### 5. How is your confidence in navigating the Linux command line growing?
After completing five labs, I feel more comfortable using the Linux command line compared to when I first started. At the beginning, I was still getting used to basic commands like `ls` and `cd`, but now I can use Docker commands and manage containers through the terminal. Being able to deploy a working server using commands has made the terminal feel less intimidating and more useful.

**Reference:**
University of Eastern Pangasinan – College of Information Technology.
(2026). *CCM101 – Cloud Computing, Midterm Module, Chapter 5.*
