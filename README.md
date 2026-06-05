

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

**SUMMARY**
### *Protocols Identified + Packet Details*

*1. IGMPv3 - Internet Group Management Protocol*
- *Packet #3*: Membership Query from `192.168.31.1` to `224.0.0.1`
- *Purpose*: Router checking which devices want multicast traffic


*2. UDP - User Datagram Protocol*
- *Packet #32*: Source `192.168.31.238` → Dest `192.168.31.1`, Port 53
- *Purpose*: DNS query transport. Connectionless, fast delivery

*3. ICMPv6 - Internet Control Message Protocol v6*
- *Packet #2*: Multicast Listener Report from `fe80::38ca:6bbd:d49d:9b49`
- *Purpose*: IPv6 neighbor discovery and network health checks


### *Output/Evidence*
- *packet capture*,protocol analysis,tcp/ip, network trouble shooting,filtering.


### *Outcome*
Gained hands-on packet analysis skills and protocol awareness.
