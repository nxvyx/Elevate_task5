# 🛰️ Network Traffic Analysis — Task 5

**Internship:** Cyber Security Virtual Internship  
**Task:** Capture and Analyze Network Traffic using Wireshark  
**Tool Used:** Wireshark  
**File Analyzed:** `networkTraffic.pcapng`

---

## 🎯 Objective
To capture live network packets and identify various protocols and communication patterns using Wireshark, focusing on both traditional and modern web traffic (UDP, TCP, QUIC, TLS, etc.).

---

## ⚙️ Steps Followed
1. Installed and opened **Wireshark**.  
2. Selected the **Wi-Fi interface** for live packet capture.  
3. Generated real-time traffic by:
   - Visiting websites like `google.com` and `youtube.com`.
   - Using the `ping` command to generate ICMP packets.
4. Stopped the capture after 1–2 minutes.  
5. Saved the capture as `networkTraffic.pcapng`.  
6. Applied filters such as:
```

dns, udp, quic, tls, tcp, http, icmp, arp, igmp

```
to analyze each protocol separately.

---

## 📡 Protocols Identified
- **DNS** – Resolves domain names to IP addresses.  
- **UDP** – Fast, connectionless protocol used by DNS and QUIC.  
- **QUIC** – Modern encrypted protocol for HTTP/3 running over UDP (port 443).  
- **TLS** – Provides encryption for HTTPS connections.  
- **TCP** – Reliable transport layer protocol for traditional HTTP/HTTPS.  
- **HTTP** – Web communication protocol for data exchange.  
- **ICMP** – Diagnostic protocol used for ping requests/replies.  
- **ARP** – Resolves IP addresses to MAC addresses on the local network.  
- **IGMP** – Manages multicast group memberships for network devices.

---

## 🧠 Key Learnings
- Understood how **UDP** and **QUIC** coexist — QUIC operates over UDP for modern encrypted web traffic.  
- Observed **TLS** handshakes and **encrypted QUIC sessions**, representing secure communication.  
- Learned how **DNS, ARP, and IGMP** operate at lower network layers.  
- Practiced Wireshark filtering, packet inspection, and protocol differentiation.  
- Gained insight into the transition from **HTTP/2 over TCP/TLS** to **HTTP/3 over QUIC/UDP**.

---

## 📊 Summary of Findings
| Aspect | Observation |
|--------|--------------|
| **Most Active Protocols** | UDP, QUIC, DNS, TLS |
| **Encryption Present** | Yes (TLS & QUIC) |
| **Local Network Activity** | ARP and IGMP packets detected |
| **Diagnostic Traffic** | ICMP echo requests and replies |
| **Transport Mechanisms** | Both UDP and TCP present |
| **Main Web Protocol** | HTTP/3 (QUIC) and HTTPS (TLS) |

---

## 📁 Files in Repository
| File | Description |
|------|--------------|
| `networkTraffic.pcapng` | Captured packet data |
| `Report_Network_Traffic_Analysis.pdf` | Detailed analysis report |
| `README.md` | Overview, procedure, and key results |

---

## ✅ Conclusion
The captured traffic demonstrates both traditional and modern internet communication.  
**UDP and QUIC** coexist — QUIC runs over UDP to deliver encrypted HTTP/3 traffic, while **TCP and TLS** handle legacy HTTPS connections.  
The capture also included **DNS, ICMP, and ARP**, representing normal system and local network operations.

This task enhanced practical knowledge of **packet analysis**, **protocol behavior**, and **secure communication flows**.

