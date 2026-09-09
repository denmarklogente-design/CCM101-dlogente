# Linux Investigation Using KillerCoda

The KillerCoda Playground was used to inspect a Linux environment and gather basic information about the server. The investigation focused on the operating system, CPU, memory, and storage by running several commands through the terminal.

---

## 1. Operating System

The installed Linux distribution was checked with:

```bash
cat /etc/os-release
```

This command was used to view the name, version, and other release details of the operating system running on the server.

### Terminal Evidence 1 – Operating System

![KillerCoda Terminal 1](screenshots/killercoda-terminal1.png)

---

## 2. CPU Information

The server's processor configuration was examined using:

```bash
lscpu
```

The command provides technical information about the processor, including its architecture, CPU count, cores, threads, and other hardware details.

### Terminal Evidence 2 – CPU Information

![KillerCoda Terminal 2](screenshots/killercoda-terminal2.png)

---

## 3. Memory

The system memory was checked through:

```bash
free -h
```

This command displays the memory resources in a readable format. It shows how much memory is installed and how much is currently being used or remains available.

### Terminal Evidence 3 – Memory

![KillerCoda Terminal 3](screenshots/killercoda-terminal3.png)

---

## 4. Disk Space

The storage condition of the server was examined using:

```bash
df -h
```

This command was used to view the size of the mounted storage, the amount already occupied, the remaining capacity, and the percentage of disk usage.

### Terminal Evidence 4 – Disk Space

![KillerCoda Terminal 4](screenshots/killercoda-terminal4.png)

---

## Linux System Information Summary

| System Information | Command Used          | Evidence            |
| ------------------ | --------------------- | ------------------- |
| Operating System   | `cat /etc/os-release` | Terminal Evidence 1 |
| CPU Information    | `lscpu`               | Terminal Evidence 2 |
| Memory             | `free -h`             | Terminal Evidence 3 |
| Disk Space         | `df -h`               | Terminal Evidence 4 |

---

## Cloud Migration

The Linux server could also be deployed in a cloud environment by using virtual machine services from major cloud providers. Each provider offers a service that can provide computing resources for running a Linux-based server.

| Cloud Provider              | Service That Could Host the Linux Server |
| --------------------------- | ---------------------------------------- |
| AWS                         | `Amazon EC2`                             |
| Microsoft Azure             | `Azure Virtual Machines`                 |
| Google Cloud Platform (GCP) | `Compute Engine`                         |
