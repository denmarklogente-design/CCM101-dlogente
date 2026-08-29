## Mission Overview
Congratulations,
Your onboarding has been successfully completed, and your Cloud Computing Portfolio has been approved by your supervisor. CloudNova Technologies has now assigned you to your first official project. Before deploying cloud services, every cloud engineer must understand the infrastructure that powers modern cloud computing. Your mission is to investigate the components of cloud infrastructure, identify how compute, storage, networking, and identity services work together, and document your findings as if you were preparing technical documentation for a client. Using the KillerCoda Playground, Linux tools, official cloud documentation, and your GitHub Cloud Computing Portfolio, you will complete a series of engineering tasks that simulate the planning phase of a cloud deployment. Remember: Great cloud engineers build systems—but exceptional cloud engineers document and justify every design decision.

## Mission Objectives
At the end of this laboratory activity, you should be able to: Explain the major components of cloud infrastructure.

- Investigate the hardware and software resources available in a Linux environment.
- Differentiate compute, storage, networking, and identity resources.
- Interpret the relationship between cloud infrastructure components.
- Create professional technical documentation using Markdown.
- Continue building a structured GitHub Cloud Computing Portfolio.

# Cloud Infrastructure Components

| Component            | What Was Found                                           |
| -------------------- | -------------------------------------------------------- |
| Compute Resources    | Intel Xeon E312xx processor, 1 CPU core, and 1.9 GiB RAM |
| Storage Resources    | 19G disk capacity with several mounted file systems      |
| Networking Resources | `172.30.1.2` and `172.17.0.1`                            |
| Operating System     | Ubuntu 24.04.4 LTS                                       |

# Tools Used

| Tool                   |
| ---------------------- |
| KillerCoda Playground  | 
| Linux Terminal         |
| GitHub                 |
| Markdown               |
| Web Browser            | 
| Draw.io (diagrams.net) | 

# Linux Commands Executed

| Command                      |
| ---------------------------- |
| `cat /etc/os-release`        |
| `uname -r`                   |
| `lscpu \| grep "Model name"` |
| `nproc`                      |
| `free -h`                    |
| `df -h`                      |
| `findmnt`                    | 
| `hostname`                   |
| `hostname -I`                | 

# Skills Learned
```
I learned how to examine a Linux server and obtain important information using basic terminal commands. I became more familiar with checking system hardware, memory, storage, networking, and operating system details.

I also learned how to organize the collected information according to different cloud infrastructure components. In addition, I practiced using Markdown and GitHub to create and maintain technical documentation.
```
# Challenges Encountered

## Challenges   
```
-  Understanding the output of Linux commands, I studied the information returned by each command and identified its purpose.
- Interpreting the `findmnt` results, I checked the mounted locations and file system types carefully. 
- Identifying the server's IP addresses, I used `hostname -I` to display the available network addresses.
- Categorizing the server information,I separated the results into compute, storage, networking, and operating system resources.
- Keeping the documentation organized ,I used Markdown headings, tables, and code formatting to arrange the information.
```
