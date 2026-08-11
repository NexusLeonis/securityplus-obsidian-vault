# 5. DNS and Name Resolution

[[00 - Overview|← Overview]]

**Related Security+ material:** [[2.4 - DNS Attacks]] · [[4.5 - Web Filtering]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **DNS** | A system that translates domain names into IP addresses and stores other domain information. | google.com resolves to a Google IP address. | DNS attacks can redirect, monitor, or disrupt users. |
| **DNS server** | A physical or virtual server running software that answers DNS questions. | An ISP, Google, or company operates the server. | DNS server security affects everyone relying on its answers. |
| **DNS resolver** | A server that finds DNS answers for clients by contacting other DNS servers. | Your router forwards a query to an ISP resolver. | A compromised resolver can give many clients false answers. |
| **Recursive query** | A request asking a DNS resolver to find the complete answer. | Your PC asks, “What is the IP for example.com?” | Recursive resolvers may face abuse or denial-of-service attacks. |
| **Root DNS server** | A top-level DNS server that directs resolvers toward the correct domain extension. | It points .com queries toward .com servers. | Root servers form part of DNS’s global hierarchy. |
| **TLD server** | A DNS server responsible for a top-level domain such as .com or .org. | The .com server points toward example.com DNS servers. | It helps resolvers locate authoritative information. |
| **Authoritative DNS server** | The DNS server that holds the official records for a domain. | The server officially states the IP for example.com. | Compromising it can redirect all users of the domain. |
| **DNS cache** | Temporarily saved DNS answers that reduce repeated lookups. | Your computer remembers a site’s IP for several minutes. | Cache poisoning inserts false information into stored answers. |
| **TTL** | The amount of time a DNS record may remain cached. | A record has a TTL of 3,600 seconds. | TTL affects how quickly legitimate or malicious DNS changes spread. |
| **A record** | A DNS record that maps a name to an IPv4 address. | www.example.com → 192.0.2.10. | Attackers may alter A records to redirect traffic. |
| **AAAA record** | A DNS record that maps a name to an IPv6 address. | www.example.com → 2001:db8::10. | Security controls must account for IPv6 records and traffic. |
| **CNAME record** | A DNS record that makes one name an alias of another name. | store.example.com points to shops.vendor.com. | Misconfigured aliases can expose or redirect services. |
| **MX record** | A DNS record that identifies the servers receiving email for a domain. | Mail for example.com goes to mail.example.com. | Attackers may target or manipulate mail routing. |
| **TXT record** | A DNS record that stores text-based information. | SPF and domain-verification information. | Email security systems use TXT records to detect spoofing. |
| **PTR record** | A DNS record that maps an IP address back to a hostname. | 192.0.2.10 → mail.example.com. | Reverse lookups help verify systems and investigate logs. |
| **DNSSEC** | A system that digitally signs DNS records so resolvers can verify their authenticity. | A resolver rejects a forged DNS response. | DNSSEC helps prevent DNS spoofing and cache poisoning. |
| **Hosts file** | A local file that manually maps names to IP addresses before DNS is used. | Mapping testserver to 192.168.1.50. | Malware can modify it to redirect users. |

---
[[00 - Overview|← Overview]]
