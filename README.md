🧪 Network Analysis: Ping & DNS

📌 Objective
Analyze basic network connectivity and DNS resolution.

## 🔍 Steps

### 1. Ping Test
Command:
ping google.com

Purpose:
Check connectivity and latency.

### 2. DNS Lookup
Command:
nslookup google.com

Purpose:
Resolve domain name to IP addresses.

## 📊 Results

### Ping
- 0% packet loss
- Average latency ~0.3–0.4 ms
- Stable connection

### DNS
- DNS server: 1.1.1.1
- Multiple IP addresses returned
- IPv4 and IPv6 present

---

## 🧠 Conclusion
The network connection is stable and DNS resolution works correctly.  
Multiple IP addresses indicate load balancing.

---

## 📸 Screenshots

<img width="1276" height="871" alt="Screenshot_6" src="https://github.com/user-attachments/assets/e4e4f504-0eef-4def-8387-f5014928a481" />

---

# 🧪 Project 2: Traffic Analysis (Wireshark)

## 📌 Objective
Capture and analyze real network traffic.

---

## 🔍 Steps
- Started Wireshark on eth0
- Generated traffic via browser
- Applied filters: dns, http, tls

---

## 📊 Findings

### DNS
- Observed queries to:
  - google-analytics.com
  - consent.cookiebot.com
- Indicates background services (tracking, cookies)

---

### HTTP / OCSP
- Observed OCSP requests
- Used for certificate validation

---

### TLS
- Majority of traffic is encrypted
- TLSv1.3 Application Data packets detected

---

## 🧠 Conclusion
Network traffic consists of DNS resolution, certificate validation (OCSP), and encrypted HTTPS communication.  
No suspicious activity detected.

---

## 📸 Screenshots
<img width="1635" height="875" alt="image" src="https://github.com/user-attachments/assets/cd8241e1-00bb-461c-831d-3d6ef058e7b4" />
<img width="1631" height="874" alt="http" src="https://github.com/user-attachments/assets/b71e4c14-306b-4fec-a94e-007264d98c05" />
<img width="1632" height="867" alt="tls" src="https://github.com/user-attachments/assets/c8ebf1c9-3c4f-49cb-8571-51e9d7576195" />
