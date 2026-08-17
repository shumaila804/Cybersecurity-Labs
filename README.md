# 🛡️ Cybersecurity Labs

This repository contains my cybersecurity practical lab reports and security assessment work performed in controlled laboratory environments.

## 📚 Lab Reports

### 🔹 Lab 2 — SIEM Deployment & Real-Time Log Analysis

**Tools:** Wazuh SIEM, Ubuntu, Windows, Wazuh Agent, Threat Hunting, MITRE ATT&CK

This lab focused on deploying Wazuh SIEM and monitoring authentication activity.

**Activities performed:**
- Deployed Wazuh Manager and Indexer
- Configured Windows Wazuh Agent
- Verified connectivity between Windows and Wazuh Manager
- Registered the Windows endpoint with Wazuh
- Monitored authentication failures
- Performed Threat Hunting
- Analyzed suspicious SSH authentication activity
- Observed MITRE ATT&CK classifications
- Tested Wazuh Active Response
- Verified firewall-drop response

**Result:**  
The lab demonstrated the complete security monitoring workflow:

`Log Collection → Detection → Threat Hunting → Alert → Active Response`

📄 **Report:** `Lab_2_Report.docx`

---

### 🔹 Lab 3 — Endpoint Detection & Response Verification

**Tools:** Atomic Red Team, Microsoft Defender, PowerShell, Windows Event Logs

This lab focused on verifying endpoint security controls against simulated adversary behavior.

**Activities performed:**
- Verified the Invoke-AtomicRedTeam PowerShell module
- Inspected MITRE ATT&CK T1059 Command and Scripting Interpreter
- Inspected T1059.001 PowerShell
- Verified Microsoft Defender Antivirus
- Verified Real-Time Protection and AMSI
- Observed Microsoft Defender threat detections
- Analyzed PowerShell ScriptBlock logging
- Reviewed Windows Security events
- Reviewed Microsoft Defender Operational logs
- Verified blocked/detected PowerShell activity

**Important Evidence:**
- PowerShell Event ID `4104`
- Windows Security Events `4624`, `4634`, `4672`
- Microsoft Defender Events `1116` and `1117`
- T1059 and T1059.001 activity
- Access Denied result during the PowerShell XML-request test

**Result:**  
The lab demonstrated endpoint visibility through Microsoft Defender and Windows logging, including detection and prevention of simulated activity.

📄 **Report:** `Lab_3_Endpoint_Detection_Report.docx`

---

### 🔹 Active Directory & Kerberos Security Assessment

**Environment:** SOORTY.LOCAL Laboratory Environment

**Tools:** Kali Linux, Windows Server 2025, Nmap, Active Directory, Kerberos, SMB, RPC

This lab focused on assessing a controlled Active Directory and Kerberos environment.

**Activities performed:**
- Verified connectivity to the Domain Controller
- Verified DNS resolution
- Performed Nmap service discovery
- Enumerated Active Directory users and groups
- Performed RPC enumeration
- Enumerated SMB shares
- Accessed SYSVOL and Group Policy information
- Validated Kerberos authentication
- Obtained and verified a Kerberos TGT
- Created the `svc_web` service account
- Registered the HTTP SPN
- Verified `HTTP/web01.soorty.local`
- Validated Kerberos service-ticket acquisition
- Used `GetUserSPNs` for service-account assessment
- Reviewed Windows Security Events `4624` and `4625`

**Lab Environment:**

```text
Domain: SOORTY.LOCAL
Domain Controller: dc01.soorty.local
Domain Controller IP: 192.168.56.10
Server OS: Windows Server 2025
Assessment Host: Kali Linux
Lab User: labuser@SOORTY.LOCAL
Service Account: svc_web
HTTP SPN: HTTP/web01.soorty.local
