

````markdown
# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

Laboratory Activity 6 focuses on deploying a private cloud storage application through Docker Compose. The deployment uses Nextcloud as the web application and MariaDB as its database service.

## Objectives

- Understand two-tier application architecture.
- Learn the purpose of a `docker-compose.yml` file.
- Use the Linux `nano` editor.
- Deploy multiple containers using Docker Compose.
- Understand basic Infrastructure as Code.
- Document the deployment using Markdown.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
````

## Skills Learned

This activity helped me develop skills in Docker Compose, YAML configuration, Linux commands, container deployment, environment variables, container communication, and technical documentation.

````

## `multi-tier-architecture.md`

```markdown
# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A Two-Tier Architecture separates an application into two main parts that work together. These are the Web/Application Tier, which handles application activities, and the Database Tier, which manages stored information.

## The Web/Application Tier

The Web/Application Tier provides the part of the system that users access. It handles HTTP requests and delivers the application's interface. In this deployment, Nextcloud performs the role of the Web/Application Tier.

## The Database Tier

The Database Tier is responsible for storing and managing information used by the application. MariaDB is used in this deployment to provide the database service for Nextcloud.

## Why Separate Them?

The web application and database are placed in two separate containers because they have different responsibilities. This separation makes each component easier to manage, troubleshoot, and maintain. It also prevents both functions from depending on one container.
````

## `docker-compose-guide.md`

```markdown
# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block defines the application components that Docker Compose will create and run. The YAML file contains two services: `database` for MariaDB and `app` for Nextcloud.

## How Does Nextcloud Find the Database?

The Nextcloud container uses the `MYSQL_HOST` environment variable to identify the database service. Since the value is set to `database`, Nextcloud connects to the MariaDB service using its Docker Compose service name.

## Difference Between `docker run` and `docker-compose up -d`

`docker run` is normally used to start an individual container while its configuration is supplied through the command. `docker-compose up -d` uses the configuration written in `docker-compose.yml` and starts the services defined there. The `-d` option allows the containers to run in the background.
```

## `reflection.md`

```markdown
# Mission 6 Reflection

## Reflection

Working with the Docker Compose configuration helped me understand how several parts of an application can be described in one file. Instead of configuring the Nextcloud application and MariaDB container separately every time, their settings can be placed in the Compose file and used for deployment.

I learned that YAML formatting is important because the indentation determines how the configuration is organized. An incorrect indentation or the use of a Tab instead of the required spaces can cause Docker Compose to reject or misunderstand the configuration.

The environment variables also helped connect the two services. Values such as `MYSQL_DATABASE`, `MYSQL_USER`, and `MYSQL_PASSWORD` provide the information needed by MariaDB and Nextcloud. The `MYSQL_HOST=database` setting identifies the database service that Nextcloud needs to communicate with.

Seeing the Nextcloud setup page in the browser helped me understand the result of the deployment. The terminal commands were not just commands by themselves because they resulted in an application that could be accessed through a browser.

My understanding of Cloud Computing has expanded since Mission 1. I now have a better idea of how containers, databases, networking, configuration files, and automation can work together. This activity also showed me how Infrastructure as Code can make deployment more organized and repeatable.
```
