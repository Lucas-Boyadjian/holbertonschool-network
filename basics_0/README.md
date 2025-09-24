# Networking basics #0

## Description

This project introduces fundamental networking concepts and essential commands for working with network interfaces and protocols on Ubuntu. You will learn about the OSI model, types of networks, IP and MAC addresses, TCP/UDP, ports, and basic network troubleshooting tools.

---

## Learning Objectives

By the end of this project, you should be able to explain:

- What is the OSI Model, its layers, and organization
- What is a LAN and a WAN, and their typical usage and size
- What is the Internet
- What is an IP address, and the difference between public/private, IPv4/IPv6
- What is localhost and what is a subnet
- Why IPv6 was created
- What are TCP and UDP, and their main differences
- What is a port, and the common port numbers for SSH (22), HTTP (80), and HTTPS (443)
- What tool/protocol is often used to check if a device is connected to a network

---

## Requirements

- All scripts are written for Ubuntu 22.04
- All scripts must be executable
- All scripts must pass Shellcheck without any error
- The first line of all scripts: `#!/usr/bin/env bash`
- The second line: a comment explaining what the script does
- A `README.md` file is mandatory at the root of the project

---

## Tasks

### 0. OSI model

Answer questions about the OSI model and its organization.

**File:** `0-OSI_model`

---

### 1. Types of network

Answer questions about LAN, WAN, and Internet usage.

**File:** `1-types_of_network`

---

### 2. MAC and IP address

Answer questions about MAC addresses and IP addresses.

**File:** `2-MAC_and_IP_address`

---

### 3. UDP and TCP

Answer questions about the differences between TCP and UDP.

**File:** `3-UDP_and_TCP`

---

### 4. TCP and UDP ports

Write a Bash script that displays all listening TCP/UDP ports and UNIX domain sockets, including the PID and program name.

**File:** `4-TCP_and_UDP_ports`

---

### 5. Is the host on the network

Write a Bash script that pings an IP address passed as an argument.  
- If no argument is passed, display: `Usage: 5-is_the_host_on_the_network {IP_ADDRESS}`  
- Ping the IP 5 times.

**File:** `5-is_the_host_on_the_network`

---

## Useful Commands

- **netstat**: Display network connections, routing tables, interface statistics, masquerade connections, and multicast memberships.
- **ping**: Send ICMP ECHO_REQUEST to network hosts to test connectivity.

---

## Example Usage

```bash
# Display all listening ports with netstat
sudo netstat -tulnp

# Ping an IP address 5 times
ping -c 5 8.8.8.8
```

---

## Author

- Lucas Boyadjian

---
