# 3. Network Devices

[[00 - Overview|← Overview]]

**Related Security+ material:** [[3.2 - Secure Infrastructures]] · [[3.2 - Network Appliances]] · [[3.2 - Firewall Types]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **Switch** | A device that connects systems on the same local network and forwards traffic using MAC addresses. | A switch connects office computers and printers. | Switches support VLANs, port security, and network segmentation. |
| **Router** | A device that connects different networks and forwards traffic using IP addresses. | A home router connects your LAN to the Internet. | Routers enforce routes, ACLs, and network boundaries. |
| **Modem** | A device that translates signals between your local equipment and your ISP’s connection. | Cable modem connected to a home router. | The modem provides the physical path to the ISP. |
| **Wireless access point** | A device that connects wireless devices to a wired network. | An office ceiling-mounted Wi-Fi access point. | Access points require secure encryption and configuration. |
| **Wireless controller** | A system that centrally manages multiple access points. | A controller configures every access point in a building. | Central management improves consistency but creates a valuable target. |
| **Hub** | An older device that sends incoming traffic to every connected port. | One PC sends data and every PC receives a copy. | Hubs make packet sniffing easier and provide no traffic separation. |
| **Bridge** | A device that connects two network segments and filters traffic by MAC address. | Connecting two parts of a LAN. | Bridges perform a simpler form of switching. |
| **Repeater** | A device that regenerates a weak signal so it can travel farther. | Extending a network cable run. | Repeaters extend signals but do not inspect or secure traffic. |
| **Gateway** | A device or service that connects systems using different networks or protocols. | A router serves as the default gateway for a LAN. | Compromising a gateway can expose or redirect large amounts of traffic. |
| **Default gateway** | The router a device sends traffic to when the destination lies outside the local network. | Your PC sends Internet traffic to 192.168.1.1. | A false gateway can enable interception or loss of connectivity. |
| [[4.5 - Firewalls\|Firewall]] | A device or program that allows or blocks traffic according to rules. | Permit HTTPS but block Telnet. | Firewalls reduce unauthorized access between networks. |
| **Stateful firewall** | A firewall that remembers active connections and allows related return traffic. | It allows a response to a web request you initiated. | Stateful filtering makes smarter decisions than simple port filtering. |
| **Stateless firewall** | A firewall that evaluates each packet separately without remembering the connection. | Block every packet from a specific IP address. | Stateless rules work quickly but lack connection context. |
| **Next-generation firewall** | A firewall that also identifies applications, users, and advanced threats. | Blocking social media traffic regardless of port. | It provides deeper control than traditional packet filtering. |
| **Proxy server** | A server that makes requests on behalf of clients. | Employees browse the web through a company proxy. | Proxies can filter, log, cache, and hide client addresses. |
| **Forward proxy** | A proxy that represents internal clients when they access external resources. | A company proxy accesses websites for employees. | It controls outbound access and records user activity. |
| **Reverse proxy** | A proxy that represents servers and receives client traffic before the servers do. | A reverse proxy sits in front of a web application. | It hides internal servers and can provide filtering or load balancing. |
| **Load balancer** | A device or service that spreads requests across multiple servers. | Website traffic divides among four web servers. | Load balancing improves availability and can remove failed servers. |
| **IDS** | A system that detects suspicious activity and raises alerts. | It alerts on known malware traffic. | An IDS observes but normally does not block the traffic. |
| **IPS** | A system that detects suspicious activity and automatically blocks it. | It drops packets matching an exploit signature. | An IPS can stop attacks in real time. |
| **Network tap** | Hardware that copies network traffic to a monitoring device. | Sending traffic copies to a packet analyzer. | Security teams use taps for visibility without changing traffic. |
| **Packet broker** | A device that collects and directs copied traffic to monitoring tools. | Sending web traffic to one sensor and email traffic to another. | It helps security tools inspect the correct traffic efficiently. |
| **VPN concentrator** | A device that manages many encrypted VPN connections. | Hundreds of remote workers connect to one concentrator. | It becomes a critical remote-access security point. |
| **Bastion host** | A heavily secured system placed where administrators can safely reach protected systems. | Administrators enter through a hardened jump server. | It reduces direct exposure of internal servers. |
| **Jump server** | A controlled system administrators use before connecting to sensitive systems. | Admins connect to the jump server, then to database servers. | It centralizes privileged access and auditing. |
| **Honeypot** | A decoy system designed to attract attackers. | A fake vulnerable server records attack attempts. | It helps detect, study, and distract attackers. |
| **Honeynet** | A network containing multiple decoy systems. | Fake servers, users, and services imitate a real environment. | It provides broader visibility into attacker behavior. |

---
[[00 - Overview|← Overview]]
