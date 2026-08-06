# 12. Routing, NAT, and Internet Access

[[00 - Overview|← Overview]]

**Related Security+ material:** [[3.2 - Secure Infrastructures]] · [[3.1 - Network Infrastructure Concepts]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **Routing** | Selecting a path for packets to travel between networks. | A router forwards traffic from a LAN toward an ISP. | Route manipulation can redirect or intercept traffic. |
| **Routing table** | A list of networks and the next path used to reach them. | A default route sends unknown destinations to the ISP. | Incorrect or malicious routes can disrupt communication. |
| **Static route** | A route manually entered by an administrator. | Send 10.10.0.0/16 through one router. | Static routes remain predictable but require manual maintenance. |
| **Dynamic routing** | Routers automatically exchange information and update routes. | OSPF routers learn network changes. | Attackers may inject false routing information. |
| **Default route** | The path used when no more specific route exists. | 0.0.0.0/0 points toward the Internet. | A false default route can capture most outbound traffic. |
| **Next hop** | The next router that should receive a packet. | A LAN router sends traffic to the ISP router. | Routing tables identify next-hop addresses. |
| **Hop** | One router-to-router step along a packet’s path. | A packet crosses eight routers to reach a server. | traceroute displays these steps. |
| **TTL in IP** | A counter that decreases at each router and stops packets from circulating forever. | A packet expires after too many hops. | Unusual TTL values can assist traffic analysis. |
| **NAT** | A router changes IP address information as traffic moves between networks. | A private address becomes a public address. | NAT hides internal addressing but does not replace a firewall. |
| **Static NAT** | One private address always maps to one public address. | A public IP permanently maps to an internal server. | It allows predictable inbound access but increases exposure. |
| **Dynamic NAT** | Private devices temporarily receive addresses from a pool of public addresses. | Several users share a limited public-address pool. | The mapping changes as connections begin and end. |
| **PAT** | Many private devices share one public IP by using different port numbers. | Every home device accesses the Internet through one public IP. | Most home routers use PAT. |
| **Port forwarding** | A router sends traffic arriving on a public port to an internal system. | Public port 443 forwards to an internal web server. | It intentionally exposes an internal service to outside traffic. |
| **Source NAT** | NAT changes the source address of outgoing traffic. | A laptop’s private IP becomes the router’s public IP. | It commonly supports Internet access. |
| **Destination NAT** | NAT changes the destination address of incoming traffic. | Public traffic redirects to a private server. | It supports published internal services. |
| **ACL** | An ordered list of rules that permits or denies traffic. | Allow HTTPS from users but deny database access. | Routers, firewalls, and switches use ACLs to enforce policy. |
| **Implicit deny** | Traffic not specifically permitted gets blocked at the end of a ruleset. | A firewall allows ports 80 and 443 and blocks everything else. | Administrators must account for the unseen final deny rule. |
| **North-south traffic** | Traffic entering or leaving an organization or data center. | Employees access an Internet website. | Perimeter controls primarily inspect north-south traffic. |
| **East-west traffic** | Traffic moving between internal systems. | An application server contacts a database server. | Attackers use east-west traffic for lateral movement. |
| **ping** | A tool that tests basic IP reachability using ICMP. | ping 8.8.8.8. | It helps identify connectivity and filtering issues. |
| **traceroute / tracert** | A tool that shows the routers a packet crosses toward a destination. | Viewing each hop between a PC and a website. | It helps identify route changes and failed network segments. |

---
[[00 - Overview|← Overview]]
