### Study Categories
- ⚡ Ports & Protocols
- 🧠 Identity Stack
- 🔐 Encryption Stack
- 🛡️ Detection Stack
- 📊 Risk & Governance


- `IAM` — Identity and Access Management <sub>controls identities and permissions | 🧠</sub>
  - `AAA` — Authentication, Authorization, Accounting <sub>verify, allow, log | 🧠</sub>
  - `MFA` — Multifactor Authentication <sub>2+ factors: know / have / are | 🧠</sub>
  - `SSO` — Single Sign-on <sub>one login for many systems | 🧠</sub>
  - `802.1X` — Network Access Control <sub>port-based authentication | 🧠</sub>
    - `EAP` — Extensible Authentication Protocol <sub>authentication framework | 🧠</sub>
      - `PEAP` — Protected EAP <sub>tunnels authentication inside TLS | 🧠</sub>
      - `EAP-TLS` — Extensible Authentication Protocol-Transport Layer Security <sub>certificate-based auth, very secure | 🧠🔐</sub>
  - `RADIUS` (UDP/1812, 1813) — Remote Authentication Dial-in User Service <sub>centralized AAA, common for network auth | 🧠⚡</sub>
  - `TACACS+` (TCP/49) — Terminal Access Controller Access Control System <sub>AAA, encrypts the session, often Cisco-focused | 🧠⚡</sub>
  - `LDAP` (TCP/389, 636) — Lightweight Directory Access Protocol <sub>directory services, users and groups | 🧠⚡</sub>
  - `Kerberos` — network authentication protocol <sub>ticket-based authentication | 🧠</sub>
    - `KDC` — Key Distribution Center <sub>issues Kerberos tickets</sub>
    - `TGT` — Ticket Granting Ticket <sub>initial ticket used to request service tickets</sub>

- `PKI` — Public Key Infrastructure <sub>manages certificates and trust | 🔐</sub>
  - `CA` — Certificate Authority <sub>trusted issuer of certificates | 🔐</sub>
  - `RA` — Registration Authority <sub>verifies identity before issuance | 🔐</sub>
  - `CSR` — Certificate Signing Request <sub>request sent to obtain a certificate | 🔐</sub>
  - `CRL` — Certificate Revocation List <sub>list of revoked certificates | 🔐</sub>
  - `OCSP` — Online Certificate Status Protocol <sub>real-time certificate status checking, often over HTTP/HTTPS | 🔐</sub>
  - `TLS` (TCP/443) — Transport Layer Security <sub>secure communication, replaces SSL | 🔐⚡</sub>
  - `SSL` — Secure Sockets Layer <sub>deprecated predecessor to TLS | 🔐</sub>
  - `RSA` — Rivest, Shamir, & Adleman <sub>asymmetric cryptography | 🔐</sub>
  - `AES` — Advanced Encryption Standard <sub>symmetric encryption, fast and widely used | 🔐</sub>
  - `ECC` — Elliptic-curve Cryptography <sub>strong security with smaller keys | 🔐</sub>
  - `DHE` — Diffie-Hellman Ephemeral <sub>ephemeral key exchange | 🔐</sub>
  - `ECDHE` — Elliptic-curve Diffie-Hellman Ephemeral <sub>ephemeral EC key exchange | 🔐</sub>
  - `PFS` — Perfect Forward Secrecy <sub>compromise of one key does not expose past sessions | 🔐</sub>

