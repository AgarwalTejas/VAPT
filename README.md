# Vulnerability Assessment and Penetration Testing (VAPT)

## 📌 Project Overview
This project demonstrates a complete Vulnerability Assessment and Penetration Testing (VAPT) process performed in a controlled lab environment using Kali Linux and intentionally vulnerable virtual machines.

The objective was to identify security weaknesses, analyze vulnerabilities, and perform controlled exploitation for educational purposes.

---

## 🎯 Objectives
- Perform reconnaissance and information gathering
- Identify open ports and running services
- Detect vulnerabilities using scanning tools
- Exploit identified vulnerabilities in a safe lab environment
- Document findings and security risks

---

## 🛠 Tools Used
- Kali Linux
- Nmap
- Metasploit Framework
- Burp Suite
- Metasploitable 2 (Vulnerable VM)

---

## 🧪 Lab Setup
- Attacker Machine: Kali Linux
- Target Machine: Metasploitable 2
- Network Type: Host-only / Internal network
- Target IP: 192.168.56.101 (example)

---

## 🔎 Methodology

### 1️⃣ Reconnaissance & Scanning

Basic Scan: 
Service Version Detection:

Findings:
- Multiple open ports detected
- FTP, SSH, HTTP, SMB services running

---

### 2️⃣ Vulnerability Assessment

Vulnerability Scan:

Identified Issues:
- Outdated FTP service (vsftpd 2.3.4)
- SMB vulnerabilities
- Exposed services

---

### 3️⃣ Exploitation Using Metasploit

Steps:
- Launched msfconsole
- Searched for vsftpd exploit
- Configured RHOST
- Executed exploit

Result:
- Successful shell access obtained (controlled lab environment)

---

### 4️⃣ Web Application Testing (Burp Suite)

- Intercepted HTTP requests
- Tested input fields for:
  - SQL Injection
  - Cross-Site Scripting (XSS)
- Analyzed server responses

---

## 📊 Key Findings

| Vulnerability | Severity | Exploited | Status |
|--------------|----------|-----------|--------|
| vsftpd Backdoor | High | Yes | Successful |
| Open Ports Exposure | Medium | No | Identified |
| Weak Service Versions | Medium | No | Observed |

---

## 🛡 Risk Analysis
The identified vulnerabilities could allow:
- Unauthorized remote access
- Data exposure
- Service compromise
- Privilege escalation

---

## ✅ Conclusion
The VAPT process successfully identified and exploited vulnerabilities in a controlled lab environment. This demonstrates the importance of:

- Regular patching
- Disabling unnecessary services
- Network monitoring
- Secure configurations

---

## ⚠ Ethical Disclaimer
This testing was performed in a controlled lab environment using intentionally vulnerable machines for educational purposes only. No real-world systems were targeted.

---

## 👨‍💻 Author
Tejas Agarwal 
Cybersecurity Intern
