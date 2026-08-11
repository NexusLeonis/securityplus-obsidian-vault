# CompTIA Security+ (SY0-701) — Exam Objectives Summary

Condensed study map of the official CompTIA objectives. Use the **[[attachments/CompTIA Security+ (SY0-701) Exam Objectives.pdf|official SY0-701 Exam Objectives PDF]] as the source of truth**.

This page keeps the **action CompTIA expects for each objective** front and center. The wording matters: some objectives ask you to compare concepts, some to explain them, and others expect you to apply them in a scenario.

[[Home|← Home]]  |  [[01 - Contents|Contents →]]  |  [[Study Method|Study Method →]]

---

## [[1.0 - General Security Concepts|1.0 — General Security Concepts (12%)]]

### 1.1 — Security Controls
**CompTIA expects:** **Compare and contrast** various types of security controls.

**Study emphasis:** Know how the categories and control types differ from one another, not just their definitions.

- **Categories:** technical, managerial, operational, physical
- **Control types:** preventive, deterrent, detective, corrective, compensating, directive

### 1.2 — Fundamental Security Concepts
**CompTIA expects:** **Summarize** fundamental security concepts.

**Study emphasis:** Understand the purpose and relationship of the major security principles and recognize what each concept is doing.

- Confidentiality, Integrity, and Availability (CIA)
- Non-repudiation
- Authentication, Authorization, and Accounting (AAA)
- Authenticating people and systems
- Authorization models
- Gap analysis
- Zero Trust
  - Control plane
  - Data plane
  - Policy Administrator / Policy Engine / Policy Enforcement Point
- Physical security controls
- Deception and disruption technologies: honeypot, honeynet, honeyfile, honeytoken

### 1.3 — Change Management
**CompTIA expects:** **Explain the importance** of change management processes and their impact to security.

**Study emphasis:** Understand why controlled change matters and what can go wrong when business, technical, or documentation requirements are ignored.

- Approval process, ownership, stakeholders, impact analysis
- Test results, backout plans, maintenance windows, standard operating procedures
- Allow lists / deny lists, restricted activities, downtime, service or application restarts
- Legacy applications and dependencies
- Updating diagrams, policies, and procedures
- Version control

### 1.4 — Cryptographic Solutions
**CompTIA expects:** **Explain the importance of using appropriate cryptographic solutions.**

**Study emphasis:** Know what each cryptographic method protects, when it is appropriate, and how the major technologies differ.

- Public key infrastructure (PKI)
- Public and private keys, key escrow
- Encryption levels and use cases
- Symmetric vs. asymmetric encryption
- Key exchange, algorithms, key length
- TPM, HSM, key management systems, secure enclaves
- Steganography, tokenization, data masking
- Hashing, salting, digital signatures, key stretching
- Blockchain and open public ledgers
- Certificates, CAs, CRLs, OCSP, roots of trust, CSRs, wildcard certificates

---

## [[2.0 - Threats, Vulnerabilities, and Mitigations|2.0 — Threats, Vulnerabilities, and Mitigations (22%)]]

### 2.1 — Threat Actors and Motivations
**CompTIA expects:** **Compare and contrast** common threat actors and motivations.

**Study emphasis:** Be able to distinguish attackers by their capabilities, resources, position, and motivation.

- Nation-state
- Unskilled attacker
- Hacktivist
- Insider threat
- Organized crime
- Shadow IT
- Internal vs. external actors
- Resources, funding, sophistication, capability
- Motivations including financial gain, espionage, disruption, revenge, political beliefs, blackmail, and war

### 2.2 — Threat Vectors and Attack Surfaces
**CompTIA expects:** **Explain** common threat vectors and attack surfaces.

**Study emphasis:** Understand how an attacker gets access or creates an opportunity for attack.

- Message-based, image-based, file-based, voice, and removable-device vectors
- Vulnerable software
- Unsupported systems and applications
- Unsecure wired, wireless, and Bluetooth networks
- Open service ports
- Default credentials
- Supply-chain vectors
- Human vectors and social engineering
- Phishing, vishing, smishing, impersonation, BEC, pretexting, watering holes, typosquatting

### 2.3 — Vulnerabilities
**CompTIA expects:** **Explain** various types of vulnerabilities.