- `TCP/IP` — Transmission Control Protocol/Internet Protocol <sub>networking foundation | ⚡</sub>
  - `TCP` — Transmission Control Protocol <sub>reliable, connection-oriented | ⚡</sub>
  - `UDP` — User Datagram Protocol <sub>fast, connectionless | ⚡</sub>
  - `IP` — Internet Protocol <sub>addressing and routing | ⚡</sub>

  - `HTTP` (TCP/80) — Hypertext Transfer Protocol <sub>web traffic, unencrypted | ⚡</sub>
  - `HTTPS` (TCP/443) — Hypertext Transfer Protocol Secure <sub>web over TLS | ⚡🔐</sub>
  - `DNS` (TCP/UDP 53) — Domain Name System <sub>resolves names to IPs | ⚡</sub>
  - `SSH` (TCP/22) — Secure Shell <sub>secure remote login and tunneling | ⚡</sub>
  - `FTP` (TCP/21 control, TCP/20 data) — File Transfer Protocol <sub>insecure file transfer | ⚡</sub>
  - `SFTP` (TCP/22) — SSH File Transfer Protocol <sub>secure file transfer over SSH | ⚡</sub>
  - `Telnet` (TCP/23) — remote terminal access <sub>insecure plaintext remote access | ⚡</sub>
  - `SMTP` (TCP/25) — Simple Mail Transfer Protocol <sub>email sending | ⚡</sub>
    - `SMTPS` (TCP/465) — Simple Mail Transfer Protocol Secure <sub>encrypted SMTP</sub>
    - `Submission` (TCP/587) — authenticated email submission <sub>client mail send</sub>
  - `DHCP` (UDP/67, 68) — Dynamic Host Configuration Protocol <sub>dynamic IP assignment | ⚡</sub>
  - `SNMP` (UDP/161, 162) — Simple Network Management Protocol <sub>network monitoring and traps | ⚡</sub>
  - `NTP` (UDP/123) — Network Time Protocol <sub>time synchronization | ⚡</sub>
  - `SMB` (TCP/445) — Server Message Block <sub>file and printer sharing | ⚡</sub>
  - `RDP` (TCP/3389) — Remote Desktop Protocol <sub>remote GUI access | ⚡</sub>
  - `SIP` (TCP/UDP 5060, TLS 5061) — Session Initiation Protocol <sub>VoIP signaling | ⚡</sub>

- `WPA2/WPA3` — Wi-Fi Protected Access <sub>wireless security protocols | 🔐</sub>
  - `CCMP` — Counter-Mode/CBC-MAC Protocol <sub>AES-based wireless encryption | 🔐</sub>
  - `TKIP` — Temporal Key Integrity Protocol <sub>legacy wireless protection, deprecated | 🔐</sub>
  - `SAE` — Simultaneous Authentication of Equals <sub>WPA3 authentication | 🔐</sub>
  - `802.11` — Wi-Fi standard <sub>wireless LAN standard family</sub>
  - `SSID` — Service Set Identifier <sub>wireless network name</sub>
    - `BSSID` — Basic Service Set Identifier <sub>specific AP MAC identifier</sub>
    - `ESSID` — Extended Service Set Identifier <sub>extended wireless network identifier</sub>
  - `WPS` — WiFi Protected Setup <sub>easy setup, insecure in practice</sub>

- `VPN` — Virtual Private Network <sub>secure tunnel over untrusted networks | 🔐</sub>
  - `IPSec` — Internet Protocol Security <sub>network-layer security suite | 🔐</sub>
    - `AH` — Authentication Header <sub>integrity/authentication only, no encryption</sub>
    - `ESP` — Encapsulating Security Payload <sub>encryption plus integrity</sub>
    - `IKE` (UDP/500) — Internet Key Exchange <sub>negotiates security associations and keys</sub>
  - `SSL VPN` — Secure Sockets Layer VPN <sub>TLS-based remote access VPN, often TCP/443 | 🔐</sub>
  - `NAT` — Network Address Translation <sub>private to public translation</sub>
    - `PAT` — Port Address Translation <sub>many internal hosts share one public IP</sub>
    - `DNAT` — Destination Network Address Translation <sub>rewrites destination address</sub>

- `IDS` — Intrusion Detection System <sub>alerts on suspicious activity, does not block | 🛡️</sub>
  - `NIDS` — Network-based Intrusion Detection System <sub>monitors network traffic | 🛡️</sub>
  - `HIDS` — Host-based Intrusion Detection System <sub>monitors an endpoint/host | 🛡️</sub>
- `IPS` — Intrusion Prevention System <sub>detects and blocks malicious activity | 🛡️</sub>
  - `NIPS` — Network-based Intrusion Prevention System <sub>inline network blocking | 🛡️</sub>
  - `HIPS` — Host-based Intrusion Prevention System <sub>host-level blocking | 🛡️</sub>
- `SIEM` — Security Information and Event Management <sub>centralized logging, correlation, analysis | 🛡️</sub>
- `SOAR` — Security Orchestration, Automation, Response <sub>automated security workflows and response | 🛡️</sub>
- `EDR` — Endpoint Detection and Response <sub>endpoint telemetry, detection, containment | 🛡️</sub>
- `DLP` — Data Loss Prevention <sub>prevents sensitive data exfiltration | 🛡️📊</sub>
- `FIM` — File Integrity Monitoring <sub>detects unauthorized file changes | 🛡️</sub>
- `AV` — Antivirus <sub>malware detection and prevention | 🛡️</sub>
- `IoC` — Indicators of Compromise <sub>evidence/signs of malicious activity | 🛡️</sub>
- `IR` — Incident Response <sub>process for handling security incidents | 🛡️</sub>
  - `IRP` — Incident Response Plan <sub>documented incident procedures</sub>
  - `CERT` — Computer Emergency Response Team <sub>incident response team</sub>
  - `CSIRT` — Computer Security Incident Response Team <sub>security-focused response team</sub>

