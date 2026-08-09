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

## Technologies Used

* Wireshark
* Network Packet Capture
* Packet Analysis

## Protocols Analyzed

### DNS

Analyzed DNS queries and responses to understand how domain names are resolved into IP addresses.

### DHCP

Captured DHCP traffic to understand how devices obtain IP addresses and other network configuration details.

### TCP

Analyzed TCP communication, including the TCP three-way handshake:

```text
SYN → SYN-ACK → ACK
```

### ICMP / Ping

Analyzed ICMP traffic using the **Ping** command to understand network connectivity and Echo Request/Echo Reply packets.

### HTTP

Captured and analyzed HTTP requests and responses to understand unencrypted web communication.

### HTTPS

Analyzed HTTPS/TLS traffic to understand encrypted web communication and identify TLS packets.

### SSH

Captured SSH traffic to understand secure remote communication between systems.

## Wireshark Filters

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

## Skills Covered

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

## Learning Outcomes

Through this project, I gained hands-on experience in:

* Capturing network packets using Wireshark
* Identifying different network protocols
* Analyzing packet headers and communication patterns
* Understanding TCP connections and handshakes
* Troubleshooting network connectivity using ICMP/Ping
* Analyzing DNS and DHCP communication
* Understanding HTTP and HTTPS traffic
* Identifying encrypted TLS traffic
* Analyzing SSH network communication

## Project Structure

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
    ├── dns-analysis.png
    ├── dhcp-analysis.png
    ├── tcp-handshake.png
    ├── icmp-ping.png
    ├── http-analysis.png
    └── https-analysis.png
```

## Note

Packet captures can contain sensitive information such as IP addresses, hostnames, usernames, and other network details. Only upload packet captures that are safe to share publicly.

## Author

**Yuvasri**

---

⭐ If you found this project useful, consider giving the repository a star!
