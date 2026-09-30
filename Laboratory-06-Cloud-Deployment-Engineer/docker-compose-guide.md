# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block identifies the different services that Docker Compose needs to run for the application. In the YAML file, the `database` service runs MariaDB, while the `app` service runs Nextcloud.

## How Does the Nextcloud App Find the Database?

The Nextcloud application uses the `MYSQL_HOST` environment variable to determine the location of its database. The value is set to `database`, which is the service name assigned to the MariaDB container. Docker Compose allows the services to communicate using their service names.

## What is the Difference Between `docker run` and `docker-compose up -d`?

The `docker run` command is used to create and start a Docker container by providing its configuration through the command line. On the other hand, `docker-compose up -d` reads the settings from the `docker-compose.yml` file and starts the services defined in it. The `-d` option runs the services in the background.
