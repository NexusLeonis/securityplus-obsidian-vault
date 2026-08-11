# 18. Security Principles and Controls

[[00 - Overview|← Overview]]

**Related Security+ material:** [[1.1 - Security Controls]] · [[1.2 - The CIA Triad]] · [[1.2 - Zero Trust]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **Confidentiality** | Prevent unauthorized people from viewing information. | Encrypt employee medical records. | Disclosure attacks directly target confidentiality. |
| **Integrity** | Ensure information remains accurate and unaltered. | Verify a software download with a hash. | Attackers may modify files, transactions, or logs. |
| **Availability** | Keep systems and data accessible when authorized users need them. | Redundant servers keep a website running. | Denial-of-service and ransomware attacks target availability. |
| [[1.2 - The CIA Triad\|CIA triad]] | Confidentiality, integrity, and availability considered together. | Encrypt data, verify changes, and maintain backups. | Security+ uses this model throughout the exam. |
| [[1.2 - Authentication, Authorization, and Accounting\|Authentication]] | Verify that a user, device, or system is genuine. | A server proves its identity with a certificate. | It prevents impersonation. |
| [[1.2 - Non-repudiation\|Non-repudiation]] | Provide evidence that an action came from a particular identity. | A digitally signed contract. | It supports accountability and proof of origin. |
| [[5.4 - Privacy\|Privacy]] | Control how personal information gets collected, used, stored, and shared. | Limit access to employee records. | Privacy requirements influence security policies and controls. |
| **Risk** | The possibility that a threat will exploit a vulnerability and cause harm. | An exposed server may suffer data theft. | Security programs prioritize risks rather than eliminating every danger. |
| [[2.2 - Common Threat Vectors\|Threat]] | Anything capable of causing harm. | Criminal group, fire, malware, or careless employee. | Threats act against vulnerabilities. |
| [[2.1 - Threat Actors\|Threat actor]] | A person or group that intentionally conducts harmful activity. | Cybercriminal, insider, or nation-state team. | Different actors have different motives and capabilities. |
| [[4.3 - Vulnerability Scanning\|Vulnerability]] | A weakness that a threat can exploit. | An unpatched web server. | Vulnerability management identifies and reduces weaknesses. |
| **Exploit** | Code or a technique that takes advantage of a vulnerability. | Malicious traffic triggers a software flaw. | A vulnerability creates risk when attackers can exploit it. |
| **Attack vector** | The path or method used to reach and attack a target. | Phishing email, exposed RDP, or malicious USB. | Defenders must reduce likely attack vectors. |
| **Attack surface** | Every reachable system, service, account, and path an attacker could target. | Open ports, cloud services, users, and vendors. | Reducing the attack surface lowers opportunities for compromise. |
| **Exposure** | A condition that leaves a system or data accessible to potential harm. | A database accidentally allows public Internet access. | Exposure may exist even without a software vulnerability. |
| **Likelihood** | The probability that an event will occur. | A public unpatched server faces high likelihood of attack. | Risk assessments combine likelihood and impact. |
| [[5.2 - Business Impact Analysis\|Impact]] | The amount of harm an event would cause. | Payroll outage prevents employees from being paid. | High-impact risks may require strong controls even if unlikely. |
| **Risk appetite** | The amount and type of risk an organization willingly accepts. | A company accepts minor downtime but not customer-data loss. | It guides security investment and decision-making. |
| **Risk tolerance** | The acceptable variation around a risk objective. | A service may remain unavailable for no more than one hour. | It provides measurable limits for risk decisions. |
| **Risk mitigation** | Reducing the likelihood or impact of a risk. | Patch a vulnerable server and restrict its firewall rules. | Most security controls mitigate risk. |
| **Risk avoidance** | Removing the activity that creates the risk. | Stop using an unsupported application. | Avoidance eliminates that specific exposure. |
| **Risk transfer** | Shifting some financial or operational impact to another party. | Purchase cyber insurance. | Transfer does not remove the underlying vulnerability. |
| **Risk acceptance** | Formally choosing to live with a known risk. | Accept a low-impact legacy-system vulnerability temporarily. | Acceptance requires informed approval and documentation. |
| **Compensating control** | An alternative safeguard used when the preferred control is not possible. | Isolate an unpatchable system behind strict firewall rules. | It reduces risk without directly fixing the weakness. |
| **Preventive control** | A safeguard intended to stop an incident from occurring. | MFA prevents many unauthorized logins. | Prevention reduces the chance of compromise. |
| **Detective control** | A safeguard intended to identify incidents or suspicious activity. | An IDS alerts on malicious traffic. | Detection reveals activity that prevention missed. |
| **Corrective control** | A safeguard intended to fix damage or restore normal operations. | Reimaging an infected workstation. | Corrective controls support recovery. |
| **Deterrent control** | A safeguard intended to discourage unwanted actions. | Warning signs and visible cameras. | Deterrence may stop some individuals before they act. |
| **Directive control** | A rule or instruction that tells people what they must do. | A policy requires users to report phishing. | Policies and procedures guide secure behavior. |
| **Physical control** | A safeguard involving the physical environment. | Locks, fences, guards, and cameras. | Cybersecurity still depends on physical protection. |
| **Technical control** | A safeguard implemented through technology. | Firewall, encryption, or endpoint protection. | Technical controls directly enforce many security rules. |
| **Administrative control** | A safeguard based on management, policy, training, or process. | Background checks or security awareness training. | Administrative controls guide people and operations. |
| **Defense in depth** | Using multiple overlapping safeguards so one failure does not expose everything. | MFA, firewalls, endpoint security, and backups. | Layered defenses slow and contain attackers. |
| **Least functionality** | Enable only the features and services necessary for the system’s purpose. | Remove unused software and disable Telnet. | Fewer functions create fewer attack opportunities. |
| **Fail secure** | A system failure leaves access blocked rather than open. | A failed electronic lock remains locked. | Secure failure prevents accidental unauthorized access. |
| **Single point of failure** | One component whose failure stops the entire system. | One router provides all Internet access. | Redundancy removes or reduces single points of failure. |
| **Redundancy** | Duplicate components that take over when one fails. | Two power supplies or two Internet connections. | Redundancy improves availability. |
| **Resilience** | The ability to withstand disruption and continue or quickly restore operations. | A service shifts to another data center after failure. | Resilience combines prevention, response, and recovery. |

---
[[00 - Overview|← Overview]]
