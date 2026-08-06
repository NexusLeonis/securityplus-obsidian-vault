# 8. OSI and TCP-IP Models

[[00 - Overview|← Overview]]

**Related Security+ material:** [[3.1 - Network Infrastructure Concepts]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **OSI model** | A seven-layer model used to describe how network communication works. | Physical through Application layers. | Security+ uses OSI layers to classify technologies and attacks. |
| **Layer 1: Physical** | Sends raw electrical, radio, or light signals. | Cables, connectors, and wireless signals. | Physical attacks include cable cuts, jamming, and device theft. |
| **Layer 2: Data Link** | Handles local delivery using frames and MAC addresses. | Ethernet switches and VLANs. | ARP spoofing, MAC flooding, and VLAN attacks operate here. |
| **Layer 3: Network** | Routes packets between networks using IP addresses. | Routers forward IPv4 packets. | IP spoofing and routing attacks operate here. |
| **Layer 4: Transport** | Manages communication between applications using TCP or UDP and port numbers. | TCP port 443 carries HTTPS traffic. | Port scans and SYN floods target this layer. |
| **Layer 5: Session** | Establishes, manages, and ends communication sessions. | Maintaining a logged-in connection. | Session hijacking targets established sessions. |
| **Layer 6: Presentation** | Translates, formats, compresses, and encrypts data. | TLS encrypts application data. | Encryption and encoding often relate to this layer. |
| **Layer 7: Application** | Provides network services directly to applications and users. | HTTP, DNS, SMTP, and FTP. | Many attacks target application protocols and user input. |
| **TCP/IP model** | The practical model used by modern Internet networks. | Link, Internet, Transport, and Application layers. | It groups the same functions as the OSI model in fewer layers. |
| **Layer 2 switch** | A switch that forwards traffic using MAC addresses. | A basic office Ethernet switch. | VLAN and MAC-table security occurs here. |
| **Layer 3 switch** | A switch that can also route traffic between IP networks or VLANs. | Routing between Finance and HR VLANs. | It combines fast switching with routing and access controls. |

---
[[00 - Overview|← Overview]]
