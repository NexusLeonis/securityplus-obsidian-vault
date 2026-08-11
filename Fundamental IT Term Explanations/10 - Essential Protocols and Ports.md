# 10. Essential Protocols and Ports

[[00 - Overview|← Overview]]

**Related Security+ material:** [[4.5 - Secure Protocols]] · [[3.2 - Port Security]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **HTTP — TCP 80** | Transfers webpages and other web content without built-in encryption. | Visiting an http:// website. | Attackers can read or modify unencrypted HTTP traffic. |
| **HTTPS — TCP 443** | Uses HTTP over TLS to encrypt web communication. | Online banking website. | It protects data in transit and authenticates websites. |
| **TLS** | Encrypts application traffic and verifies identities with certificates. | A browser establishes a secure HTTPS connection. | Weak TLS settings can expose sensitive traffic. |
| **SSL** | The outdated predecessor to TLS. | Legacy systems may still reference SSL certificates. | SSL versions contain serious weaknesses and should not be used. |
| **FTP — TCP 20/21** | Transfers files but normally sends usernames, passwords, and data without encryption. | Uploading files to an old server. | Attackers can intercept FTP credentials and content. |
| **FTPS — TCP 989/990** | Secures FTP traffic with TLS. | Encrypted transfer to an FTP server. | It protects file-transfer credentials and data. |
| **SFTP — TCP 22** | Transfers files through an encrypted SSH connection. | Securely copying files to a Linux server. | It provides safer file transfer than standard FTP. |
| **TFTP — UDP 69** | A simple file-transfer protocol with no authentication or encryption. | Network devices download configuration files. | Attackers may steal or replace files on exposed TFTP servers. |
| **SSH — TCP 22** | Provides encrypted remote command-line access and file transfer. | An administrator securely manages a Linux server. | Strong keys and access controls protect remote administration. |
| **Telnet — TCP 23** | Provides remote command-line access without encryption. | Managing an old network device. | Anyone capturing traffic can read Telnet credentials. |
| **SMTP — TCP 25** | Transfers outgoing email between mail servers. | One organization’s mail server sends email to another. | Email spoofing and relay abuse involve SMTP. |
| **SMTP submission — TCP 587** | Allows authenticated users to submit outgoing email securely. | Outlook sends mail through an organization’s server. | Authentication prevents unauthorized mail relay. |
| **SMTPS — TCP 465** | Commonly provides SMTP protected by implicit TLS. | A mail client establishes an encrypted connection immediately. | It protects credentials and outgoing mail in transit. |
| **POP3 — TCP 110** | Downloads email from a server, often storing it locally. | An old mail client retrieves messages. | Standard POP3 does not encrypt credentials or messages. |
| **POP3S — TCP 995** | Protects POP3 email retrieval with TLS. | Securely downloading email. | It prevents interception of login information and mail. |
| **IMAP — TCP 143** | Lets clients manage email while messages remain on the server. | Multiple devices view the same mailbox. | Standard IMAP requires additional encryption for security. |
| **IMAPS — TCP 993** | Protects IMAP email access with TLS. | A phone securely synchronizes a mailbox. | It protects credentials and messages in transit. |
| **DNS — UDP/TCP 53** | Resolves names and exchanges DNS information. | Looking up the IP address for example.com. | DNS supports spoofing, tunneling, poisoning, and amplification attacks. |
| **DHCP — UDP 67/68** | Automatically assigns IP addresses and other network settings. | A laptop joins Wi-Fi. | Rogue DHCP and DHCP starvation attacks target this service. |
| **SNMP — UDP 161** | Monitors and manages network devices. | A monitoring server checks switch status. | Weak SNMP credentials can expose or change device configurations. |
| **SNMP trap — UDP 162** | Allows devices to send alerts to a monitoring server. | A router reports that an interface failed. | Attackers may spoof alerts or exploit weak SNMP configurations. |
| **SNMPv3** | A secure SNMP version that supports authentication and encryption. | Encrypted monitoring of routers and switches. | It replaces insecure community strings used by older versions. |
| **LDAP — TCP/UDP 389** | Queries and updates directory information. | An application looks up a user account. | Standard LDAP can expose directory traffic unless protected. |
| **LDAPS — TCP 636** | Protects LDAP communication with TLS. | An application securely queries Active Directory. | It protects directory credentials and information. |
| **Kerberos — TCP/UDP 88** | Uses tickets to authenticate users and services without repeatedly sending passwords. | A user logs into a Windows domain. | Ticket theft and weak service accounts can undermine Kerberos. |
| **SMB — TCP 445** | Provides Windows file, printer, and resource sharing. | Opening a shared network folder. | SMB vulnerabilities and weak shares commonly support lateral movement. |
| **NetBIOS — TCP/UDP 137–139** | Older Windows networking services for names, sessions, and file sharing. | Legacy Windows systems locate shared resources. | Attackers can exploit exposed or misconfigured NetBIOS services. |
| **RDP — TCP/UDP 3389** | Provides remote graphical access to Windows systems. | Remotely controlling a Windows server. | Exposed RDP attracts password attacks and ransomware operators. |
| **NTP — UDP 123** | Synchronizes clocks across systems. | Domain computers match the same time source. | Accurate time supports logs, certificates, and Kerberos. |
| **Syslog — UDP 514** | Sends system and device log messages to a central server. | A firewall sends alerts to a SIEM. | Central logs support detection and incident investigation. |
| **Secure syslog — TCP 6514** | Sends syslog data through TLS. | A router securely sends logs to a collector. | Encryption prevents log interception and manipulation. |
| **ICMP** | Sends network status, error, and diagnostic messages. | ping uses ICMP echo messages. | Attackers use ICMP for discovery, tunneling, or denial of service. |
| **ARP** | Finds the MAC address associated with a local IPv4 address. | “Who has 192.168.1.1?” | ARP spoofing enables local traffic interception. |
| **SIP — TCP/UDP 5060** | Establishes and manages voice or video calls. | Starting a VoIP phone call. | Attackers may hijack calls or abuse exposed SIP services. |
| **SRTP** | Encrypts the audio or video carried during real-time communications. | Protecting the voice content of a VoIP call. | It prevents interception of call media. |
| **RTP** | Carries real-time audio and video but does not encrypt it by itself. | Streaming voice packets during a call. | Unprotected RTP traffic can reveal conversations. |
| **SQL Server — TCP 1433** | Common default port for Microsoft SQL Server. | An application connects to a Microsoft database. | Exposed databases attract credential and injection attacks. |
| **MySQL — TCP 3306** | Common default port for MySQL databases. | A web application connects to MySQL. | Database access should remain restricted to authorized systems. |
| **PostgreSQL — TCP 5432** | Common default port for PostgreSQL databases. | An application queries a PostgreSQL server. | Exposed database ports can reveal sensitive records. |
| **VNC — TCP 5900** | Provides remote graphical desktop access. | A technician remotely controls a workstation. | Weak VNC passwords and encryption expose systems. |
| **IPsec — UDP 500/4500** | Protects IP traffic and commonly supports VPN connections. | A site-to-site VPN joins two offices. | IPsec provides authentication, integrity, and encryption. |

---
[[00 - Overview|← Overview]]
