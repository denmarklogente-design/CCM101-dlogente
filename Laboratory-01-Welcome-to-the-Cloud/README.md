# Laboratory Activity 1: Mission 1 - Welcome to the Cloud

## Mission Overview
As a Junior Cloud Infrastructure Engineer Trainee at CloudNova Technologies, the onboarding mission focused on learning how to work inside a Linux environment, documenting technical work professionally, and maintaining a version-controlled portfolio using GitHub.

## Objectives
- Access a cloud-based Linux environment using KillerCoda.
- Explore and navigate the Linux operating system.
- Gather basic system information.
- Organize files and directories using Linux commands.
- Create and maintain a professional GitHub repository.
- Document technical work using Markdown.
- Demonstrate proper documentation practices used by cloud professionals[.

## Activities Performed
1. **Entered the Cloud**: Launched an Ubuntu Linux playground via KillerCoda, created a new user account with Bash and sudo privileges, logged into the account, and recorded user session details.
2. **Met the Environment**: Investigated the Linux distribution, kernel version, CPU info, total memory, and available disk space, recording findings in `system-information.md`.
3. **Built the Workspace**: Created standard directory structures (`Documents`, `Notes`, `Reports`, `Screenshots`) inside the home directory and drafted an introductory `about-me.md` file.
4. **Created Portfolio**: Built a public GitHub repository named `CCM101-dlogente` following the required folder hierarchy.
5. **Captured Evidence**: Organized and saved terminal session and environment screenshots inside the `screenshots` folder.

## Linux Commands Used
- `sudo useradd -m -s /bin/bash dlogente` - Created a new user account with a home directory and Bash shell.
- `sudo passwd dlogente` - Set the password for the new user account.
- `sudo usermod -aG sudo dlogente` - Granted sudo privileges to the new user.
- `su - dlogente` - Switched to the new user account session.
- `whoami`, `pwd`, `hostname` - Gathered current user, working directory, and hostname details.
- `cat /etc/os-release`, `uname -r`, `lscpu`, `free -h`, `df -h` - Investigated system distribution, kernel, CPU, memory, and disk utilization.
- `mkdir` - Created workspace directories.
- `nano` - Created and edited Markdown documentation files.

## Skills Learned
- Navigating and operating within a cloud-based Linux terminal environment.
- Managing user accounts and permissions securely.
- Extracting system diagnostics and hardware specs using command-line utilities[cite: 1].
- Structuring technical portfolios using Markdown and GitHub version control[cite: 1].
