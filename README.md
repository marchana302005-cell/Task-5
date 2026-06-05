

### *Objective*
Capture live network packets using Wireshark and identify basic protocols and traffic types.

### *Tools Used*
- *Wireshark* v4.x (free packet analyzer)
- *Windows 11* Wi-Fi Interface
- *GitHub Desktop* for evidence repository

### *Deliverables*
1. *Packet Capture File*: `elevate_task5.pcap` - 285 packets captured
2. *GitHub Repository*: Contains .pcap files
3. *Protocol Analysis Report*: Summary below


### *Protocols Identified + Packet Details*

*1. IGMPv3 - Internet Group Management Protocol*
- *Packet #3*: Membership Query from `192.168.31.1` to `224.0.0.1`
- *Purpose*: Router checking which devices want multicast traffic
- *GRC Relevance*: Normal multicast management. Absence of unexpected IGMP joins indicates no rogue multicast apps

*2. UDP - User Datagram Protocol*
- *Packet #32*: Source `192.168.31.238` → Dest `192.168.31.1`, Port 53
- *Purpose*: DNS query transport. Connectionless, fast delivery
- *GRC Relevance*: Confirms DNS requests use UDP as per standard. Excessive UDP could indicate DDoS

*3. ICMPv6 - Internet Control Message Protocol v6*
- *Packet #2*: Multicast Listener Report from `fe80::38ca:6bbd:d49d:9b49`
- *Purpose*: IPv6 neighbor discovery and network health checks
- *GRC Relevance*: Standard IPv6 operation. Unexpected ICMPv6 redirects are a red flag in audits

*4. DNS - Domain Name System*
- *Packet #29*: Standard query `0x6782` for `HTTPS web.whatsapp.com`
- *Packet #30*: Response with `AAAA` record `2a03:2880:f281:1c:face:b00c:0:167`
- *Purpose*: Resolving domain names to IP addresses
- *GRC Relevance*: DNS logs are critical for detecting data exfiltration, phishing domains, or DNS tunneling

### *Output/Evidence*
- *Total Packets*: 285 captured, 19 displayed after filtering
- *packet capture*,protocol analysis,tcp/ip, network trouble shooting,filtering.


### *Outcome*
Gained hands-on packet analysis skills and protocol awareness.
