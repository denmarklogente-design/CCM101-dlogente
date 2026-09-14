# Docker Deployment

## Checkpoint 3 - Docker Verification

### 1. Check Docker Version

```bash
docker --version
```

This command checks if Docker is installed and shows the Docker version available in the environment.

### 2. Check Docker Information

```bash
docker info
```

This command displays information about the Docker environment and helps verify that Docker is working properly.

## Checkpoint 4 - Nginx Deployment

### 3. Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the Nginx image from the Docker registry so it can be used to create a container.

### 4. Run the Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This command creates and starts the Nginx container. The `-p 8080:80` option connects port 8080 on the host to port 80 inside the container.

### 5. Test the Nginx Server

```bash
curl http://localhost:8080
```

This command sends a request to the Nginx server and checks if it is responding correctly.

## Checkpoint 5 - Container Lifecycle

### 6. View Running Containers

```bash
docker ps
```

This command displays the containers that are currently running.

### 7. Stop the Nginx Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container.

### 8. Check Running Containers

```bash
docker ps
```

This command verifies that the Nginx container is no longer running.

### 9. Remove the Nginx Container

```bash
docker rm nginx-server
```

This command removes the stopped Nginx container.

### 10. View All Containers

```bash
docker ps -a
```

This command displays all containers and can be used to verify that the Nginx container was removed.

