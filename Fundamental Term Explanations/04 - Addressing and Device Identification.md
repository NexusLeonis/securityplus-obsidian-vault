# 4. Addressing and Device Identification

[[00 - Overview|← Overview]]

**Related Security+ material:** [[3.1 - Network Infrastructure Concepts]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **IP address** | A logical address that tells networks where a device resides and where to send packets. | 192.168.1.25 | Routing, filtering, logging, and many attacks depend on IP addresses. |
| **IPv4** | The older and still common IP format that uses four decimal numbers. | 10.20.30.40 | Security+ questions commonly use IPv4 addressing. |
| **IPv6** | A newer IP format with a much larger address space. | 2001:db8::25 | IPv6 introduces different addressing and security considerations. |
| **Public IP address** | An address that systems can route across the public Internet. | Your ISP assigns your router a public address. | Public systems face direct Internet exposure. |
| **Private IP address** | An address reserved for internal networks and not routed directly across the Internet. | 192.168.1.25 | NAT usually translates private addresses before Internet access. |
| **APIPA** | An automatic IPv4 address used when a device cannot reach DHCP. | 169.254.10.20 | An APIPA address usually indicates a DHCP or connectivity problem. |
| **Loopback address** | An address a device uses to communicate with itself. | 127.0.0.1 or ::1. | Administrators use loopback to test local networking and services. |
| **localhost** | A hostname that refers to the current device. | Opening localhost accesses a local web server. | Malware and administrators may use local-only services. |
| **MAC address** | A hardware address that identifies a network interface on the local network. | 00:1A:2B:3C:4D:5E | Switches and ARP use MAC addresses for local delivery. |
| **OUI** | The first part of a MAC address that identifies the manufacturer. | A prefix associated with Cisco or Dell. | Analysts can use it to identify unfamiliar devices. |
| **Hostname** | A human-readable name assigned to a device. | FINANCE-PC-07. | Hostnames help identify systems in logs and directories. |
| **Domain name** | A human-readable name used instead of an IP address. | example.com. | Attackers imitate and manipulate domain names. |
| **FQDN** | The complete DNS name showing a specific host and its domain. | mail.example.com. | Certificates, DNS records, and access rules often use FQDNs. |
| **URL** | The complete address used to locate a resource. | https://example.com/login. | Phishing and web attacks often rely on deceptive URLs. |
| **URI** | A general identifier for a resource; a URL is one type of URI. | https://example.com/file.pdf. | Security tools may inspect or filter resource identifiers. |
| **Subnet** | A smaller network created inside a larger IP network. | Finance uses 192.168.10.0/24. | Subnets improve organization, routing, and segmentation. |
| **Subnet mask** | A value that tells a device which part of an IPv4 address identifies the network. | 255.255.255.0. | Devices use it to decide whether traffic stays local or goes to a router. |
| **CIDR notation** | A shorter way to show an IP network and subnet size. | 192.168.1.0/24. | Firewall rules and network diagrams commonly use CIDR notation. |
| **Network address** | The address that represents an entire subnet rather than one device. | 192.168.1.0 in a /24. | Routes and firewall rules may apply to the whole network. |
| **Broadcast address** | An IPv4 address that sends traffic to every device in a subnet. | 192.168.1.255 in a /24. | Broadcast traffic can support discovery or enable certain attacks. |
| **Unicast** | Communication from one sender to one receiver. | Your PC sends a request to one web server. | Most normal network traffic uses unicast. |
| **Broadcast** | Communication from one sender to every device on the local subnet. | An ARP request asks all devices for a MAC address. | Excessive broadcasts can expose data or reduce performance. |
| **Multicast** | Communication from one sender to a selected group of receivers. | Streaming video to subscribed devices. | Multicast requires proper network and access controls. |
| **Anycast** | Multiple servers share one address, and routing sends users to a nearby available server. | Global DNS providers use anycast. | Anycast improves performance and resilience against failures. |
| **Socket** | The combination of an IP address and a port that identifies one network connection endpoint. | 192.168.1.20:443. | Logs and firewall rules often identify connections by sockets. |

---
[[00 - Overview|← Overview]]
