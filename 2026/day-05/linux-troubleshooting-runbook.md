# Linux Practice Lab: Service Health Check & Troubleshooting (Nginx)

## Objective

Perform a health check on a running Linux service (**Nginx**) by:

* Capturing a quick system health snapshot
* Inspecting the service status
* Tracing service logs
* Writing a simple troubleshooting runbook

---

# Step 1: Verify the Service Status

Check whether Nginx is running.

<img width="471" height="164" alt="image" src="https://github.com/user-attachments/assets/739a30bd-9ee9-488b-81fd-b2af0e9bbcf7" />


### Observation

Verify:

* Service is **active (running)**
* Main PID is displayed
* No recent failures or warnings


---

# Step 2: Capture a Quick Health Snapshot

## CPU

Check system load:

<img width="470" height="25" alt="image" src="https://github.com/user-attachments/assets/fcfa5f31-434f-4dfb-a712-2333abd09cb1" />




Monitor CPU utilization:

<img width="476" height="389" alt="image" src="https://github.com/user-attachments/assets/d35621c9-4a29-4d11-9870-8805b4af1d4d" />


### Observation

* CPU utilization is normal.
* System load is low.
* Nginx process is consuming minimal CPU.

---

## Memory

Check memory usage:

<img width="347" height="37" alt="image" src="https://github.com/user-attachments/assets/ac8468e6-3276-4da2-b241-d35a4c44e9fa" />


### Observation

* Available memory is sufficient.
* Swap is not being utilized.

---

## Disk

Check filesystem usage:

<img width="356" height="104" alt="image" src="https://github.com/user-attachments/assets/f65a20d6-3dcc-4a26-857a-735e298b2477" />



### Observation

* Root filesystem has adequate free space.
* No filesystem is critically full.

---

## Network

Verify Nginx is listening on port **80**.

<img width="472" height="44" alt="image" src="https://github.com/user-attachments/assets/6631e30b-d45c-428f-8b7b-2b4c1f040793" />



Test the web server locally:

<img width="437" height="175" alt="image" src="https://github.com/user-attachments/assets/2e623e96-8a97-4d4f-8897-18f406e2c0a5" />

### Observation

* Nginx is accepting HTTP connections.
* Local web page loads successfully.

---

# Step 3: Trace Service Logs

View service logs:

<img width="471" height="142" alt="image" src="https://github.com/user-attachments/assets/0229782d-53e0-49da-8a95-c925ccdc7d09" />


View the last 10 log entries:

<img width="473" height="78" alt="image" src="https://github.com/user-attachments/assets/0517030c-9166-440e-bdf4-96dd6ae64538" />


Monitor logs in real time:

<img width="479" height="124" alt="image" src="https://github.com/user-attachments/assets/9628d37e-0237-49c0-8a9b-f99afaef6f46" />


### Observation

Verify:

* Successful service startup
* Configuration reloads
* Client connections
* No critical errors

---

# Mini Runbook

## Incident

A user reports that the company website is unavailable.

---

## Actions Performed

### 1. Verified the service status

<img width="470" height="139" alt="image" src="https://github.com/user-attachments/assets/767df9dd-e723-46ee-ba5a-79c6b1177ada" />


Confirmed the service was not running.

---


### 2. Reviewed service logs

<img width="463" height="43" alt="image" src="https://github.com/user-attachments/assets/c0ee5909-63a9-4eef-a647-a13719f88ab1" />

Reviewed logs for startup failures, permission errors, or configuration issues.

---

### 3. Start the process

<img width="470" height="147" alt="image" src="https://github.com/user-attachments/assets/60dc8be3-95e1-4504-88b8-b481a5724463" />


Confirmed that the Nginx process was active.

---

### 4. Verified listening port

<img width="472" height="43" alt="image" src="https://github.com/user-attachments/assets/c5080138-a323-4c6b-b67e-d1416519d4ab" />


Confirmed that Nginx was listening on TCP port 80.

---

### 5. Tested the application locally

<img width="418" height="173" alt="image" src="https://github.com/user-attachments/assets/6b56cccb-c3d3-49ef-a401-64aa85d2cd02" />

Verified that the default Nginx web page was returned successfully.

---


