# 🧪 Cybersecurity Home Lab Setup

This project documents the setup of a virtual cybersecurity lab using VirtualBox, Ubuntu Server, SSH, and a host-only internal network. This lab environment will be used for penetration testing, vulnerability scanning, and defensive tool configuration in future projects.

---

## 🔧 Tools Used
- Oracle VirtualBox
- Ubuntu 22.04 LTS
- Host-Only Network Adapter
- OpenSSH Server

---

## 🛠 Lab Setup Summary

1. **Created VirtualBox Host-Only Network**
   - IPv4 Address: `192.168.56.1/24`
   - DHCP Server: Enabled

2. **Ubuntu VM Configuration**
   - Attached to Host-Only Adapter
   - Received IP: `192.168.56.101`
   - Enabled SSH server:
     ```bash
     sudo apt update && sudo apt install openssh-server -y
     sudo systemctl enable ssh
     sudo systemctl start ssh
     ```

---

## 🧾 Screenshots

| Screenshot | Description |
|------------|-------------|
| ![IP Config](./Screenshot%202025-06-11%20234606.png) | Ubuntu VM showing IP address `192.168.56.101` |
| ![SSH Status](./Screenshot%202025-06-11%20234812.png) | SSH service running and active |
| ![VirtualBox Network](./Screenshot%202025-06-11%20234617.png) | Host-only adapter setup in VirtualBox |
| ![VM Network Attached](./Screenshot%202025-06-11%20234714.png) | VM network settings attached to Host-Only |

---

## ✅ Outcome

- Successfully isolated Ubuntu server in a virtual testbed
- Verified SSH connectivity and static IP setup
- Ready for vulnerability scanning in Week 2

---

## 📅 Next Steps
- Add Kali Linux and Metasploitable2
- Perform Nmap vulnerability scans
- Document findings in a penetration test-style report
