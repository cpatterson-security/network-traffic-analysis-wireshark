# Wireshark Network Traffic Analysis Lab (Kali Linux)

## Objective
Capture and analyze ICMP, DNS, and HTTP network traffic using Wireshark in a Kali Linux virtual lab environment to observe protocol behavior and practice packet filtering.

## Lab Environment
- Attacker/Analyst VM: Kali Linux
- Tool: Wireshark
- Traffic generation: Terminal + web browser (Firefox)

## Tools Used
- Wireshark
- Terminal (ping, nslookup)
- Firefox (HTTP test site)

## Methodology (What I Did)
1. Started a capture in Wireshark on the active network interface.
2. Generated ICMP traffic:
   - `ping 8.8.8.8`
3. Generated DNS traffic:
   - `nslookup example.com`
4. Generated HTTP traffic:
   - Visited `http://neverssl.com`
5. Applied display filters in Wireshark to isolate each protocol and reviewed packet details.

## Evidence (Screenshots)

### 01 - ICMP Display Filter
![01-icmp-filter](evidence/01-icmp-filter.png)

### 02 - DNS Capture / Filter
![02-dns-capture](evidence/02-dns-capture.png)

### 03 - HTTP Display Filter
![03-http-filter](evidence/03-http-filter.png)

## Packet Captures (PCAPs)
- ICMP Capture: [icmp-capture.pcapng](pcaps/icmp-capture.pcapng)
- DNS Capture: [dns-capture.pcapng](pcaps/dns-capture.pcapng)
- HTTP Capture: [http-capture-trimmed.pcapng](pcaps/http-capture-trimmed.pcapng)

## Analysis Summary
### ICMP
- Observed echo requests and replies.
- Confirmed connectivity between the Kali host and an external IP.

### DNS
- Observed DNS queries and responses.
- Verified domain name resolution to IP addresses.

### HTTP
- Observed unencrypted HTTP requests and responses.
- Verified how readable HTTP traffic can be when not protected by TLS.

## Conclusion
This lab demonstrated how to capture live traffic, apply Wireshark display filters, and analyze ICMP, DNS, and HTTP packets. These skills support troubleshooting, threat detection, and security monitoring in real environments.
