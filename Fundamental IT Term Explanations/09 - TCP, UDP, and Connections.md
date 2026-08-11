# 9. TCP, UDP, and Connections

[[00 - Overview|← Overview]]

**Related Security+ material:** [[2.4 - Denial of Service]] · [[2.4 - On-path Attacks]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **TCP** | A connection-based protocol that numbers data, confirms delivery, and retransmits missing pieces. | Downloading a webpage or sending email. | TCP supports reliable services but faces connection-based attacks. |
| **UDP** | A connectionless protocol that sends data without confirming every delivery. | Streaming, gaming, DNS, or voice calls. | UDP is fast but easier to spoof and abuse for amplification. |
| **Connection-oriented** | Communication establishes a session before transferring application data. | TCP completes a handshake before sending a webpage. | Stateful devices can track and secure established connections. |
| **Connectionless** | Communication sends individual messages without first establishing a session. | UDP sends a DNS request immediately. | Attackers can spoof source addresses more easily. |
| **TCP three-way handshake** | TCP starts a connection with SYN, SYN-ACK, and ACK messages. | A browser establishes a connection to a web server. | SYN floods abuse this process to exhaust server resources. |
| **SYN** | A TCP flag used to request a new connection and synchronize sequence numbers. | Client sends SYN to a server. | Large numbers of SYN packets may indicate a SYN flood. |
| **SYN-ACK** | A TCP response that accepts a connection request and returns synchronization information. | Server replies to the client’s SYN. | Attackers may exploit incomplete handshakes. |
| **ACK** | A TCP message confirming receipt of data or connection information. | Client acknowledges the server’s SYN-ACK. | Firewalls inspect ACK flags when tracking sessions. |
| **FIN** | A TCP flag used to close a connection normally. | A browser finishes and closes a web session. | Attackers may use unusual FIN scans to identify ports. |
| **RST** | A TCP flag that immediately resets or rejects a connection. | A closed port responds with RST. | Scanners use response behavior to determine port status. |
| **Sequence number** | A TCP value that places received data in the correct order. | Segments 1, 2, and 3 rebuild a file. | Predictable sequence numbers can support session hijacking. |
| **Acknowledgment** | Confirmation that specific TCP data arrived. | Receiver confirms it received bytes through a certain number. | Missing acknowledgments trigger retransmission. |
| **Retransmission** | Sending TCP data again when the sender believes it was lost. | Packet 3 disappears, so TCP resends it. | Excessive retransmissions may indicate congestion or interference. |
| **Port number** | A number that identifies a specific service or application on a host. | HTTPS commonly uses TCP port 443. | Firewalls and scans rely heavily on port numbers. |
| **Well-known port** | A port from 0 through 1023 commonly assigned to standard services. | SSH uses port 22. | Exposed well-known ports reveal available services. |
| **Registered port** | A port from 1024 through 49151 associated with applications or vendors. | Microsoft SQL Server often uses port 1433. | Administrators must know which applications require these ports. |
| **Ephemeral port** | A temporary high-numbered port selected by a client for one connection. | Your browser uses a temporary source port when contacting port 443. | Firewalls must allow valid return traffic to these ports. |
| **Listening port** | A port where a service waits for incoming connections. | A web server listens on port 443. | Every listening port increases the system’s attack surface. |
| **Open port** | A port where a service accepts connections. | SSH accepts a connection on port 22. | Attackers scan for open ports and vulnerable services. |
| **Closed port** | A reachable port with no service accepting connections. | TCP port 23 responds that it is closed. | Closed ports reveal the host exists but deny the service. |
| **Filtered port** | A port where a firewall or filter prevents a clear response. | A scanner receives no response from port 3389. | Filtering hides or blocks access to services. |

---
[[00 - Overview|← Overview]]
