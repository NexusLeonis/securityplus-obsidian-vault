# 6. DHCP and Automatic Configuration

[[00 - Overview|← Overview]]

**Related Security+ material:** [[3.1 - Network Infrastructure Concepts]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **DHCP** | A service that automatically gives devices IP configuration information. | A laptop joins Wi-Fi and receives an IP address. | Rogue DHCP servers can redirect or disrupt clients. |
| **DHCP server** | The system that assigns IP settings to clients. | A router hands out home-network addresses. | Attackers may impersonate or exhaust the DHCP server. |
| **DHCP client** | A device requesting network configuration from DHCP. | A new phone joining office Wi-Fi. | Client behavior forms part of DHCP attacks and troubleshooting. |
| **DHCP lease** | A temporary assignment of an IP address to a device. | A laptop receives an address for eight hours. | Devices must renew leases to keep using their addresses. |
| **DHCP scope** | The pool of addresses and settings a DHCP server can provide. | 192.168.1.100–192.168.1.200. | Exhausting the scope can prevent legitimate devices from connecting. |
| **DHCP reservation** | A rule that always gives one device the same IP address. | A printer always receives 192.168.1.50. | Stable addressing helps manage and secure important devices. |
| **DORA** | The four-step DHCP process: Discover, Offer, Request, Acknowledge. | A client finds a server and accepts an offered address. | Understanding DORA helps identify rogue DHCP and starvation attacks. |
| **DNS setting from DHCP** | DHCP usually tells a client which DNS server to use. | A laptop receives both an IP and DNS server address. | A rogue DHCP server can direct users to a malicious DNS server. |
| **Default gateway from DHCP** | DHCP usually tells a client which router provides access outside the subnet. | The client receives 192.168.1.1 as its gateway. | A false gateway can intercept or block traffic. |

---
[[00 - Overview|← Overview]]
