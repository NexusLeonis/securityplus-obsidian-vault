# 19. Security Monitoring and Response Tools

[[00 - Overview|← Overview]]

**Related Security+ material:** [[4.4 - Security Monitoring]] · [[4.4 - Security Tools]] · [[4.8 - Incident Response]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **Antivirus** | Software that identifies and removes known malicious files or behavior. | It quarantines an infected attachment. | Traditional antivirus forms one layer of endpoint protection. |
| **Anti-malware** | A broader term for software that detects many types of malicious code. | It blocks spyware and ransomware. | Modern tools combine signature and behavior detection. |
| **EDR** | Endpoint software that records activity and helps detect, investigate, and respond to threats. | An analyst isolates a compromised laptop remotely. | EDR provides deeper visibility than basic antivirus. |
| **XDR** | A platform that combines detection data across endpoints, networks, email, cloud, and identity. | One alert links a phishing email to endpoint malware. | It improves cross-system detection and investigation. |
| **SIEM** | A system that collects and analyzes logs from many sources. | Firewall, server, and identity logs feed one platform. | SIEM supports centralized detection and investigation. |
| **SOAR** | Technology that automates security workflows and response actions. | Automatically disable an account after confirmed credential theft. | SOAR reduces repetitive analyst work and response time. |
| **DLP** | Controls that detect or prevent unauthorized movement of sensitive data. | Block Social Security numbers from leaving through email. | DLP protects confidentiality and supports compliance. |
| **NAC** | Technology that checks users or devices before allowing network access. | Block a laptop that lacks required antivirus. | NAC enforces access and device-health requirements. |
| **NIDS** | An IDS that monitors network traffic. | A sensor detects exploit traffic crossing a network link. | It sees network behavior but may miss encrypted content. |
| **HIDS** | An IDS that monitors activity on one host. | A server detects changes to critical files. | It provides visibility inside the endpoint. |
| **Signature-based detection** | Detection that matches activity against known malicious patterns. | An antivirus recognizes a known malware hash. | It works well for known threats but may miss new ones. |
| **Behavior-based detection** | Detection that identifies suspicious actions rather than exact known patterns. | A document launches PowerShell and encrypts many files. | It can detect new or modified threats. |
| **Anomaly detection** | Detection that flags activity that differs from an established normal pattern. | A user downloads far more data than usual. | It can identify unknown threats but may create false positives. |
| **False positive** | A security tool reports malicious activity when the activity is legitimate. | A normal admin script triggers an alert. | Excessive false positives waste analyst time. |
| **False negative** | A security tool fails to detect actual malicious activity. | Malware runs without triggering an alert. | False negatives allow real threats to continue. |
| **Vulnerability scanner** | A tool that checks systems for known weaknesses and misconfigurations. | Scanning servers for missing patches. | Findings help prioritize remediation. |
| **Port scanner** | A tool that identifies listening ports and services. | Nmap finds ports 22 and 443 open. | Defenders and attackers both use port scanning. |
| **Packet analyzer** | A tool that captures and displays network traffic. | Wireshark shows DNS and TCP packets. | Analysts use it to troubleshoot and investigate attacks. |
| **Sandbox** | An isolated environment used to safely run and observe suspicious files or code. | An email attachment executes inside a controlled VM. | Sandboxing reveals behavior without risking production systems. |
| **Quarantine** | Isolating a suspicious file, device, or message so it cannot cause further harm. | Antivirus moves malware into a protected folder. | Quarantine contains threats while analysts investigate. |
| **Indicator of compromise** | Evidence suggesting that a security incident occurred. | Malicious IP, file hash, or unusual registry key. | IOCs support detection and threat hunting. |
| **Indicator of attack** | Evidence that an attack is currently developing or being attempted. | Repeated credential attempts followed by privilege escalation. | IOAs focus on attacker behavior rather than artifacts alone. |
| [[4.3 - Threat Intelligence\|Threat intelligence]] | Collected information about threats, actors, tools, and indicators. | A feed lists malicious domains used by ransomware groups. | It improves detection and risk decisions. |
| [[4.8 - Incident Response\|Incident]] | An event that harms or threatens confidentiality, integrity, or availability. | Malware compromises a workstation. | Incident response processes manage and contain damage. |
| [[3.2 - Intrusion Prevention\|Event]] | Any observable occurrence on a system or network. | A successful login. | Most events are normal; some become alerts or incidents. |
| **Alert** | A notification that a tool detected something potentially important. | SIEM reports repeated failed logins. | Analysts must validate alerts before declaring incidents. |
| **Containment** | Actions that limit an incident’s spread and damage. | Disconnect an infected device from the network. | Fast containment protects remaining systems. |
| **Eradication** | Removing the threat and its persistence mechanisms. | Delete malware and close the exploited vulnerability. | Eradication prevents the attacker from returning through the same path. |
| [[3.4 - Recovery Testing\|Recovery]] | Restoring systems and operations after an incident. | Rebuild servers and monitor them for reinfection. | Recovery returns the organization to normal operation. |
| **Root cause analysis** | Determining the underlying reason an incident occurred. | The breach began with an unpatched VPN appliance. | Fixing root causes reduces repeat incidents. |

---
[[00 - Overview|← Overview]]
