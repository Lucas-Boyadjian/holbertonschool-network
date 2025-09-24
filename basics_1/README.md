# Networking basics #1

## Description

This project introduces basic networking concepts and essential commands for working with network interfaces and connections on Ubuntu. You will learn about `localhost`, IP addresses, the `/etc/hosts` file, and how to use tools like `ifconfig`, `telnet`, `nc`, and `cut`.

---

## Learning Objectives

By the end of this project, you should be able to explain:

- What is `localhost` / `127.0.0.1`
- What is `0.0.0.0`
- What is `/etc/hosts`
- How to display your machine’s active network interfaces

---

## Requirements

- All scripts are written for Ubuntu 22.04
- All scripts must be executable
- All scripts must pass Shellcheck (version 0.7.0)
- The first line of all scripts: `#!/usr/bin/env bash`
- The second line: a comment explaining what the script does

---

## Tasks

### 0. Change your home IP

Write a Bash script that configures an Ubuntu server so that:
- `localhost` resolves to `127.0.0.2`
- `facebook.com` resolves to `8.8.8.8`

**File:** `0-change_your_home_IP`

---

### 1. Show attached IPs

Write a Bash script that displays all active IPv4 IPs on the machine, one per line.

**File:** `1-show_attached_IPs`

---

### 2. Port listening on localhost

Write a Bash script that listens on port 98 on localhost.  
You can test it using `telnet localhost 98` from another terminal.

**File:** `2-port_listening_on_localhost`

---

## Useful Commands

- **ifconfig**: Display or configure network interfaces.
- **telnet**: Connect to a remote host and port (useful for testing open ports).
- **nc (netcat)**: Read/write data across network connections, test ports, debug, etc.
- **cut**: Extract specific columns or fields from text.

---

## Example Usage

```bash
# Show all active IPv4 addresses
ifconfig | grep 'inet ' | cut -d' ' -f2

# Listen on port 98
nc -l 98
```

---

## Author

- Lucas Boyadjian

---
