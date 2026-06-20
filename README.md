# Home Network Security Lab

## Overview

This project demonstrates a hands-on home lab focused on network security, traffic analysis, and wireless attack techniques. The goal was to simulate real-world attacker behavior in a controlled and ethical environment.

## Lab Environment

* Kali Linux (Attacker Machine)
* Personal Home Network (Isolated testing scope)
* VMware Fusion (Virtualization)

## Tools Used

* Nmap (Network Discovery & Scanning)
* Wireshark (Packet Analysis)
* Aircrack-ng (WiFi Security Testing)

## Objectives

* Discover active devices on a network
* Analyze packet-level traffic during scanning
* Capture and analyze WiFi authentication handshakes
* Perform password cracking on captured data
* Understand common attack methodologies used in real environments

---

## 1. Network Discovery

Performed network scanning using Nmap to identify active hosts on the local subnet.

**Command Used:**

```
nmap -sn 192.168.40.0/24
```

**Outcome:**

* Identified multiple active devices on the network
* Selected targets for further enumeration

---

## 2. Packet Capture & Analysis

Used Wireshark to capture live network traffic during scanning.

**Focus Areas:**

* ARP Requests/Replies
* ICMP Traffic (Ping Sweep)

**Key Insight:**
Observed how Nmap generates ARP and ICMP packets to discover hosts, providing visibility into how attackers map networks.

---

## 3. WiFi Handshake Capture

Captured a WPA2 handshake using wireless monitoring tools.

**Process:**

* Enabled monitor mode
* Targeted specific access point
* Captured authentication handshake

**Outcome:**
Successfully captured handshake data for offline analysis.

---

## 4. Password Cracking

Performed offline password cracking against the captured handshake.

**Tool Used:**

* Aircrack-ng

**Outcome:**

* Successfully recovered the WiFi password from the captured handshake
* Demonstrated risks of weak passwords in wireless networks

---

## Results

* Successfully mapped a local network
* Captured and analyzed packet-level traffic
* Demonstrated wireless attack techniques
* Identified security weaknesses in a controlled environment

---

## Key Takeaways

* Network discovery is a critical first step in any attack
* Packet analysis provides deep visibility into network behavior
* Weak passwords significantly increase security risk
* Wireless networks are vulnerable without proper configuration

---

## Disclaimer

This project was conducted in a controlled home lab environment for educational purposes only. No unauthorized systems were targeted.

---

## Screenshots

See the `/screenshots` folder for:

* Nmap scan results
* Wireshark packet captures
* WiFi handshake capture
* Password cracking results