**Study emphasis:** Know what makes each vulnerability possible and how the major vulnerability classes differ.

- Memory injection
- Buffer overflow
- Race conditions: TOC / TOU
- Malicious updates
- OS-based vulnerabilities
- SQL injection and XSS
- Firmware, end-of-life, and legacy hardware
- VM escape and resource reuse
- Cloud-specific vulnerabilities
- Supply-chain vulnerabilities
- Cryptographic vulnerabilities
- Misconfiguration
- Mobile side loading and jailbreaking
- Zero-day vulnerabilities

### 2.4 — Indicators of Malicious Activity
**CompTIA expects:** **Given a scenario, analyze indicators of malicious activity.**

**Study emphasis:** This is an application objective. Connect symptoms and indicators to the likely attack rather than memorizing attack names in isolation.

- Malware: ransomware, Trojan, worm, spyware, bloatware, virus, keylogger, logic bomb, rootkit
- Physical attacks
- DDoS, DNS, wireless, on-path, replay, and malicious-code attacks
- Application attacks
- Cryptographic attacks
- Password spraying and brute force
- Indicators such as account lockouts, impossible travel, abnormal resource usage, inaccessible resources, missing logs, and out-of-cycle logging

### 2.5 — Mitigation Techniques
**CompTIA expects:** **Explain the purpose** of mitigation techniques used to secure the enterprise.

**Study emphasis:** Know what problem each mitigation addresses and why you would choose it.

- Segmentation
- Access control, ACLs, permissions
- Application allow lists
- Isolation
- Patching
- Encryption
- Monitoring
- Least privilege
- Configuration enforcement
- Decommissioning
- Hardening
- Endpoint protection, host firewalls, HIPS
- Disabling unnecessary ports and protocols
- Changing default passwords
- Removing unnecessary software

---

## [[3.0 - Security Architecture|3.0 — Security Architecture (18%)]]

### 3.1 — Architecture Models
**CompTIA expects:** **Compare and contrast** the security implications of different architecture models.

**Study emphasis:** Understand the security tradeoffs between architectures, not simply what each architecture is.

- Cloud, hybrid, and third-party considerations
- Infrastructure as code (IaC)
- Serverless and microservices
- Physical isolation and air gaps
- Logical segmentation and SDN
- On-premises
- Centralized vs. decentralized
- Containerization and virtualization
- IoT
- ICS / SCADA
- RTOS and embedded systems
- High availability
- Availability, resilience, cost, responsiveness, scalability, recovery, patching, power, and compute considerations

### 3.2 — Securing Enterprise Infrastructure
**CompTIA expects:** **Given a scenario, apply security principles** to secure enterprise infrastructure.

**Study emphasis:** Choose and place the right controls for a scenario.

- Device placement and security zones
- Attack surface and connectivity
- Fail-open vs. fail-closed
- Active vs. passive devices
- Inline vs. tap/monitor
- Jump servers and proxy servers
- IDS / IPS
- Load balancers and sensors
- 802.1X and EAP
- WAF, UTM, NGFW, Layer 4 / Layer 7 firewalls
- VPN, remote access, tunneling, TLS, IPSec
- SD-WAN and SASE
- Selection of effective controls

### 3.3 — Protecting Data
**CompTIA expects:** **Compare and contrast** concepts and strategies to protect data.

**Study emphasis:** Distinguish data types, classifications, states, and protection methods, including when one method fits better than another.

- Regulated, trade secret, intellectual property, legal, and financial data
- Human- and non-human-readable data
- Sensitive, confidential, public, restricted, private, and critical classifications
- Data at rest, in transit, and in use
- Data sovereignty and geolocation
- Geographic restrictions
- Encryption, hashing, masking, tokenization, obfuscation
- Segmentation and permission restrictions

### 3.4 — Resilience and Recovery
**CompTIA expects:** **Explain the importance** of resilience and recovery in security architecture.

**Study emphasis:** Understand how architecture choices keep services available and restore operations after failure.

- Load balancing vs. clustering
- Hot, cold, and warm sites
- Geographic dispersion
- Platform diversity
- Multi-cloud systems
- Continuity of operations
- Capacity planning
- Tabletop exercises, failover, simulation, parallel processing
- Backups, snapshots, replication, journaling
- Generators and UPS

