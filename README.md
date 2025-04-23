# 🛡️ Penetration Testing Tools (Basics)

Welcome to the **Penetration Testing Tools – Basics** repository!  
This repo is a beginner-friendly collection of essential tools used in the ethical hacking and penetration testing process.

> 🚨 **Disclaimer:** This repository is intended for **educational purposes only**. Always obtain proper authorization before performing any kind of penetration testing or security assessments.

---

## 📌 Table of Contents
- [🔍 Phases of Penetration Testing](#-phases-of-penetration-testing)
- [🧰 Tool List with Descriptions](#-tool-list-with-descriptions)
- [⚙️ Tool Usage Examples](#️-tool-usage-examples)
- [📄 License](https://github.com/preetika-cyber/preetika-cyber/blob/main/LICENSE)

---

## 🔍 Phases of Penetration Testing

| Phase                  | Description | Example |
|------------------------|-------------|---------|
| **Reconnaissance**      | Gather initial information about the target (e.g., IPs, domains). | Using **whois** to gather domain registration details. |
| **Scanning & Enumeration** | Discover live systems, open ports, and services; identify weaknesses. | Using **Nmap** to identify open ports and services. |
| **Exploitation**        | Use vulnerabilities to gain unauthorized access. | Using **Metasploit** to exploit a known vulnerability. |
| **Post-Exploitation**   | Gather further info or maintain access once inside. | Setting up a **reverse shell** using **Netcat**. |
| **Reporting**           | Document findings, vulnerabilities, and suggestions for mitigation. | Creating a **report** that details discovered vulnerabilities and how to patch them. |
| **Password Attacks**    | Brute-force or exploit weak passwords to gain access to systems or accounts. | Using **Hydra** to brute-force SSH login credentials. |

---

## 🧰 Tool List with Descriptions

| Tool              | Phase(s) Involved        | Description |
|-------------------|--------------------------|-------------|
| **Nmap**          | Reconnaissance, Scanning | Scans hosts for open ports and services. |
| **Nikto**         | Scanning                 | Finds web server vulnerabilities and misconfigs. |
| **Dirb / Gobuster** | Scanning               | Discovers hidden directories and files. |
| **Hydra**         | Exploitation             | Performs brute-force logins (e.g., SSH, FTP, HTTP). |
| **Burp Suite**    | Scanning, Exploitation   | Intercepts and modifies HTTP traffic; great for web app testing. |
| **SQLmap**        | Exploitation             | Detects and exploits SQL injection flaws. |
| **Metasploit**    | Exploitation             | Framework to find, develop, and launch exploits. |
| **Wireshark**     | Reconnaissance, Post-Exploitation | Network protocol analyzer used to capture and analyze traffic. |
| **John the Ripper** | Post-Exploitation      | Cracks password hashes using dictionaries. |
| **Netcat**        | Post-Exploitation        | Useful for reverse shells, port listening, and banner grabbing. |
| **Strings**       | Reconnaissance           | Pulls readable strings from binary files—useful in reversing. |

---

## ⚙️ Tool Usage Examples

Here are some simple usage examples to help you get started:

### 🔹 Nmap
```bash
nmap -sV -T4 target_ip
```
- Scans for services and versions on open ports

### 🔹 Dirb
```bash
dirb http://target.com
```
- Scans the target website for hidden directories and files using a wordlist

###  🔹 WPscan
```bash
wpscan --url http://target.com
```
- Scans a WordPress site for known vulnerabilities, plugins, and user enumeration

###  🔹 Hydra
```bash
hydra -l admin -P rockyou.txt ssh://target_ip
```
- Brute-forces SSH logins with the username admin

###  🔹 SQLmap
```bash
sqlmap -u "http://target_ip/vuln.php?id=1" --batch --dbs
```
- Automatically detects and exploits SQLi

###  🔹 Metasploit
```bash
msfconsole
```
- Launch Metasploit console

###  🔹 John the Ripper
```bash
john hash.txt --wordlist=/usr/share/wordlists/rockyou.txt
```
- Cracks password hashes using a wordlist

###  🔹 Wireshark
```bash
wireshark
```
- Captures and analyzes network traffic in real-time


