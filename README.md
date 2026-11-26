Multi-AS BGP Routing & Enterprise Network Services

A comprehensive Cisco Packet Tracer network simulation developed for the Computer Network Laboratory (ENCS4130) at Birzeit University. The project demonstrates inter-autonomous system routing using BGP alongside internal IGP redistribution and core enterprise application services.

Network Architecture & Protocols

Exterior Gateway Protocol (BGP): Configured eBGP peering across three distinct Autonomous Systems (AS XXX, AS YYY, and AS ZZZ) on the border routers, including custom BGP timer tuning (keepalive: 25s, hold-time: 75s) on Router1.

Interior Gateway Protocols (IGPs) & Redistribution:

AS XXX: Multi-Area OSPF (Process ID 1) spanning Area 0, Area 1, Area 2, and Area 3.

AS YYY: EIGRP (AS 10).

AS ZZZ: EIGRP (AS 20).

Implemented mutual route redistribution between BGP and the respective IGPs to achieve full end-to-end reachability across all autonomous systems.

IPv4 Subnetting (VLSM): Configured point-to-point serial links (/30) and multiple LAN segments (/24, /25, /26, /27, /29).

Enterprise Services Configured

DHCP & DHCP Relay:

Server-Based DHCP (Server0): Configured a pool to dynamically assign up to 32 IPv4 addresses in the 192.168.1.0/24 wireless subnet, utilizing an IP Helper Address (DHCP Relay) across routers.

Router-Based DHCP (Router2): Configured local DHCP services for 172.16.1.0/25 with reserved excluded host address ranges.

DNS Server (Server1): Configured Resource Records (A and MX records) to resolve internal web and mail domains.

HTTP Web Server: Hosted a custom webpage accessible via both www.DomainName.com and DomainName.com.

Email Server (SMTP/POP3): Configured user mailboxes under staff.DomainName.edu and verified cross-network email delivery between client endpoints.

Tools Used

Cisco Packet Tracer
