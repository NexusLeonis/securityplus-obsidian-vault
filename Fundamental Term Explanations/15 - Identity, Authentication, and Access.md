# 15. Identity, Authentication, and Access

[[00 - Overview|← Overview]]

**Related Security+ material:** [[1.2 - Authentication, Authorization, and Accounting]] · [[4.6 - Identity and Access Management]] · [[4.6 - Access Controls]] · [[4.6 - Multifactor Authentication]]

| Term | Simple Explanation | Example | Security+ Why It Matters |
|---|---|---|---|
| **Identification** | Claiming an identity. | Entering a username. | A system must know which identity requests access. |
| [[1.2 - Authentication, Authorization, and Accounting\|Authentication]] | Proving that a claimed identity is genuine. | Entering the correct password. | Authentication prevents unauthorized users from logging in. |
| [[1.2 - Authentication, Authorization, and Accounting\|Authorization]] | Deciding what an authenticated identity may access or do. | A manager may approve timecards. | Authentication alone does not determine permissions. |
| [[1.2 - Authentication, Authorization, and Accounting\|Accounting]] | Recording user activity and resource use. | Logging login times and commands. | Accounting supports investigations and accountability. |
| **AAA** | Authentication, authorization, and accounting considered together. | RADIUS performs AAA for network access. | AAA forms the foundation of access control. |
| [[2.4 - Password Attacks\|Password]] | A secret string used to prove identity. | A user enters a unique passphrase. | Weak or reused passwords support account compromise. |
| **Passphrase** | A longer password made from multiple words or a memorable phrase. | River-Moon-Train-Glass. | Length usually improves resistance to guessing attacks. |
| **PIN** | A short numeric or alphanumeric secret, often tied to a specific device. | Phone unlock code. | PINs should have retry limits and device protections. |
| **Biometrics** | Authentication using physical or behavioral traits. | Fingerprint, face, or voice. | Biometrics cannot easily be changed after compromise. |
| **Token** | A physical or digital item used to prove identity or represent an authenticated session. | Hardware key or website session token. | Stolen tokens can allow access without a password. |
| **MFA** | Authentication using factors from at least two different categories. | Password plus hardware security key. | MFA reduces the value of stolen passwords. |
| **Something you know** | An authentication factor based on secret knowledge. | Password or PIN. | Attackers may steal or guess knowledge factors. |
| **Something you have** | An authentication factor based on possession. | Phone, smart card, or hardware token. | Theft or token duplication can defeat possession factors. |
| **Something you are** | An authentication factor based on physical characteristics. | Fingerprint or iris. | Biometric systems must prevent spoofing. |
| **Somewhere you are** | Context based on physical or network location. | Login allowed only from the office. | Location can strengthen risk-based decisions. |
| **Something you do** | A factor based on behavior. | Typing rhythm or touchscreen gestures. | Behavioral patterns can support continuous authentication. |
| **Single sign-on** | One login gives access to multiple related systems. | Signing into Microsoft 365 once. | SSO improves convenience but makes the central identity highly valuable. |
| **Federation** | Separate organizations trust one another’s identity systems. | A partner account accesses another company’s portal. | Federation reduces duplicate accounts but requires strong trust controls. |
| **Identity provider** | A system that authenticates users and provides identity information to other services. | Microsoft Entra ID authenticates a user. | Compromising the provider affects many connected applications. |
| **Service provider** | An application that relies on an identity provider for authentication. | A cloud application accepts the organization’s login. | It must correctly validate identity assertions and tokens. |
| **SAML** | A standard that sends signed identity assertions between an identity provider and a service provider. | Company credentials log a user into a cloud application. | SAML commonly supports enterprise web SSO. |
| **OAuth** | A framework that lets one application receive limited access without learning the user’s password. | A calendar app receives access to Google Calendar. | Stolen OAuth tokens can grant ongoing access. |
| **OpenID Connect** | An identity layer built on OAuth that lets applications verify who a user is. | “Sign in with Google.” | It supports modern authentication and SSO. |
| **Active Directory** | Microsoft’s directory service for centrally managing users, computers, groups, and policies. | Employees log into a Windows domain. | AD compromise can expose an entire organization. |
| **Domain** | A centrally managed collection of accounts, computers, and resources. | example.local. | Domain administrators hold broad authority. |
| **Domain controller** | A server that stores directory information and authenticates domain users. | A Windows server validates employee logins. | Domain controllers represent critical security assets. |
| **Organizational unit** | A container used to organize directory objects and apply policies. | Finance users and computers reside in one OU. | Incorrect OU placement may apply the wrong security settings. |
| **Security group** | A group used to assign access rights to multiple users at once. | The HR group receives access to HR files. | Group membership often determines authorization. |
| **Group Policy** | A Microsoft feature that centrally applies settings to users and computers. | Require screen locks on every workstation. | Group Policy enforces security controls at scale. |
| **Local account** | An account that exists only on one device. | A laptop’s local administrator. | Reused local passwords can support lateral movement. |
| **Service account** | An account used by an application or automated service. | A backup program accesses file shares. | Service accounts often have excessive rights and long-lived passwords. |
| **Privileged account** | An account with elevated access. | Domain administrator or database administrator. | These accounts require stronger protection and monitoring. |
| **Least privilege** | Give users and systems only the access required for their duties. | Help desk staff may reset passwords but not read payroll data. | It limits damage from compromise or mistakes. |
| **Separation of duties** | Divide sensitive tasks among multiple people. | One employee creates a payment and another approves it. | It prevents one person from controlling an entire process. |
| **Role-based access control** | Permissions depend on job roles. | Every HR specialist receives the HR role. | It simplifies consistent permission management. |
| **Attribute-based access control** | Access decisions use characteristics of the user, resource, action, and environment. | Allow doctors to view assigned patients during work hours. | It supports detailed, context-aware policies. |
| **Mandatory access control** | A central authority assigns security labels that users cannot change. | Classified documents require matching clearances. | It provides strict control in high-security environments. |
| **Discretionary access control** | Resource owners decide who may access their resources. | A file owner shares a folder with another user. | Owners may accidentally grant excessive access. |
| [[1.2 - Zero Trust\|Zero trust]] | A security model that continually verifies users, devices, and requests instead of trusting network location. | An internal user still needs device checks and authorization. | It reduces reliance on the traditional trusted internal network. |
| **Conditional access** | Access rules evaluate conditions such as user, device, location, and risk. | Require MFA when a login comes from another country. | It adds context to authentication decisions. |
| **Session** | The temporary authenticated interaction between a user and a system. | A website keeps you logged in after authentication. | Session theft can bypass the original login. |
| **Session timeout** | A rule that ends a session after inactivity or a set period. | A banking site logs out after ten minutes. | It reduces opportunities to abuse unattended sessions. |
| **Account lockout** | A control that disables login after too many failed attempts. | Five incorrect passwords lock the account. | It slows brute-force attacks but can enable denial of service. |
| **Password manager** | Software that securely stores and generates passwords. | A user creates unique passwords for every site. | It reduces password reuse and weak-password habits. |

---
[[00 - Overview|← Overview]]
