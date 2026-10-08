MinIO Deployment Documentation
Docker Command Used
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
elestio/minio server /data --console-address ":9001"

Port Used to Access the Web Console
Port 9001 — accessed through KillerCoda's "Traffic/Ports" tab to open
the MinIO Web Console in the browser.
Bucket Created
client-photos
What the -e Flags Did
The -e flag is used to define environment variables when the container starts.
In this command:
- MINIO_ROOT_USER=cloudadmin sets the administrator username used to access
  the MinIO console
- MINIO_ROOT_PASSWORD=CloudNova2026! sets the administrator password
These environment variables allow MinIO's login credentials to be configured
during deployment, making the container reusable while keeping its credentials
configurable for each deployment.
