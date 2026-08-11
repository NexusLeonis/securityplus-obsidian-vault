# 7. How Data Moves

[[00 - Overview|← Overview]]

**Related Security+ material:** [[3.1 - Network Infrastructure Concepts]] · [[3.2 - Secure Communication]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **Packet** | A formatted unit of data carried across an IP network. | Part of a webpage travels inside one packet. | Firewalls and routers inspect packet information. |
| **Frame** | A unit of data used for communication on a local network. | An Ethernet frame carries an IP packet to a switch. | Switches forward frames using MAC addresses. |
| [[2.5 - Segmentation and Access Control\|Segment]] | A unit of data created by TCP. | TCP divides a file into numbered segments. | TCP attacks target connection and segment behavior. |
| **Datagram** | A self-contained unit of data commonly associated with UDP. | A DNS request travels in a UDP datagram. | UDP sends datagrams without guaranteeing delivery. |
| **Header** | Control information placed before the actual data. | Source IP, destination IP, and protocol number. | Security devices inspect headers to make decisions. |
| **Payload** | The actual content carried inside a packet or frame. | Part of an email or webpage. | Encryption protects payloads from unauthorized viewing. |
| **Trailer** | Information placed at the end of certain data units. | An Ethernet frame includes an error-checking value. | Trailers help detect accidental transmission errors. |
| **Encapsulation** | Each networking layer wraps data with its own control information. | TCP adds a header, IP adds another, and Ethernet adds a frame. | Packet analysis requires understanding these nested layers. |
| **Decapsulation** | A receiving device removes each layer’s headers to reach the original data. | A web server unwraps the Ethernet, IP, and TCP information. | Attackers may craft malformed layers to confuse systems. |
| **Fragmentation** | Dividing a large IP packet into smaller pieces that fit the network. | A router splits a packet to cross a link with a smaller MTU. | Fragmented packets can bypass poorly configured security controls. |
| **Reassembly** | Combining fragments or segments back into the original data. | A receiving computer rebuilds a large packet. | Security devices must properly inspect reassembled traffic. |
| **MTU** | The largest packet size a network link can carry without fragmentation. | Ethernet commonly uses an MTU of 1,500 bytes. | Incorrect MTU settings can cause connection problems or evasions. |
| **Bandwidth** | The maximum amount of data a connection can carry over time. | A 1 Gbps network link. | Attackers may consume bandwidth during denial-of-service attacks. |
| **Throughput** | The amount of useful data actually transferred over time. | A 1 Gbps link delivers 700 Mbps in practice. | Low throughput may indicate congestion, failures, or attacks. |
| **Latency** | The delay between sending data and receiving a response. | A request takes 80 milliseconds to reach a server. | High latency affects applications and may signal routing problems. |
| **Jitter** | Variation in packet delay over time. | Voice packets arrive at uneven intervals. | Jitter harms voice and video quality. |
| **Packet loss** | Packets fail to reach their destination. | Two out of 100 packets disappear. | Loss can indicate congestion, bad links, filtering, or attacks. |
| **Full duplex** | A connection sends and receives data at the same time. | A modern Ethernet link. | Duplex mismatches can cause serious performance problems. |
| **Half duplex** | A connection can send or receive at one time, but not both simultaneously. | Older shared Ethernet equipment. | Collisions and poor performance occur more often. |
| **Collision** | Two devices transmit at the same time and their signals interfere. | Devices on an old Ethernet hub transmit together. | Modern switched networks largely eliminate collisions. |
| **QoS** | Rules that prioritize important traffic over less urgent traffic. | Voice calls receive priority over file downloads. | Attackers or misconfiguration can disrupt critical services. |

---
[[00 - Overview|← Overview]]
