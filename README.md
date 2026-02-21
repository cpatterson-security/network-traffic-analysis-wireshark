# Network Traffic Analysis Using Wireshark

## Objective

The objective of this lab was to capture and analyze live network traffic using Wireshark in order to observe different network protocols and understand how data is transmitted across a network.

---

## Lab Environment

- Platform: Kali Linux Virtual Machine
- Tool Used: Wireshark
- Network Interface: eth0

---

## Protocols Analyzed

- ICMP (Internet Control Message Protocol)
- DNS (Domain Name System)
- HTTP (Hypertext Transfer Protocol)

---

## Steps Performed

1. Started packet capture using Wireshark on the eth0 interface.
2. Generated ICMP traffic using the `ping` command to test network connectivity.
3. Used the `nslookup` command to generate DNS query traffic.
4. Accessed http://neverssl.com to generate unencrypted HTTP traffic.
5. Applied protocol filters in Wireshark to isolate ICMP, DNS, and HTTP packets.
6. Examined packet details including source IP, destination IP, protocol type, and packet structure.

---

## Evidence

### ICMP Packet Capture
![ICMP Capture](evidence/01-icmp-filter.png)

### DNS Packet Capture
![DNS Capture](evidence/02-dns-capture.png)

### HTTP Packet Capture
![HTTP Capture](evidence/03-http-filter.png)

---

## Key Skills Demonstrated

- Live packet capture using Wireshark
- Network traffic analysis
- Protocol filtering
- Identification of ICMP, DNS, and HTTP packets
- Understanding packet structure and communication behavior
