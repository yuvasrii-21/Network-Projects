# Network Traffic Monitoring and Packet Analysis

## Purpose

The purpose of this project is to analyze network communication using packet capture and traffic analysis techniques.

## Project Description

Captured and analyzed different types of network traffic using **Wireshark** to understand protocol behavior, packet communication, and basic network troubleshooting techniques.

The following protocols were analyzed:

* DNS
* DHCP
* TCP
* ICMP
* HTTP
* HTTPS
* SSH

---

## Technologies Used

* Wireshark
* Network Packet Capture
* Packet Analysis

---

# Protocols Analyzed

## 1. DNS

Analyzed DNS queries and responses to understand how domain names are resolved into IP addresses.

### Wireshark Capture

![DNS Traffic Analysis](screenshots/DNS.png)

**Filter used:**

```text
dns
```

---

## 2. DHCP

Captured DHCP traffic to understand how devices obtain IP addresses and other network configuration details.

DHCP communication can include messages such as:

```text
Discover → Offer → Request → ACK
```

### Wireshark Capture

![DHCP Traffic Analysis](screenshots/DHCP.png)

**Filter used:**

```text
dhcp
```

---

## 3. TCP

Analyzed TCP communication, including the TCP three-way handshake.

```text
SYN → SYN-ACK → ACK
```

The TCP handshake establishes a reliable connection between two devices before data transmission.

### Wireshark Capture

![TCP Traffic Analysis](screenshots/TCP.png)

**Filter used:**

```text
tcp
```

---

## 4. ICMP / Ping

Analyzed ICMP traffic using the **Ping** command to understand network connectivity and Echo Request/Echo Reply packets.

Example:

```text
ping 8.8.8.8
```

ICMP communication can be observed as:

```text
Echo Request → Echo Reply
```

### Wireshark Capture

![ICMP Traffic Analysis](screenshots/ICMP.png)

**Filter used:**

```text
icmp
```

---

## 5. HTTP

Captured and analyzed HTTP requests and responses to understand unencrypted web communication.

HTTP traffic can expose application-layer information because it is not encrypted.

### Wireshark Capture

![HTTP Traffic Analysis](screenshots/HTTP.png)

**Filter used:**

```text
http
```

---

## 6. HTTPS / TLS

Analyzed HTTPS/TLS traffic to understand encrypted web communication and identify TLS packets.

Unlike HTTP, HTTPS encrypts application data using TLS, so the actual web content is generally not visible in the packet capture.

### Wireshark Capture

![HTTPS TLS Traffic Analysis](screenshots/HTTPS.png)

**Filter used:**

```text
tls
```

---

## 7. SSH

Captured SSH traffic to understand secure remote communication between systems.

SSH encrypts the communication between the client and server.

**Filter used:**

```text
ssh
```

> If you have an SSH screenshot, add it as `screenshots/SSH.png` and use:
>
> `![SSH Traffic Analysis](screenshots/SSH.png)`

---

# Wireshark Filters

The following Wireshark display filters were used during packet analysis:

```text
dns
dhcp
tcp
icmp
http
tls
ssh
```

---

# Skills Covered

* Wireshark
* Network Traffic Analysis
* Packet Capture
* DNS Analysis
* DHCP Analysis
* TCP Analysis
* ICMP Analysis
* Ping Analysis
* HTTP Analysis
* HTTPS/TLS Analysis
* SSH Analysis
* Network Troubleshooting

---

# Learning Outcomes

Through this project, I gained practical experience in:

* Capturing network packets using Wireshark
* Identifying different network protocols
* Analyzing packet headers and communication patterns
* Understanding TCP connections and three-way handshakes
* Troubleshooting network connectivity using ICMP/Ping
* Analyzing DNS and DHCP communication
* Understanding HTTP and HTTPS traffic
* Identifying encrypted TLS traffic
* Analyzing SSH network communication
* Using Wireshark display filters for protocol-specific analysis

---

# Project Structure

```text
Network-Traffic-Monitoring/
│
├── README.md
│
├── captures/
│   ├── dns.pcapng
│   ├── dhcp.pcapng
│   ├── tcp.pcapng
│   ├── icmp.pcapng
│   ├── http.pcapng
│   ├── https.pcapng
│   └── ssh.pcapng
│
└── screenshots/
    ├── DNS.png
    ├── DHCP.png
    ├── TCP.png
    ├── ICMP.png
    ├── HTTP.png
    ├── HTTPS.png
    └── SSH.png
```

---

# Security & Privacy Note

Packet captures can contain sensitive information such as:

* IP addresses
* MAC addresses
* Hostnames
* Usernames
* DNS queries
* Network infrastructure details
* Unencrypted application data

Only upload packet captures that are safe to share publicly.

For a public GitHub repository, **screenshots are generally safer than uploading raw `.pcapng` files**, especially if the captures contain traffic from your personal or college network.

Before publishing captures, review them in Wireshark and remove or avoid any sensitive information.

---

# Author

**Yuvasri**

---

⭐ If you found this project useful, consider giving the repository a star!
