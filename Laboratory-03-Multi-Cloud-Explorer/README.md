# Linux Investigation Using KillerCoda

A Linux server environment was examined through the KillerCoda Playground to gather basic system information. The investigation covered the operating system, processor details, memory allocation, and available storage by using different Linux commands.

---

## 1. Operating System

The operating system was checked using the following command:

```bash
cat /etc/os-release
```

This command provides details about the Linux distribution currently running in the environment, including its name, version, and other release information.

### Terminal Evidence 1 – Operating System

[KillerCoda Terminal 1 - Operating System](screenshots/killercoda-terminal1.png)

---

## 2. CPU Information

The processor information was examined using:

```bash
lscpu
```

The command provides several details about the server's processor, such as the CPU architecture, processor count, and other hardware-related information.

### Terminal Evidence 2 – CPU Information

[KillerCoda Terminal 2 - CPU Information](screenshots/killercoda-terminal2.png)

---

## 3. Memory

The server's memory usage was examined with:

```bash
free -h
```

This command presents the memory statistics in an easier-to-read format. It shows the total memory together with the amount currently used, free, and available.

### Terminal Evidence 3 – Memory

[KillerCoda Terminal 3 - Memory](screenshots/killercoda-terminal3.png)

---

## 4. Disk Space

The available storage was checked using:

```bash
df -h
```

This command shows the storage capacity of the mounted file systems. It also provides information about used space, remaining space, and the percentage of storage currently being used.

### Terminal Evidence 4 – Disk Space

[KillerCoda Terminal 4 - Disk Space](screenshots/killercoda-terminal4.png)

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

If the Linux server were transferred to a cloud environment, it could be deployed through virtual machine services offered by major cloud providers.

| Cloud Provider              | Service That Could Host the Linux Server |
| --------------------------- | ---------------------------------------- |
| AWS                         | Amazon EC2                               |
| Microsoft Azure             | Azure Virtual Machines                   |
| Google Cloud Platform (GCP) | Compute Engine                           |

These services provide virtual machines where Linux operating systems can be installed and used for different workloads. The server could therefore be moved from the current environment to a cloud platform while continuing to use Linux as its operating system.

