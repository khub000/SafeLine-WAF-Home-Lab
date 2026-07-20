# 🛡️ SafeLine WAF Home Lab

> A hands-on Web Application Firewall (WAF) lab built using SafeLine WAF to protect a vulnerable web application (DVWA) from common web attacks.

![SafeLine WAF](https://img.shields.io/badge/SafeLine-WAF-blue)
![DVWA](https://img.shields.io/badge/DVWA-Vulnerable%20App-red)
![Ubuntu](https://img.shields.io/badge/Ubuntu-Server-E95420)
![Kali](https://img.shields.io/badge/Kali-Linux-557C94)

---

# 📌 Overview

This project demonstrates the deployment and configuration of **SafeLine Web Application Firewall (WAF)** in a home lab environment. A vulnerable web application (DVWA) was hosted on an Ubuntu server and protected using SafeLine WAF configured as a reverse proxy.

The lab includes attack simulation, WAF rule validation, and traffic inspection to understand how a WAF detects and blocks malicious web requests.

---

# 🎯 Objectives

- Deploy SafeLine WAF
- Configure DVWA behind a reverse proxy
- Simulate SQL Injection attacks
- Validate WAF detection and blocking
- Configure HTTP Flood protection
- Implement IP-based access control
- Explore authentication and HTTPS protection

---

# 🏗️ Lab Architecture

```
                +----------------+
                | Kali Linux VM  |
                |   (Attacker)   |
                +--------+-------+
                         |
               SQL Injection Requests
                         |
                         ▼
                +------------------+
                |  SafeLine WAF    |
                | Reverse Proxy    |
                +--------+---------+
                         |
                         ▼
                +------------------+
                | Ubuntu Server    |
                | Apache + DVWA    |
                +------------------+
```

---

# 🛠️ Technologies Used

- SafeLine WAF
- DVWA (Damn Vulnerable Web Application)
- Ubuntu Server
- Kali Linux
- Apache2
- MariaDB / MySQL
- VirtualBox
- OpenSSL

---

# 🔒 Security Features Implemented

- Reverse Proxy Configuration
- SQL Injection Protection
- HTTPS using Self-Signed Certificate
- HTTP Flood Defense
- Custom IP Blocking Rules
- Authentication Protection
- Web Traffic Inspection

---

# 🧪 Attack Simulation

The following attack scenarios were tested:

- SQL Injection
- HTTP Flood Requests
- Unauthorized Access Attempts
- IP-based Access Blocking

---

# 📈 Skills Demonstrated

- Web Application Security
- Web Application Firewall (WAF)
- Reverse Proxy Configuration
- SQL Injection Detection
- HTTPS Configuration
- Apache Administration
- Ubuntu Server Administration
- Security Monitoring
- Attack Simulation
- Blue Team Fundamentals

---

# 📁 Repository Structure

```
SafeLine-WAF-Home-Lab/
│
├── README.md
├── REPORT.pdf
├── screenshots/
│   ├── lab-architecture.png
│   ├── safeline-dashboard.png
│   ├── sql-injection-block.png
│   ├── http-flood-defense.png
│   ├── ip-block-rule.png
│   └── https-configuration.png
│
├── configuration/
│   ├── apache.conf
│   ├── ssl-setup.md
│   └── safeline-notes.md
│
├── LICENSE
└── .gitignore
```

---

# 📚 Learning Outcomes

- Deploying and configuring SafeLine WAF
- Protecting web applications with a reverse proxy
- Detecting and blocking SQL Injection attacks
- Configuring HTTPS with SSL certificates
- Implementing custom security policies
- Understanding WAF logging and traffic inspection

---

# 👨‍💻 Author

**Khubaib PP**

Aspiring SOC Analyst | Cybersecurity Enthusiast

- GitHub: https://github.com/khub000
- LinkedIn: https://linkedin.com/in/khubaibpp
- Portfolio: https://www.khubaibpp.online

---