---

## [[4.0 - Operations and Incident Response|4.0 — Security Operations (28%)]]

### 4.1 — Securing Computing Resources
**CompTIA expects:** **Given a scenario, apply common security techniques** to computing resources.

**Study emphasis:** Choose practical hardening and security settings for different systems and device types.

- Secure baselines: establish, deploy, maintain
- Hardening mobile devices, workstations, switches, routers, cloud infrastructure, servers, ICS/SCADA, RTOS, IoT, embedded systems
- Wireless site surveys and heat maps
- MDM
- BYOD, COPE, CYOD
- Cellular, Wi-Fi, Bluetooth
- WPA3, RADIUS, cryptographic and authentication protocols
- Input validation, secure cookies, static code analysis, code signing
- Sandboxing and monitoring

### 4.2 — Asset Management
**CompTIA expects:** **Explain the security implications** of proper hardware, software, and data asset management.

**Study emphasis:** Understand how security changes across the asset lifecycle.

- Acquisition and procurement
- Assignment and accounting
- Ownership and classification
- Inventory and enumeration
- Monitoring and asset tracking
- Disposal and decommissioning
- Sanitization, destruction, certification
- Data retention

### 4.3 — Vulnerability Management
**CompTIA expects:** **Explain** activities associated with vulnerability management.

**Study emphasis:** Know the full vulnerability-management process from discovery through validation and reporting.

- Vulnerability scanning
- Static and dynamic application analysis
- Package monitoring
- Threat feeds, OSINT, third-party intelligence, information-sharing organizations, dark web
- Penetration testing
- Responsible disclosure and bug bounty programs
- Audits
- False positives and false negatives
- CVSS and CVE
- Prioritization, exposure, organizational impact, risk tolerance
- Patching, segmentation, compensating controls, exceptions
- Rescanning, audit, verification
- Reporting

### 4.4 — Security Alerting and Monitoring
**CompTIA expects:** **Explain** security alerting and monitoring concepts and tools.

**Study emphasis:** Understand what is monitored, what the tools do, and what happens after an alert.

- Systems, applications, and infrastructure monitoring
- Log aggregation
- Alerting
- Scanning
- Reporting and archiving
- Quarantine
- Alert tuning
- SCAP and benchmarks
- Agents vs. agentless
- SIEM
- Antivirus
- DLP
- SNMP traps
- NetFlow
- Vulnerability scanners

### 4.5 — Enterprise Security Capabilities
**CompTIA expects:** **Given a scenario, modify enterprise capabilities to enhance security.**

**Study emphasis:** Apply or change enterprise security controls based on the problem presented.

- Firewall rules, access lists, ports, protocols, screened subnets
- IDS / IPS signatures and trends
- Web filtering
- Group Policy and SELinux
- Secure protocol, port, and transport selection
- DNS filtering
- DMARC, DKIM, SPF, email gateways
- File integrity monitoring
- DLP
- NAC
- EDR / XDR
- User behavior analytics

### 4.6 — Identity and Access Management
**CompTIA expects:** **Given a scenario, implement and maintain** identity and access management.

**Study emphasis:** Choose and manage identity, authentication, authorization, and privileged-access controls.

- Provisioning and de-provisioning
- Permission assignments
- Identity proofing
- Federation and SSO
- LDAP, OAuth, SAML
- Interoperability and attestation
- Mandatory, discretionary, role-based, rule-based, and attribute-based access control
- Time-of-day restrictions
- Least privilege
- MFA implementations and factors
- Password practices, managers, passwordless authentication
- Privileged access management
- Just-in-time permissions, password vaulting, ephemeral credentials

### 4.7 — Automation and Orchestration
**CompTIA expects:** **Explain the importance** of automation and orchestration related to secure operations.

**Study emphasis:** Understand where automation helps, what benefits it provides, and what risks or tradeoffs it introduces.

- User and resource provisioning
- Guard rails and security groups
- Ticket creation and escalation
- Enabling or disabling services and access
- Continuous integration and testing
- APIs and integrations
- Efficiency, consistency, scaling, reaction time
- Complexity, cost, single points of failure, technical debt, supportability

### 4.8 — Incident Response
**CompTIA expects:** **Explain appropriate incident response activities.**

