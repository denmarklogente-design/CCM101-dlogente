# Container Observability

## 404 Error

```text id="p6y2nf"
172.17.0.1 - - [05/Oct/2026:01:49:54 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

Application logs are useful because they provide a record of requests and errors made while the application is running. They give the engineer information that can be used to locate and understand problems during troubleshooting.

## Docker Metrics

The `docker stats` command was used to observe the running `client-website` container.

**Memory Usage:** `2.742MiB`

**CPU Percentage:** `0.00%`
