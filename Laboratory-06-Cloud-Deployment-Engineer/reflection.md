# Mission 6 Reflection

## Reflection

Creating the Docker Compose configuration showed me how multiple parts of an application can be organized in one file. Instead of setting up the Nextcloud application and MariaDB container separately each time, their configurations can be defined together and deployed using Docker Compose. This makes the deployment process more organized and repeatable.

I learned that YAML indentation must be handled carefully. The spaces determine how the different settings are grouped within the configuration. If a Tab is used instead of spaces or the indentation is incorrect, Docker Compose may not properly understand the file and the deployment can fail.

Environment variables are also important because they provide configuration information to the containers. The database name, username, and password are provided through variables such as `MYSQL_DATABASE`, `MYSQL_USER`, and `MYSQL_PASSWORD`. The `MYSQL_HOST=database` setting tells Nextcloud which service it should use for its database connection.

Seeing the Nextcloud setup page through the browser made the deployment more understandable. It showed me that the commands entered in the terminal resulted in an actual application that could be accessed through a web browser.

Since Mission 1, my understanding of Cloud Computing has developed from learning basic cloud concepts to understanding how containers, databases, networking, and configuration files can work together. This activity also helped me see how Infrastructure as Code can make cloud deployment more organized and easier to repeat.
