# Active Directory Security

<br>

## AD Machines Writeups

Complete domain compromise walkthroughs from initial access to Domain Administrator<br><br>

| Machine | Difficulty | Key Techniques | Writeup | Status |
|---------|------------|----------------|---------|--------|
| Support | Easy | SMB Access, Binary Analysis, XOR Decryption, LDAP Enumeration, Credentials, WinRM, RBCD Attack, S4U2Proxy, DCSync | [Read](https://github.com/achnouri/support_machine_writeup) | Completed |
| Eighteen | Easy | MSSQL Impersonation, Password Spraying, WinRM, Delegated Permissions Abuse, CreateChild Rights, BadSuccessor Attack, dMSA Creation | [Planned](#) | Completed |
| MonitorsFour | Easy | Virtual Host Discovery, IDOR (PHP Type Juggling), MD5 Cracking, Cacti RCE (CVE-2025-24367), Unauthenticated Docker API, Container Escape (CVE-2025-9074), Windows Host Access | [Planned](#) | In Progress |
| Active | Medium | SMB Enumeration, Kerberoasting, GPP | [Planned](#) | Pending |
| Resolute | Medium | LDAP Enumeration, Password Spraying | [Planned](#) | Pending |
| Sauna | Easy | AS-REP Roasting, DNS Admin Abuse | [Planned](#) | Pending |
| Blackfield | Hard | SMB Enumeration, AS-REP Roasting, DCSync, SeBackupPrivilege | [Planned](#) | Pending |
| Monteverde | Medium | Azure AD Connect, Password in SMB | [Planned](#) | Pending |
| Cascade | Medium | LDAP Enumeration, Kerberoasting, AD Recycle Bin | [Planned](#) | Pending |
| Absolute | Insane | Image Metadata Analysis, Kerberos, Domain Compromise | [Planned](#) | Pending |
| Analysis | Hard | LDAP Injection, DLL Hijacking, GPO Abuse | [Planned](#) | Pending |
| Bruno | Medium | AS-REP Roasting, DLL Hijacking, RBCD, Kerberos Relay | [Planned](#) | Pending |
| Certified | Medium | ACL Abuse, WriteOwner, Shadow Credentials, ADCS ESC9 | [Planned](#) | Pending |
| Cicada | Easy | Unauthenticated AD Enumeration, Password Spraying, SeBackupPrivilege | [Planned](#) | Pending |
| Escape | Medium | SMB Guest Access, AD CS (ESC1) | [Planned](#) | Pending |
| Flight | Hard | LFI, UNC Injection, NTLM Capture, SweetPotato | [Planned](#) | Pending |
| Intelligence | Medium | PDF Metadata Analysis, BloodHound, GMSA Password Abuse | [Planned](#) | Pending |
| Mantis | Hard | OrchardCMS Exploitation, MS14-068, Golden Ticket | [Planned](#) | Pending |
| Object | Hard | Jenkins, Command Injection, RPC Object Hijacking | [Planned](#) | Pending |
| Office | Hard | Joomla RCE (CVE-2023-23752), AS-REP Roasting, Pass-the-Hash | [Planned](#) | Pending |
| Overwatch | Medium | .NET Analysis, MSSQL, Service Exploitation | [Planned](#) | Pending |
| PingPong | Insane | Multi-Domain AD, Cross-Realm Trust Abuse, JEA Bypass, SUID Path Hijacking, RBCD, MSSQL S4U Abuse, DCSync| [Planned](#) | Pending |
| Timelapse | Easy | LAPS, RunasCS, DCSync | [Planned](#) | Pending |

---

<br><br>
## AD Attack Techniques Library

| Technique | MITRE ID | Writeup | Detection Mapping |
|-----------|----------|---------|-------------------|
| AS-REP Roasting | T1558.004 | [Planned](#) | Pending |
| Kerberoasting | T1558.003 | [Planned](#) | Pending |
| DCSync | T1003.006 | [Planned](#) | Pending |
| Golden Ticket | T1558.001 | [Planned](#) | Pending |
| Silver Ticket | T1558.002 | [Planned](#) | Pending |
| ACL Abuse (GenericAll) | T1098 | [Planned](#) | Pending |
| Resource-Based Constrained Delegation | T1558 | [Planned](#) | Pending |
| NTLM Relay | T1557.001 | [Planned](#) | Pending |
| Pass-the-Hash | T1550.002 | [Planned](#) | Pending |
| Overpass-the-Hash | T1550.002 | [Planned](#) | Pending |
| DCShadow | T1207 | [Planned](#) | Pending |
| AdminSDHolder Backdoor | T1098 | [Planned](#) | Pending |
| Skeleton Key | T1556.001 | [Planned](#) | Pending |

---

<br>

## Detection & Evasion

| Attack | Detection (Event IDs) | Evasion Technique | Writeup |
|--------|----------------------|-------------------|---------|
| Kerberoasting | 4769, 4662 | Target AES-only accounts | [Planned](#) |
| DCSync | 4662, 5136 | LSASS remote extraction | [Planned](#) |
| Golden Ticket | 4624, 4672 | Monitor krbtgt hash changes | [Planned](#) |
| AS-REP Roasting | 4768 | Disable RC4, enforce strong passwords | [Planned](#) |
| Pass-the-Hash | 4624 | Credential Guard, Protected Users group | [Planned](#) |
---

<br><br>

**Last Updated:** June 2026  