**Study emphasis:** Know the incident-response process and what actions belong at each stage.

- Preparation
- Detection
- Analysis
- Containment
- Eradication
- Recovery
- Lessons learned
- Training
- Tabletop exercises and simulations
- Root cause analysis
- Threat hunting
- Digital forensics
- Legal hold, chain of custody, acquisition, preservation, reporting, e-discovery

### 4.9 — Investigation Data Sources
**CompTIA expects:** **Given a scenario, use data sources** to support an investigation.

**Study emphasis:** Know which evidence source can answer the investigative question presented.

- Firewall logs
- Application logs
- Endpoint logs
- OS security logs
- IDS / IPS logs
- Network logs
- Metadata
- Vulnerability scans
- Automated reports
- Dashboards
- Packet captures

---

## [[5.0 - Governance, Risk, and Compliance|5.0 — Security Program Management and Oversight (20%)]]

### 5.1 — Security Governance
**CompTIA expects:** **Summarize** elements of effective security governance.

**Study emphasis:** Understand how governance documents, structures, responsibilities, and external requirements fit together.

- Guidelines
- Policies: AUP, information security, business continuity, disaster recovery, incident response, SDLC, change management
- Standards
- Procedures
- Regulatory, legal, industry, local, national, and global considerations
- Monitoring and revision
- Boards, committees, government entities
- Centralized vs. decentralized governance
- Owners, controllers, processors, custodians, stewards

### 5.2 — Risk Management
**CompTIA expects:** **Explain** elements of the risk management process.

**Study emphasis:** Understand the complete risk process and how the measurements and response strategies relate.

- Risk identification
- Risk assessment
- Qualitative vs. quantitative analysis
- SLE, ALE, ARO
- Probability, likelihood, exposure factor, impact
- Risk register
- Key risk indicators
- Risk owners and thresholds
- Risk tolerance and appetite
- Transfer, accept, avoid, mitigate
- Exceptions and exemptions
- Risk reporting
- Business impact analysis
- RTO, RPO, MTTR, MTBF

### 5.3 — Third-Party Risk
**CompTIA expects:** **Explain the processes** associated with third-party risk assessment and management.

**Study emphasis:** Understand how organizations evaluate, select, contract with, and monitor vendors.

- Vendor assessment
- Penetration testing
- Right-to-audit clauses
- Internal audit evidence and independent assessments
- Supply-chain analysis
- Due diligence and conflict of interest
- SLA, MOA, MOU, MSA, SOW, NDA, BPA
- Vendor monitoring
- Questionnaires
- Rules of engagement

### 5.4 — Security Compliance
**CompTIA expects:** **Summarize** elements of effective security compliance.

**Study emphasis:** Understand how compliance is monitored, reported, and enforced, including privacy obligations.

- Internal and external compliance reporting
- Fines, sanctions, reputational damage, loss of license, contractual impacts
- Due diligence and due care
- Attestation and acknowledgement
- Internal and external monitoring
- Automation
- Privacy
- Local, national, and global legal implications
- Data subjects
- Controller vs. processor
- Ownership
- Data inventory and retention
- Right to be forgotten

### 5.5 — Audits and Assessments
**CompTIA expects:** **Explain the types and purposes** of audits and assessments.

**Study emphasis:** Distinguish who performs each assessment, why it is performed, and what kind of testing is involved.

- Attestation
- Internal compliance audits
- Audit committees
- Self-assessments
- Regulatory examinations
- External assessments
- Independent third-party audits
- Penetration testing
- Physical, offensive, defensive, and integrated testing
- Known, partially known, and unknown environments
- Passive and active reconnaissance

### 5.6 — Security Awareness
**CompTIA expects:** **Given a scenario, implement** security awareness practices.

**Study emphasis:** Apply the right awareness or training response to the user behavior or organizational problem presented.

- Phishing campaigns
- Recognizing phishing attempts
- Responding to suspicious-message reports
- Risky, unexpected, and unintentional behavior
- Policy and handbook guidance
- Situational awareness
- Insider threat
- Password management
- Removable media and cables
- Social engineering
- Operational security
- Hybrid and remote work
- Initial and recurring reporting and monitoring
- Program development and execution

---

[[Home|← Home]]  |  [[01 - Contents|Contents →]]
