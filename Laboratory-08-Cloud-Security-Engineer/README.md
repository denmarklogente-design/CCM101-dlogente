
## Mission Overview

This laboratory activity demonstrates how to improve server security by controlling network access with UFW. The task includes launching an Nginx container, checking its availability, and applying firewall rules to permit only the required connections.

## Objectives

- Apply the Principle of Least Privilege.
- Review the network exposure of a running application.
- Configure default firewall policies.
- Permit SSH and TCP port 8080 when required.
- Check and record the active firewall rules.

## Commands Executed

```bash
docker --version
docker run -d --name secure-web-app -p 8080:80 nginx
docker ps
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
curl -I --max-time 5 http://localhost:8080
```

## Skills Learned

This laboratory provided experience in starting a Docker-based web server, testing HTTP responses, and managing network access with UFW. It also demonstrated how default firewall policies and specific allow rules help limit unnecessary connections to a server.

## Evidence

Screenshots are included to document the running application, firewall activation, and the rule that permits access through the required application port.
