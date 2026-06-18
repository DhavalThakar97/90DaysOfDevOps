# Day 03 - Linux Cheat Sheet

## Process Management

| Command | Description |
|----------|-------------|
| `ps` | Display running processes |
| `ps -ef` | View all running processes |
| `ps aux` | Detailed process information |
| `top` | Monitor processes in real time |
| `pstree` | View process hierarchy |
| `kill <PID>` | Gracefully terminate a process |
| `kill -9 <PID>` | Forcefully terminate a process |
| `pkill <name>` | Kill process by name |

### Examples

```bash
ps
ps -ef
ps aux
top
kill 1234
kill -9 1234
pkill nginx
pstree
```

---

## File System & Permissions

| Command | Description |
|----------|-------------|
| `pwd` | Show current directory |
| `ls -la` | List files and directories |
| `cd <dir>` | Change directory |
| `mkdir <dir>` | Create directory |
| `touch file.txt` | Create file |
| `cat file.txt` | View file contents |
| `cp source dest` | Copy files |
| `mv source dest` | Move or rename files |
| `rm -rf <dir>` | Remove files/directories |
| `find / -name file.txt` | Search for files |
| `chmod 755 file` | Change file permissions |
| `chown user:group file` | Change file ownership |
| `df -h` | Check disk usage |

### Examples

```bash
cat /etc/passwd
chmod 755 script.sh
chown user:user file.txt
find /home -name "*.log"
df -h
```

---

## System Memory

| Command | Description |
|----------|-------------|
| `free -h` | Display memory and swap usage |

### Example

```bash
free -h
```

---

## Network Troubleshooting

| Command | Description |
|----------|-------------|
| `ip a` | Show IP address information |
| `ping <host>` | Test network connectivity |
| `ss -tulpn` | View listening ports and services |
| `nslookup <domain>` | Perform DNS lookup |
| `curl <url>` | Test web connectivity |

### Examples

```bash
ip a
ping google.com
ss -tulpn
nslookup google.com
curl https://google.com
```

---

## Most Used Commands for DevOps

```bash
ps aux
top
kill
free -h
ls -la
cat
chmod
chown
find
df -h
ip a
ping
ss -tulpn
curl
```
