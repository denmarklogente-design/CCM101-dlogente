# Reflection

Object storage is more suitable for millions of photos because it is designed to handle large amounts of unstructured data. Instead of treating every photo like part of a traditional hard drive, object storage saves each photo as an object with its own information and identifier. This makes it practical for applications that need to store and manage a large number of images.

Docker made the MinIO deployment easier because I did not have to manually install all of the required components. I was able to download the MinIO image and create a running container using a single Docker command. The command also allowed me to configure the ports and administrator credentials at the same time.

A bucket is a container used by object storage to organize and store objects. In this activity, I created a bucket named `client-photos` and used it to store the sample file that I uploaded through the MinIO Web Console.

Enterprises can protect object storage data from physical server failures by using methods such as replication, redundancy, backups, and multiple storage locations. Having additional copies of important data helps reduce the possibility of losing information when a server or storage device fails.

My confidence with Linux command-line tools improved through this activity because I was able to use several Docker commands and understand their output. Commands such as `docker pull`, `docker run`, and `docker ps` helped me download the required image, start the MinIO service, and check whether the container was running. I also learned that checking the command output carefully is important when troubleshooting a cloud deployment.
