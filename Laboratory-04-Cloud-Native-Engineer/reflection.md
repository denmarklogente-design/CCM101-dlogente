# Mission Reflection

## Reflection

This laboratory activity helped me understand the basic idea of containerization and how Docker is used to run applications. Before doing the activity, I knew that Virtual Machines and containers were both used for applications, but I did not fully understand their differences. I learned that a VM needs a complete operating system, while a container shares the host operating system. Because of this, containers are usually lighter and can be started faster.

Setting up the Nginx container was also easier compared with setting up a complete Virtual Machine. With a VM, I would need to prepare and configure an operating system before running the web server. With Docker, I only needed to pull the Nginx image and use the `docker run` command. This showed me how containers can simplify the deployment process and reduce the resources needed to run an application.

I also learned the purpose of the `-p 8080:80` option. It connects port 8080 on the host machine to port 80 inside the Nginx container. This allowed me to access the web server using `http://localhost:8080`. When I used the `curl` command, I received a response from Nginx, which confirmed that the container was working correctly.

The container lifecycle activity also showed me what happens when a container is stopped and removed. Using `docker stop` stops the container, while `docker rm` removes it. Data stored only inside the container does not automatically become permanent after the container is removed, so persistent storage should be used when important data needs to be saved.

Containerization can improve communication between developers and IT operations because both teams can work with the same application environment. Developers can prepare the application in a container, and the operations team can deploy the same container with less manual configuration. This supports DevOps by making the deployment process more consistent.

This laboratory also helped improve my GitHub portfolio. I added my research, Docker commands, screenshots, documentation, and reflection. It gave me practical experience with a cloud-native technology that I can continue learning and using in future IT activities.

