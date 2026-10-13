# Firewall Configuration

## Permit SSH Access

Command used:

```bash
sudo ufw allow ssh
```

This rule permits SSH connections for remote server administration. It should be configured before enabling UFW when the server is being managed through SSH.

## Set the Default Traffic Policies

Commands used:

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

The incoming policy rejects connections unless an allow rule exists. The outgoing policy permits outbound traffic by default, allowing the server to initiate necessary connections.

## Allow the Web Application Port

Command used:

```bash
sudo ufw allow 8080/tcp
```

This rule allows incoming TCP traffic through port 8080, which is mapped to the Nginx container's web service in this laboratory setup.

## Activate and Inspect UFW

Commands used:

```bash
sudo ufw enable
sudo ufw status verbose
sudo ufw status numbered
```

These commands enable the firewall and display its current policy and numbered rules. Reviewing the output helps verify that the configuration matches the intended settings.