- `OWASP` — Open Web Application Security Project <sub>publishes web app guidance like Top 10 | 📊</sub>
  - `XSS` — Cross-site Scripting <sub>injects malicious scripts into web content</sub>
  - `SQLi` — SQL Injection <sub>injects malicious SQL into application input</sub>
  - `CSRF` — Cross-Site Request Forgery <sub>tricks authenticated users into unintended actions</sub>
  - `API` — Application Programming Interface <sub>application-to-application interface</sub>
  - `REST` — Representational State Transfer <sub>lightweight web service architecture</sub>
  - `SOAP` — Simple Object Access Protocol <sub>XML-based web service protocol</sub>

- `NIST` — National Institute of Standards & Technology <sub>frameworks, controls, guidance | 📊</sub>
- `CIS` — Center for Internet Security <sub>benchmarks and controls | 📊</sub>
- `GDPR` — General Data Protection Regulation <sub>EU privacy law | 📊</sub>
- `PCI DSS` — Payment Card Industry Data Security Standard <sub>cardholder data security standard | 📊</sub>
- `PII` — Personally Identifiable Information <sub>personal identifying data | 📊</sub>
- `PHI` — Personal Health Information <sub>health-related sensitive data | 📊</sub>

- `BCP` — Business Continuity Planning <sub>keeping business operations running | 📊</sub>
- `DRP` — Disaster Recovery Plan <sub>restoring systems after disruption | 📊</sub>
- `RTO` — Recovery Time Objective <sub>maximum acceptable downtime | 📊</sub>
- `RPO` — Recovery Point Objective <sub>maximum acceptable data loss | 📊</sub>

- `SLE` — Single Loss Expectancy <sub>loss from one incident | 📊</sub>
- `ARO` — Annualized Rate of Occurrence <sub>expected frequency per year | 📊</sub>
- `ALE` — Annualized Loss Expectancy <sub>SLE × ARO | 📊</sub>

- `XaaS` — Anything as a Service <sub>umbrella term for cloud delivery models</sub>
  - `SaaS` — Software as a Service <sub>provider hosts application</sub>
  - `PaaS` — Platform as a Service <sub>provider hosts platform/runtime</sub>
  - `IaaS` — Infrastructure as a Service <sub>provider hosts compute/network/storage</sub>
- `CASB` — Cloud Access Security Broker <sub>policy enforcement between users and cloud services</sub>
- `CSP` — Cloud Service Provider <sub>cloud vendor/provider</sub>
- `VM` — Virtual Machine <sub>software-defined computer</sub>
- `VPC` — Virtual Private Cloud <sub>isolated cloud network</sub>

- `AES` — Advanced Encryption Standard <sub>symmetric encryption standard | 🔐</sub>
- `DES` — Data Encryption Standard <sub>legacy symmetric encryption, insecure | 🔐</sub>
- `3DES` — Triple Data Encryption Standard <sub>legacy DES variant, deprecated | 🔐</sub>
- `SHA` — Secure Hashing Algorithm <sub>hashing for integrity | 🔐</sub>
- `MD5` — Message Digest 5 <sub>broken hash algorithm, collision-prone | 🔐</sub>
- `HMAC` — Hash-based Message Authentication Code <sub>integrity and authenticity using a shared secret | 🔐</sub>
- `PBKDF2` — Password-based Key Derivation Function 2 <sub>slow password hashing / key stretching | 🔐</sub>
- `IV` — Initialization Vector <sub>adds randomness to encryption operations | 🔐</sub>

- `TPM` — Trusted Platform Module <sub>hardware chip for secure key storage and platform trust | 🔐</sub>
- `HSM` — Hardware Security Module <sub>enterprise hardware cryptographic device | 🔐</sub>
- `FDE` — Full Disk Encryption <sub>encrypts an entire disk | 🔐</sub>
- `BIOS` — Basic Input/Output System <sub>legacy firmware interface</sub>
- `UEFI` — Unified Extensible Firmware Interface <sub>modern firmware interface</sub>
- `Secure Boot` — boot security feature <sub>prevents unauthorized boot code from loading</sub>
- `ASLR` — Address Space Layout Randomization <sub>memory layout randomization defense</sub>
- `DEP` — Data Execution Prevention <sub>prevents execution in non-executable memory</sub>