# SafeLine WAF Configuration Notes

## Environment

- Hypervisor: VirtualBox
- Attacker: Kali Linux
- Target: Ubuntu Server
- Web Server: Apache2
- Application: DVWA
- Database: MariaDB
- WAF: SafeLine

---

## Reverse Proxy

Backend:

```
http://<Ubuntu-IP>:8080
```

Frontend:

```
https://dvwa.local
```

---

## Tested Security Features

- SQL Injection Protection
- HTTP Flood Defense
- Authentication Sign-In
- HTTPS Protection
- Custom IP Blocking

---

## SQL Injection Payload

```sql
' OR '1'='1
```

Result:

- SafeLine WAF detected the malicious request.
- Request was blocked before reaching DVWA.

---

## HTTP Flood Test

Multiple HTTP requests were generated from Kali Linux.

Result:

- SafeLine rate limiting was triggered.
- Excessive requests were blocked.

---

## Custom Deny Rule

Blocked IP:

```
<Kali-IP>
```

Action:

```
Deny
```

Result:

All requests from the attacker's IP were blocked.

---

## Learning Outcomes

- Reverse Proxy Configuration
- Web Application Firewall Deployment
- SQL Injection Detection
- HTTPS Configuration
- Web Traffic Inspection
- Security Policy Management
