# 🛡️ Kali Linux Virtual Cybersecurity Lab

### Virtual Lab Deployment and Network Configuration

## 📌 Project Overview

This project focuses on building a virtual cybersecurity laboratory using **Kali Linux** and **Oracle VirtualBox**. The environment provides a dedicated Linux workspace for learning cybersecurity concepts, exploring security utilities, and performing authorized security assessments.

The implementation includes virtual machine deployment, resource allocation, network configuration, and basic Linux terminal operations.

---

## 🎯 Project Objectives

- Deploy Kali Linux using Oracle VirtualBox.
- Configure virtual machine hardware resources.
- Establish a NAT Network connection.
- Understand DHCP-based IP address allocation.
- Explore Linux terminal commands.
- Verify network connectivity and DNS resolution.
- Document the laboratory configuration with screenshots.

---

## 🖥️ System Specifications

### Virtual Machine Configuration

| Component | Configuration |
|---|---|
| Virtualization Platform | Oracle VirtualBox |
| Guest Operating System | Kali Linux |
| VM Name | Kali |
| RAM | 4096 MB |
| CPU | 2 Processors |
| Video Memory | 128 MB |
| Graphics Controller | VMSVGA |
| Virtual Storage | Kali.vdi |
| Disk Capacity | 40 GB |
| Network Adapter | Intel PRO/1000 MT Desktop |
| Network Mode | NAT Network |
| NAT Network Name | NatNetwork |
| Desktop Environment | XFCE |

---

## ⚙️ Virtual Machine Setup

The Kali Linux virtual machine was configured with dedicated memory, processing resources, virtual storage, and display settings to support cybersecurity laboratory activities.

### Hardware Allocation

- **Memory:** 4 GB
- **Processors:** 2
- **Storage:** 40 GB virtual disk
- **Display Controller:** VMSVGA
- **Video Memory:** 128 MB

### Virtual Machine Overview

![Kali Virtual Machine](screenshots/01-virtual-machine.png)

---

## 🌐 Virtual Network Configuration

A NAT Network named **NatNetwork** was configured in Oracle VirtualBox to provide networking capabilities for virtual machines connected to the same network.

### NAT Network Parameters

| Parameter | Value |
|---|---|
| Network Name | NatNetwork |
| IPv4 Prefix | 10.0.2.0/24 |
| DHCP Server | Enabled |
| IPv6 | Disabled |

### NAT Network Configuration

![NAT Network Configuration](screenshots/02-nat-network.png)

### Network Adapter Configuration

The Kali Linux virtual machine was connected to the configured NAT Network through its virtual network adapter.

| Parameter | Value |
|---|---|
| Adapter | Adapter 1 |
| Adapter Type | Intel PRO/1000 MT Desktop |
| Attached To | NAT Network |
| Network Name | NatNetwork |
| Cable Connected | Enabled |

![Kali NAT Network Adapter](screenshots/04-nat-network-adapter.png)

### Networking Concepts

**NAT:** Provides outbound network access through the host system using network address translation.

**NAT Network:** Enables communication between virtual machines connected to the same NAT Network while supporting outbound connectivity.

**DHCP:** Automatically assigns network configuration parameters to connected virtual machines.

---

## 🐧 Kali Linux Environment

Kali Linux is a Debian-based distribution designed for penetration testing, security research, digital forensics, and cybersecurity education.

The configured environment uses the XFCE desktop interface and Linux terminal for performing administrative and security-related tasks.

### Terminal Environment

![Kali Linux Terminal](screenshots/03-kali-terminal.png)

### Basic Linux Commands

| Command | Description |
|---|---|
| `pwd` | Displays the current directory |
| `ls` | Lists files and directories |
| `mkdir` | Creates a directory |
| `touch` | Creates an empty file |
| `cat` | Displays file contents |
| `nano` | Opens a text editor |
| `ip a` | Displays network interfaces |
| `ip route` | Displays routing information |
| `ping` | Tests network reachability |

---

## 🧪 Network Verification

The following commands can be used to evaluate the connectivity of the configured Kali Linux environment.

### 1. Inspect Network Interfaces

```bash
ip a
```

Displays network interfaces and their assigned IP addresses.

### 2. Inspect the Routing Table

```bash
ip route
```

Displays available routes and the default gateway.

### 3. Test External Connectivity

```bash
ping -c 4 8.8.8.8
```

Checks connectivity to an external IP address.

### 4. Test DNS Resolution

```bash
nslookup google.com
```

Checks whether DNS resolution is working correctly.

### 5. Verify Nmap Installation

```bash
nmap --version
```

Displays the installed Nmap version.

*Network verification results should be recorded after executing these commands.*

---

## 📚 Learning Outcomes

The laboratory setup provides practical understanding of:

- Virtual machine deployment and configuration
- Virtual hardware resource allocation
- NAT and NAT Network functionality
- DHCP-based network configuration
- IPv4 networking fundamentals
- Linux terminal operations
- Basic network troubleshooting
- Cybersecurity laboratory preparation
- Technical documentation

---

## 🔐 Ethical Considerations

This environment is intended for educational activities and authorized security testing.

Any scanning, enumeration, or penetration testing activities must be performed only against systems for which explicit permission has been obtained.

---

## 🛠️ Technologies Used

- Oracle VirtualBox
- Kali Linux
- XFCE Desktop Environment
- Linux Terminal
- NAT Network
- DHCP
- IPv4
- Nmap

---

## 📸 Project Documentation

The `screenshots/` directory contains visual records of the virtual machine deployment, network configuration, and Linux terminal environment.

---

## 👩‍💻 Project Details

**Project Name:** Kali Linux Virtual Cybersecurity Lab  
**Domain:** Cybersecurity  
**Platform:** Oracle VirtualBox  
**Operating System:** Kali Linux  
**Project Type:** Practical Laboratory Setup

---

*Developing cybersecurity skills through practical experimentation and virtual laboratory environments.*

