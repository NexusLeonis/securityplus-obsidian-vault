# Contents

Clickable table of contents, following Professor Messer's SY0-701 course notes order exactly. Page numbers reference the official course notes PDF.

Check a box once you've completed that topic's **learning loop**: Messer notes + one video pass + immediate recall. The progress bars below read directly off these checkboxes.

[[Home|← Home]]  |  [[00 - CompTIA Objectives Summary|Objectives Summary →]]  | 


%% First-pass history remains in Daily Notes/2026-08-04 through 2026-08-10. Contents reset on 2026-08-11 for the 60-day relearn. %%

---

```dataviewjs
const page = dv.page(dv.current().file.path);
const tasks = page.file.tasks;
const groups = {};
const order = [];
for (const t of tasks) {
    const h = t.section ? t.section.subpath : "Other";
    if (!groups[h]) { groups[h] = {done: 0, total: 0}; order.push(h); }
    groups[h].total++;
    if (t.completed) groups[h].done++;
}
function bar(done, total, len) {
    const filled = total > 0 ? Math.round(len * done / total) : 0;
    return "\u2588".repeat(filled) + "\u2591".repeat(len - filled);
}
let totalDone = 0, totalAll = 0;
for (const h of order) {
    const g = groups[h];
    totalDone += g.done; totalAll += g.total;
    const pct = g.total > 0 ? Math.round(100 * g.done / g.total) : 0;
    dv.paragraph(`**${h}**: ${g.done}/${g.total} (${pct}%)  \`${bar(g.done, g.total, 20)}\``);
}
const pctAll = totalAll > 0 ? Math.round(100 * totalDone / totalAll) : 0;
dv.paragraph(`---\n**Overall**: ${totalDone}/${totalAll} (${pctAll}%)  \`${bar(totalDone, totalAll, 20)}\``);
```

---

## 1.0 - General Security Concepts (p.1)
[[1.0 - General Security Concepts|→ Domain overview]]

- [ ] [[1.1 - Security Controls|1.1 - Security Controls]] — p.1
- [ ] [[1.2 - The CIA Triad|1.2 - The CIA Triad]] — p.2
- [ ] [[1.2 - Non-repudiation|1.2 - Non-repudiation]] — p.3
- [ ] [[1.2 - Authentication, Authorization, and Accounting|1.2 - Authentication, Authorization, and Accounting]] — p.4
- [ ] [[1.2 - Gap Analysis|1.2 - Gap Analysis]] — p.5
- [ ] [[1.2 - Zero Trust|1.2 - Zero Trust]] — p.5
- [ ] [[1.2 - Physical Security|1.2 - Physical Security]] — p.7
- [ ] [[1.2 - Deception and Disruption|1.2 - Deception and Disruption]] — p.7
- [ ] [[1.3 - Change Management|1.3 - Change Management]] — p.8
- [ ] [[1.3 - Technical Change Management|1.3 - Technical Change Management]] — p.9
- [ ] [[1.4 - Public Key Infrastructure|1.4 - Public Key Infrastructure]] — p.10
- [ ] [[1.4 - Encrypting Data|1.4 - Encrypting Data]] — p.11
- [ ] [[1.4 - Key Exchange|1.4 - Key Exchange]] — p.11
- [ ] [[1.4 - Encryption Technologies|1.4 - Encryption Technologies]] — p.12
- [ ] [[1.4 - Obfuscation|1.4 - Obfuscation]] — p.13
- [ ] [[1.4 - Hashing and Digital Signatures|1.4 - Hashing and Digital Signatures]] — p.14
- [ ] [[1.4 - Blockchain Technology|1.4 - Blockchain Technology]] — p.15
- [ ] [[1.4 - Certificates|1.4 - Certificates]] — p.16

## 2.0 - Threats, Vulnerabilities, and Mitigations (p.18)
[[2.0 - Threats, Vulnerabilities, and Mitigations|→ Domain overview]]

- [ ] [[2.1 - Threat Actors|2.1 - Threat Actors]] — p.18
- [ ] [[2.2 - Common Threat Vectors|2.2 - Common Threat Vectors]] — p.19
- [ ] [[2.2 - Phishing|2.2 - Phishing]] — p.20
- [ ] [[2.2 - Impersonation|2.2 - Impersonation]] — p.21
- [ ] [[2.2 - Watering Hole Attacks|2.2 - Watering Hole Attacks]] — p.21
- [ ] [[2.2 - Other Social Engineering Attacks|2.2 - Other Social Engineering Attacks]] — p.22
- [ ] [[2.3 - Memory Injections|2.3 - Memory Injections]] — p.22
- [ ] [[2.3 - Buffer Overflows|2.3 - Buffer Overflows]] — p.23
- [ ] [[2.3 - Race Conditions|2.3 - Race Conditions]] — p.23
- [ ] [[2.3 - Malicious Updates|2.3 - Malicious Updates]] — p.24
- [ ] [[2.3 - Operating System Vulnerabilities|2.3 - Operating System Vulnerabilities]] — p.24
- [ ] [[2.3 - SQL Injection|2.3 - SQL Injection]] — p.25
- [ ] [[2.3 - Cross-site Scripting|2.3 - Cross-site Scripting]] — p.25
- [ ] [[2.3 - Hardware Vulnerabilities|2.3 - Hardware Vulnerabilities]] — p.26
- [ ] [[2.3 - Virtualization Vulnerabilities|2.3 - Virtualization Vulnerabilities]] — p.27
- [ ] [[2.3 - Cloud-specific Vulnerabilities|2.3 - Cloud-specific Vulnerabilities]] — p.27
- [ ] [[2.3 - Supply Chain Vulnerabilities|2.3 - Supply Chain Vulnerabilities]] — p.28
- [ ] [[2.3 - Misconfiguration Vulnerabilities|2.3 - Misconfiguration Vulnerabilities]] — p.28
- [ ] [[2.3 - Mobile Device Vulnerabilities|2.3 - Mobile Device Vulnerabilities]] — p.29
- [ ] [[2.3 - Zero-day Vulnerabilities|2.3 - Zero-day Vulnerabilities]] — p.29
- [ ] [[2.4 - An Overview of Malware|2.4 - An Overview of Malware]] — p.30
- [ ] [[2.4 - Viruses and Worms|2.4 - Viruses and Worms]] — p.30
- [ ] [[2.4 - Spyware and Bloatware|2.4 - Spyware and Bloatware]] — p.31
- [ ] [[2.4 - Other Malware Types|2.4 - Other Malware Types]] — p.32
- [ ] [[2.4 - Physical Attacks|2.4 - Physical Attacks]] — p.32
- [ ] [[2.4 - Denial of Service|2.4 - Denial of Service]] — p.33
- [ ] [[2.4 - DNS Attacks|2.4 - DNS Attacks]] — p.33
- [ ] [[2.4 - Wireless Attacks|2.4 - Wireless Attacks]] — p.34
- [ ] [[2.4 - On-path Attacks|2.4 - On-path Attacks]] — p.34
- [ ] [[2.4 - Replay Attacks|2.4 - Replay Attacks]] — p.35
- [ ] [[2.4 - Malicious Code|2.4 - Malicious Code]] — p.36
- [ ] [[2.4 - Application Attacks|2.4 - Application Attacks]] — p.36
- [ ] [[2.4 - Cryptographic Attacks|2.4 - Cryptographic Attacks]] — p.38
- [ ] [[2.4 - Password Attacks|2.4 - Password Attacks]] — p.39
- [ ] [[2.4 - Indicators of Compromise|2.4 - Indicators of Compromise]] — p.39
- [ ] [[2.5 - Segmentation and Access Control|2.5 - Segmentation and Access Control]] — p.40
- [ ] [[2.5 - Mitigation Techniques|2.5 - Mitigation Techniques]] — p.41
- [ ] [[2.5 - Hardening Techniques|2.5 - Hardening Techniques]] — p.41

## 3.0 - Security Architecture (p.42)
[[3.0 - Security Architecture|→ Domain overview]]

- [ ] [[3.1 - Cloud Infrastructures|3.1 - Cloud Infrastructures]] — p.42
- [ ] [[3.1 - Network Infrastructure Concepts|3.1 - Network Infrastructure Concepts]] — p.44
- [ ] [[3.1 - Other Infrastructure Concepts|3.1 - Other Infrastructure Concepts]] — p.44
- [ ] [[3.1 - Infrastructure Considerations|3.1 - Infrastructure Considerations]] — p.45
- [ ] [[3.2 - Secure Infrastructures|3.2 - Secure Infrastructures]] — p.47
- [ ] [[3.2 - Intrusion Prevention|3.2 - Intrusion Prevention]] — p.48
- [ ] [[3.2 - Network Appliances|3.2 - Network Appliances]] — p.48
- [ ] [[3.2 - Port Security|3.2 - Port Security]] — p.50
- [ ] [[3.2 - Firewall Types|3.2 - Firewall Types]] — p.50
- [ ] [[3.2 - Secure Communication|3.2 - Secure Communication]] — p.51
- [ ] [[3.3 - Data Types and Classifications|3.3 - Data Types and Classifications]] — p.53
- [ ] [[3.3 - States of Data|3.3 - States of Data]] — p.53
- [ ] [[3.3 - Protecting Data|3.3 - Protecting Data]] — p.54
- [ ] [[3.4 - Resiliency|3.4 - Resiliency]] — p.55
- [ ] [[3.4 - Capacity Planning|3.4 - Capacity Planning]] — p.56
- [ ] [[3.4 - Recovery Testing|3.4 - Recovery Testing]] — p.57
- [ ] [[3.4 - Backups|3.4 - Backups]] — p.57
- [ ] [[3.4 - Power Resiliency|3.4 - Power Resiliency]] — p.58

## 4.0 - Operations and Incident Response (p.59)
[[4.0 - Operations and Incident Response|→ Domain overview]]

- [ ] [[4.1 - Secure Baselines|4.1 - Secure Baselines]] — p.59
- [ ] [[4.1 - Hardening Targets|4.1 - Hardening Targets]] — p.59
- [ ] [[4.1 - Securing Wireless and Mobile|4.1 - Securing Wireless and Mobile]] — p.60
- [ ] [[4.1 - Wireless Security Settings|4.1 - Wireless Security Settings]] — p.61
- [ ] [[4.1 - Application Security|4.1 - Application Security]] — p.62
- [ ] [[4.2 - Asset Management|4.2 - Asset Management]] — p.63
- [ ] [[4.3 - Vulnerability Scanning|4.3 - Vulnerability Scanning]] — p.64
- [ ] [[4.3 - Threat Intelligence|4.3 - Threat Intelligence]] — p.65
- [ ] [[4.3 - Penetration Testing|4.3 - Penetration Testing]] — p.65-66
- [ ] [[4.3 - Analyzing Vulnerabilities|4.3 - Analyzing Vulnerabilities]] — p.66
- [ ] [[4.3 - Vulnerability Remediation|4.3 - Vulnerability Remediation]] — p.67
- [ ] [[4.4 - Security Monitoring|4.4 - Security Monitoring]] — p.68
- [ ] [[4.4 - Security Tools|4.4 - Security Tools]] — p.69
- [ ] [[4.5 - Firewalls|4.5 - Firewalls]] — p.70
- [ ] [[4.5 - Web Filtering|4.5 - Web Filtering]] — p.71
- [ ] [[4.5 - Operating System Security|4.5 - Operating System Security]] — p.72
- [ ] [[4.5 - Secure Protocols|4.5 - Secure Protocols]] — p.72
- [ ] [[4.5 - Email Security|4.5 - Email Security]] — p.73
- [ ] [[4.5 - Monitoring Data|4.5 - Monitoring Data]] — p.73
- [ ] [[4.5 - Endpoint Security|4.5 - Endpoint Security]] — p.74
- [ ] [[4.6 - Identity and Access Management|4.6 - Identity and Access Management]] — p.75
- [ ] [[4.6 - Access Controls|4.6 - Access Controls]] — p.77
- [ ] [[4.6 - Multifactor Authentication|4.6 - Multifactor Authentication]] — p.78
- [ ] [[4.6 - Password Security|4.6 - Password Security]] — p.78
- [ ] [[4.7 - Scripting and Automation|4.7 - Scripting and Automation]] — p.79
- [ ] [[4.8 - Incident Response|4.8 - Incident Response]] — p.80
- [ ] [[4.8 - Incident Planning|4.8 - Incident Planning]] — p.81
- [ ] [[4.8 - Digital Forensics|4.8 - Digital Forensics]] — p.82
- [ ] [[4.9 - Log Data|4.9 - Log Data]] — p.83

## 5.0 - Governance, Risk, and Compliance (p.84)
[[5.0 - Governance, Risk, and Compliance|→ Domain overview]]

- [ ] [[5.1 - Security Policies|5.1 - Security Policies]] — p.84
- [ ] [[5.1 - Security Standards|5.1 - Security Standards]] — p.85
- [ ] [[5.1 - Security Procedures|5.1 - Security Procedures]] — p.86
- [ ] [[5.1 - Security Considerations|5.1 - Security Considerations]] — p.87
- [ ] [[5.1 - Data Roles and Responsibilities|5.1 - Data Roles and Responsibilities]] — p.87
- [ ] [[5.2 - Risk Management|5.2 - Risk Management]] — p.88
- [ ] [[5.2 - Risk Analysis|5.2 - Risk Analysis]] — p.88
- [ ] [[5.2 - Risk Management Strategies|5.2 - Risk Management Strategies]] — p.89
- [ ] [[5.2 - Business Impact Analysis|5.2 - Business Impact Analysis]] — p.89
- [ ] [[5.3 - Third-party Risk Assessment|5.3 - Third-party Risk Assessment]] — p.90
- [ ] [[5.3 - Agreement Types|5.3 - Agreement Types]] — p.91
- [ ] [[5.4 - Compliance|5.4 - Compliance]] — p.92
- [ ] [[5.4 - Privacy|5.4 - Privacy]] — p.93
- [ ] [[5.5 - Audits and Assessments|5.5 - Audits and Assessments]] — p.93
- [ ] [[5.5 - Penetration Tests|5.5 - Penetration Tests]] — p.94
- [ ] [[5.6 - Security Awareness|5.6 - Security Awareness]] — p.95
- [ ] [[5.6 - User Training|5.6 - User Training]] — p.96

---
[[Home|← Home]]  |  [[00 - CompTIA Objectives Summary|Objectives Summary →]]
