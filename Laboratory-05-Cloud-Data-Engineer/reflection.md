Reflection
1. Why is object storage better suited for storing millions of photos compared to a traditional block storage hard drive?
Block storage works like a raw hard drive connected to a VM. It is useful for fast and structured data, but it is not ideal for handling huge amounts of unstructured files. Object storage uses scalable buckets where each file is stored as an object with its own ID and metadata. This makes it more suitable for storing millions of photos that mainly need to be uploaded, stored, and accessed when needed.
2. How did using Docker make it easier to deploy the MinIO storage server?
Docker made the deployment much easier because I did not have to manually install MinIO, configure its dependencies, or set up the network separately. With one command, I was able to create and run the MinIO server. The -e flags were used to set the administrator credentials, while the -p flags exposed the required ports.
3. What is a "bucket" in the context of cloud storage?
A bucket is a main container in object storage where files, also called objects, are stored. Instead of using a traditional folder structure, objects are stored inside the bucket and can be identified using their unique IDs and metadata.
4. How do you think large enterprise companies ensure their object storage data is not lost if the physical server crashes?
Large companies can protect their data by keeping multiple copies across different drives, servers, or locations. This way, if one physical server fails, the data can still be recovered from another copy. They can also use backups in addition to replication to protect against accidental deletion or corrupted files.
5. How is your confidence in navigating the Linux command line growing?
After five labs, I feel more comfortable using the Linux command line compared to when I started. At first, I was still getting familiar with basic commands like ls and cd, but now I can use Docker commands and manage containers through the terminal. Deploying a working server using commands has also made the terminal feel less intimidating and more useful.
