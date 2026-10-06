# Mission Reflection

Before doing this activity, I mainly thought that checking whether a container was running was enough to know that an application was working. After completing the activity, I understood that the host server also needs to be monitored because the containers depend on the server's available resources. If the CPU, memory, or disk space becomes insufficient, the application can be affected even when the container itself is still running. This made me realize why checking the server's condition is an important part of cloud operations.

I also found the `docker logs` command useful because it gives information about what is happening inside the container. If a user says that they cannot log into a web application, I would check the logs for error messages or failed requests that could give a clue about the problem. This is more useful than simply guessing because the logs provide actual records of what happened.

The activity also made the difference between logs and metrics clearer to me. Logs focus on events, such as HTTP requests and errors, while metrics focus on measurable resource usage. For example, CPU percentage and memory usage from `docker stats` show how much of the host's resources the container is using at a particular time.

For an enterprise company with thousands of containers, checking everything manually would be difficult. Monitoring tools such as Prometheus and Grafana can make this process more manageable. Prometheus can collect metrics from different systems, while Grafana can display the collected information in dashboards so engineers can monitor many containers more efficiently.

I also became more comfortable with Linux troubleshooting during this activity. Using `free`, `df`, `top`, `curl`, `docker logs`, and `docker stats` gave me practical experience with checking different parts of a system. I learned to look at the available information first before deciding what might be causing a problem.
