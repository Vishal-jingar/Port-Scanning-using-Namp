# 🔍 Local Network Port Scanning Guide

## 📘 Objective
Learn how to discover open ports on devices within your local network to understand service exposure and identify potential security risks.

---

## 🛠️ Tools Required
- [Nmap](https://nmap.org/download.html) (Free port scanner)
- [Wireshark](https://www.wireshark.org/) *(optional)* – for network traffic analysis

---

## 🧭 Step-by-Step Instructions

1. **Install Nmap**  
   Download and install from [https://nmap.org/download.html](https://nmap.org/download.html).

2. **Identify Your Local IP Range**  
   - Windows: `ipconfig`  
   - macOS/Linux: `ifconfig` or `ip a`  
   - Example subnet: `192.168.1.4/24`

3. **Perform a TCP SYN Scan**
   ```bash
   nmap -sS 192.168.1.4/24
nmap -sS 192.168.1.4/24 -oN scan_results.txt

