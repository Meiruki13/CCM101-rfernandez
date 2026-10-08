# MinIO Deployment Documentation

## Docker Command Used
```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
elestio/minio server /data --console-address ":9001"

## Port Used to Access the Web Console
Port 9001 — accessed through KillerCoda's "Traffic/Ports" tab to open
the MinIO Web Console in the browser.
Port 9000 is used for the MinIO server, while port 9001 is used
for the MinIO Web Console.
## Bucket Created
client-photos
The client-photos bucket was created in the MinIO Web Console to store
the test file required for the activity.
## What the -e Flags Did
The -e flag is used to set environment variables when the container starts.
In this command:
- MINIO_ROOT_USER=cloudadmin sets the administrator username used to log into
  the MinIO console
- MINIO_ROOT_PASSWORD=CloudNova2026! sets the administrator password
These environment variables allow the MinIO login credentials to be configured
during deployment. This makes the container reusable while allowing the
credentials to be configured for each deployment.
