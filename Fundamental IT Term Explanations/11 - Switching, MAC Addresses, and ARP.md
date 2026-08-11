# 11. Switching, MAC Addresses, and ARP

[[00 - Overview|← Overview]]

**Related Security+ material:** [[3.2 - Port Security]] · [[3.2 - Network Appliances]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **MAC address table** | A switch’s list showing which MAC addresses appear on which ports. | The switch learns that a printer sits on port 8. | Attackers may overflow or manipulate this table. |
| **MAC learning** | A switch records the source MAC address of incoming frames. | Traffic from a PC teaches the switch its location. | This process allows efficient local delivery. |
| **Unknown unicast** | Traffic sent to a MAC address the switch has not learned. | The switch does not know where a new device resides. | The switch floods it, which may expose traffic to other ports. |
| **Flooding** | A switch copies traffic to multiple ports when it cannot identify the destination port. | An unknown destination frame reaches every port in the VLAN. | MAC flooding attacks intentionally trigger this behavior. |
| **ARP request** | A broadcast asking which device owns a particular IPv4 address. | “Who has 192.168.1.1?” | Every local device receives the request. |
| **ARP reply** | A response providing the MAC address associated with an IPv4 address. | The router replies with its MAC address. | Attackers can send forged ARP replies. |
| **ARP cache** | A device’s temporary table linking IPv4 addresses to MAC addresses. | A PC remembers the router’s MAC address. | Poisoning the cache can redirect local traffic. |
| **Gratuitous ARP** | An ARP message announcing a device’s IP-to-MAC mapping without receiving a request. | A backup router announces it has taken over an IP. | Attackers can abuse it to poison ARP caches. |
| **VLAN** | A logical network that separates devices even when they share the same physical switch. | HR and Finance use different VLANs. | VLANs limit broadcasts and reduce lateral movement. |
| **Access port** | A switch port assigned to one VLAN, normally for an endpoint. | A user PC connects to VLAN 20. | Incorrect access-port settings can place devices in the wrong network. |
| **Trunk port** | A switch port that carries traffic for multiple VLANs. | A link between two switches. | Trunks require protection against VLAN hopping. |
| **802.1Q** | The standard that adds VLAN identification tags to Ethernet frames. | A trunk marks a frame as VLAN 30. | Attackers may exploit poorly configured VLAN tagging. |
| **Native VLAN** | The VLAN that crosses an 802.1Q trunk without a tag by default. | Untagged traffic belongs to VLAN 1. | Mismatched native VLANs can create security problems. |
| [[3.2 - Port Security\|Port security]] | Switch controls that restrict which MAC addresses may use a port. | Only one approved workstation may connect to port 12. | It helps block unauthorized devices and MAC flooding. |
| **Network segmentation** | Dividing a network into smaller controlled sections. | Separate user, server, and guest networks. | Segmentation limits attacker movement and reduces exposure. |
| **Microsegmentation** | Applying very small, workload-specific communication boundaries. | One application server may contact only one database server. | It supports least privilege and zero-trust designs. |
| **Broadcast domain** | The group of devices that receive one another’s broadcast traffic. | All devices in the same VLAN. | Routers and VLANs separate broadcast domains. |
| **Collision domain** | The group of devices that could experience Ethernet collisions. | Each modern switch port forms its own collision domain. | Switches improve performance and reduce collisions. |
| **Spanning Tree Protocol** | A protocol that blocks redundant switch paths to prevent loops. | One backup link remains inactive until needed. | Attackers can manipulate STP if switches lack protections. |
| **Network loop** | A condition where frames circulate repeatedly between switches. | Two switches forward broadcasts back and forth forever. | Loops can overwhelm a network quickly. |

---
[[00 - Overview|← Overview]]
