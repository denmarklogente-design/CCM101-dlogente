# Mission Overview

The purpose of this laboratory activity was to perform basic cloud operations and observe the condition of a server and its Docker container. The activity included checking the host resources, running an Nginx web server, sending web requests, checking the generated logs, and observing the container's resource usage.

# Objectives

- Utilize native Linux command-line tools to monitor host CPU, Memory, and Disk capacity.
- Deploy a web container and track its real-time performance using Docker metrics.
- Generate web traffic and extract application access logs for analysis.
- Translate raw performance data into a readable technical report using Markdown.
- Continue expanding a professional GitHub Cloud Computing Portfolio.

# Monitoring Commands Executed

### Checking Memory

```bash id="4xj8pn"
free -h
```

### Checking Disk

```bash id="m3kq7d"
df -h /
```

### Checking Processes and CPU

```bash id="y5v1rc"
top
```

### Running the Nginx Container

```bash id="8c2wlf"
docker run -d -p 8080:80 --name client-website nginx
```

### Sending HTTP Requests

```bash id="z7p4ha"
curl http://localhost:8080
```

### Creating a 404 Request

```bash id="n6t9qx"
curl http://localhost:8080/hidden-admin-page
```

### Viewing Container Logs

```bash id="r2m5vk"
docker logs client-website
```

### Checking Container Metrics

```bash id="b8f3wd"
docker stats
```

# Skills Learned

- Checking Linux server resources
- Monitoring CPU, memory, and disk capacity
- Running a Docker-based web server
- Testing HTTP requests
- Reading application logs
- Checking container resource usage
- Recording technical results in Markdown
- Organizing cloud laboratory work in GitHub
