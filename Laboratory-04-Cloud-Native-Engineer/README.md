# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

In this laboratory activity, I learned about Virtual Machines, containers, and basic Docker operations. I used KillerCoda to check Docker, deploy an Nginx web server, and manage the container lifecycle. I also documented my work and organized the screenshots in my GitHub portfolio.

## Objectives

* Understand the difference between Virtual Machines and containers.
* Learn the basic concepts of containerization.
* Verify Docker in a Linux environment.
* Download and run an Nginx container.
* Test a web server using curl.
* Practice starting, stopping, and removing containers.
* Document the activity using Markdown and GitHub.

## Docker Commands Executed

### Docker Verification

```bash
docker --version
docker info
```

### Nginx Deployment

```bash
docker pull nginx
docker run -d --name nginx-server -p 8080:80 nginx
curl http://localhost:8080
```

### Container Lifecycle

```bash
docker ps
docker stop nginx-server
docker ps
docker rm nginx-server
docker ps -a
```

## Skills Learned

I learned how to verify a Docker installation, download Docker images, create containers, and run applications inside containers. I also learned how port mapping works and how to use basic Docker commands for managing containers. In addition, I practiced documenting technical work using Markdown and GitHub.

## Challenges Encountered

One challenge I experienced was understanding the different Docker commands and their purpose. I also needed to understand how the host port and container port work together when running Nginx. After testing the container using curl and checking the container lifecycle, I became more familiar with the basic Docker workflow.

