# 🛡️ CyberOps Academy — Day 2 Mission

## Networking Basics & Protocols · OSI Model · TCP/IP · Ports & DNS

![Bootcamp](https://img.shields.io/badge/Bootcamp-CyberOps%20Academy-blue?style=for-the-badge&logo=shield&logoColor=white)
![Day](https://img.shields.io/badge/Day-02%20of%2030-brightgreen?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![Domain](https://img.shields.io/badge/Domain-Cybersecurity-red?style=for-the-badge)

> **"The network is the battlefield — you need to know the terrain."** — CyberOps Academy

---

## 📋 Mission Overview

| Field | Details |
|---|---|
| 🗓️ **Date** | April 10, 2026 |
| 📚 **Bootcamp** | CyberOps Academy — 30-Day Analyst Bootcamp (Offline Edition) |
| 🎯 **Day** | Day 2 of 30 |
| 🔖 **Topic** | Networking Basics & Protocols |
| 👤 **Analyst** | Ganesh (0407ganesh) |
| ⚡ **XP Earned** | 100 XP |

---

## 🌐 Why Networking Matters to Security

Almost every cyber attack travels over a network. If you don't understand how data moves, you can't detect when something is wrong. Networks are the battlefield — every analyst must know the terrain.

---

## 📊 The OSI Model — 7 Layers

The OSI (Open Systems Interconnection) model is the foundation of network communication. Every packet, every attack, every defense operates within these layers.

| Layer | Name | What It Does | Security Relevance |
|---|---|---|---|
| L7 | Application | HTTP, FTP, SMTP, DNS | Malware C2, phishing, injection attacks |
| L6 | Presentation | Encryption, encoding (SSL/TLS) | SSL stripping, encoding attacks |
| L5 | Session | Manages sessions between apps | Session hijacking |
| L4 | Transport | TCP/UDP — ports, reliability | Port scanning, SYN floods |
| L3 | Network | IP addressing, routing | IP spoofing, routing attacks |
| L2 | Data Link | MAC addresses, switches, ARP | ARP poisoning, MAC spoofing |
| L1 | Physical | Cables, signals, bits | Physical tampering, eavesdropping |

> 💡 **Analogy:** The OSI model is like sending a letter. You write it (Application), seal the envelope (Presentation), address it (Network), and the postal system routes it physically (Physical). Each layer adds/removes its own "envelope."

---

## 🔌 Critical Ports Every Analyst Must Know

| Port | Protocol | Description | Attacker Interest |
|---|---|---|---|
| 22 | SSH | Secure remote login | Brute force attacks |
| 80 | HTTP | Unencrypted web traffic | Man-in-the-middle |
| 443 | HTTPS | Encrypted web traffic | SSL inspection |
| 21 | FTP | File transfer (unencrypted) | Credential sniffing |
| 53 | DNS | Domain name resolution | DNS tunneling, poisoning |
| 3389 | RDP | Windows Remote Desktop | Ransomware delivery |
| 445 | SMB | Windows file sharing | EternalBlue / WannaCry |

---

## 🤝 TCP 3-Way Handshake

```
# TCP 3-Way Handshake (how connections start)
Client → Server:  SYN       # "Hello, can we talk?"
Server → Client:  SYN-ACK   # "Yes! Ready."
Client → Server:  ACK       # "Great, let's go!"

# SYN Flood attack = sending thousands of SYNs without ACK
# This exhausts server resources — a classic DoS attack
```

---

## 🔎 DNS — The Internet's Phone Book

DNS translates domain names (google.com) to IP addresses (142.250.80.46).

**How Attackers Abuse DNS:**

| Attack Type | Description |
|---|---|
| **DNS Poisoning** | Injecting fake DNS records to redirect users to malicious sites |
| **DNS Tunneling** | Hiding data or C2 traffic inside DNS queries to bypass firewalls |
| **Typosquatting** | Registering similar-looking domains (g00gle.com) to trick users |
| **DNS Amplification** | Using open DNS resolvers for DDoS amplification |

---

## 🔍 Protocol Security Analysis

### TCP vs UDP — Analyst Perspective

| Feature | TCP | UDP |
|---|---|---|
| Connection | Connection-oriented (3-way handshake) | Connectionless |
| Reliability | Reliable, ordered delivery | Fast, no guarantee |
| Use Cases | HTTP, SSH, FTP, SMTP | DNS, VoIP, streaming |
| Attack Surface | SYN floods, session hijacking | UDP floods, amplification |

### HTTP vs HTTPS — Security Implication

- **HTTP (Port 80):** Traffic is plaintext — any attacker on the network can read credentials, session cookies, and sensitive data
- **HTTPS (Port 443):** Traffic is encrypted with TLS — protects confidentiality and integrity in transit
- **Analyst Note:** Malware increasingly uses HTTPS to hide C2 communication — HTTPS is not automatically "safe"

---

## 🧠 Key Takeaways

- The **OSI Model** maps every network attack to a specific layer — essential for threat analysis
- **Port numbers** are attack entry points — knowing common ports helps identify suspicious traffic
- The **TCP 3-Way Handshake** is fundamental to understanding connection-based attacks like SYN floods
- **DNS** is heavily abused by attackers for tunneling, poisoning, and C2 communication
- **HTTPS ≠ Safe** — encrypted malware traffic is a real threat that SOC analysts must handle

---

## 🗂️ Repository Structure

```
cyberops-day2-networking-protocols/
│
├── README.md     ← Mission write-up (this file)
└── index.html    ← Attractive HTML portfolio page
```

---

## 🚀 About This Bootcamp

The **CyberOps Academy 30-Day Analyst Bootcamp** is an offline, self-paced cybersecurity program designed to build real analyst skills from the ground up — covering fundamentals, tools, threat analysis, and hands-on labs across 30 structured days.

**📌 Part of the CyberOps Academy 30-Day Bootcamp Portfolio**

[GitHub](https://github.com/0407ganesh)

Aspiring Cybersecurity Analyst · BCA 3rd Year · Bengaluru, Karnataka
