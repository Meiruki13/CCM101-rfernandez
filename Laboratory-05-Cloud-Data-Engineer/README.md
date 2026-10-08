# Laboratory Activity 5: Mission 5 – The Cloud Data Engineer

## Mission Overview

In this mission, I explored cloud storage and learned how object storage can be used to manage large amounts of data. I deployed MinIO using Docker, accessed its web console through KillerCoda, created a storage bucket, and uploaded a test file.

## Objectives

- Understand the differences between Block Storage, File Storage, and Object Storage
- Deploy MinIO using Docker
- Access a cloud storage service through port forwarding
- Create a bucket and upload objects using MinIO
- Document the deployment process using Markdown
- Add the completed work to my GitHub Cloud Computing portfolio

## Tools Used

- KillerCoda
- Docker
- MinIO
- Linux Terminal
- GitHub
- Markdown

## Skills Learned

Through this activity, I learned how different cloud storage types are used for different purposes. I also gained experience deploying a cloud storage server with Docker and accessing it through a web browser.

I learned how to create and manage a bucket in MinIO and upload files as objects. This activity also helped me become more comfortable with Linux commands, Docker containers, port forwarding, and documenting technical tasks using Markdown.

## MinIO Deployment

MinIO was deployed using Docker with ports `9000` and `9001`. Port `9001` was used to access the MinIO Web Console through KillerCoda's Traffic/Ports feature.

The `elestio/minio` image was used because the `minio/minio` image specified in the laboratory instructions could not be pulled successfully in the KillerCoda environment.

## Bucket Created

The bucket created for this activity was:

`client-photos`

This bucket was used to store the test file required for the activity.

## Conclusion

This activity gave me a better understanding of how cloud object storage works in a practical environment. Deploying MinIO with Docker and creating a bucket helped me see how object storage can be used to manage large amounts of files such as photos.

It also improved my confidence in using the Linux terminal and Docker commands. Overall, the activity helped me connect the concepts of cloud storage with an actual working deployment.
