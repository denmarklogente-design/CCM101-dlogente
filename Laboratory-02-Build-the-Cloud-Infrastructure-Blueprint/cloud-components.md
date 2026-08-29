# Cloud Infrastructure Components

## Compute Resources

### Purpose

Compute resources are the processing resources of a cloud environment. They include components such as the CPU and memory that allow a server to perform operations and execute workloads.

### Why It Is Important

Compute resources are important because applications and system processes need processing power and memory to function. The available computing capacity affects the server's ability to handle tasks.

### Relation to the Linux Environment Provided by KillerCoda

In the KillerCoda environment, I examined the CPU model, number of CPU cores, and RAM. The information showed me the computing resources available in the Linux server for processing commands and running tasks.

## Storage Resources

### Purpose

Storage resources are used to keep system files, applications, configurations, and other data on a server.

### Why It Is Important

Storage is necessary because cloud systems need space to save information and retrieve it when applications or users require it.

### Relation to the Linux Environment Provided by KillerCoda

I used `df -h` to examine the available disk space and `findmnt` to identify the mounted file systems. These commands helped me understand how storage is being used and organized in the Linux server.

## Networking Resources

### Purpose

Networking resources allow servers, computers, users, and other services to exchange information.

### Why It Is Important

Networking is important because cloud resources must communicate with each other and with users in order to provide services and applications.

### Relation to the Linux Environment Provided by KillerCoda

I used the `hostname -I` command to check the IP addresses of the KillerCoda Linux environment. This helped me understand how the server is identified within its network.

## Operating System

### Purpose

The operating system manages the hardware and software resources of the server and provides a platform for applications and commands.

### Why It Is Important

The operating system is important because it coordinates system resources and provides the environment needed for users and applications to interact with the server.

### Relation to the Linux Environment Provided by KillerCoda

KillerCoda provided an Ubuntu Linux environment where I could use the terminal to investigate the server. Through Linux commands, I was able to examine its compute, storage, networking, and system information.

