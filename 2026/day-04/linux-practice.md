# Day 04 - Linux Practice Lab

## Objective

Practice basic Linux administration by checking running processes, inspecting a systemd service, and performing a simple troubleshooting workflow.

---

## 1. Check Running Processes

<img width="957" height="823" alt="image" src="https://github.com/user-attachments/assets/148d9eb8-04af-4df2-a4c7-0e216a8c2453" />


### Observation

- Displayed currently running processes.
- Identified important processes such as `docker`, `sshd`, and my shell session.
- Noticed that each process has a unique PID (Process ID).

---

## 2. Inspect a Systemd Service

<img width="958" height="311" alt="image" src="https://github.com/user-attachments/assets/2aaf013c-7f85-4061-b8f7-46ff837d0ed9" />


### Observation

- Verified that the SSH service was active and running.
- Checked the service status, uptime, and PID.
- Confirmed that systemd is managing the service.

<img width="958" height="300" alt="image" src="https://github.com/user-attachments/assets/53a838c5-44bf-42b1-8a4d-06307d550a7c" />

### Observation

- Docker Daemon started successfully
- Existing containers were loaded
- Network rules were initialized
- systemd marked the service as active

---

## 3. Basic Troubleshooting Flow

### a. Unable to curl localhost

<img width="939" height="34" alt="image" src="https://github.com/user-attachments/assets/9648fc11-7e30-4b59-ab9a-246ba21237ae" />

### Observation:

- Failed to connect localhost at port 80

### b. checking nginx logs

<img width="956" height="92" alt="image" src="https://github.com/user-attachments/assets/11924ad9-1ee8-46ea-8e85-8e62a899419f" />

### Observation:

- Logs shows nginx is deactivated and nginx.service is stopped

### c. Checking nginx status

<img width="959" height="246" alt="image" src="https://github.com/user-attachments/assets/de99c865-0284-4e97-8571-eae188cae563" />

### Observation:

- show inactive nginx status

### d. Is the port listening ?

<img width="953" height="171" alt="image" src="https://github.com/user-attachments/assets/99ad94d0-91e3-43c9-9428-c2ac35d61112" />

### Observation: 

- port is not listening to port 80

### e. Enabling nginx status and curl localhost

<img width="959" height="748" alt="image" src="https://github.com/user-attachments/assets/e6f85cea-8bc8-4b90-87b5-14b60a9fe712" />

### Observation: 

- Shows nginx status as active. nginx service is up in running and was successfuly able to curl localhost

---
