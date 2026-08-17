# 🛡️ Cybersecurity Labs

Welcome to my Cybersecurity Lab Repository.

This repository contains my practical cybersecurity lab reports, technical evidence, security testing activities, findings, and recommendations. The labs were performed in controlled laboratory environments using Windows, Linux, SIEM, endpoint security, Active Directory, and Kerberos technologies.

---

## 👩‍💻 Student Information

**Name:** Shumaila Arif

**Field:**  Cybersecurity

**Repository:** Cybersecurity Practical Labs

---

# 📚 Labs Included

This repository contains the following three cybersecurity practical reports:

1. **Lab 2 — SIEM Deployment & Real-Time Log Analysis**
2. **Lab 3 — Endpoint Detection & Response Verification**
3. **Active Directory & Kerberos Security Assessment**

---

# 🔹 Lab 2 — SIEM Deployment & Real-Time Log Analysis

## 🎯 Objective

The purpose of this lab was to deploy a Wazuh SIEM environment and verify security monitoring, authentication-event detection, threat hunting, and automated response.

## 🏗️ Lab Environment

The lab used:

- Ubuntu Linux — Wazuh Manager
- Wazuh Indexer
- Windows VM — Wazuh Agent
- Private virtual network
- Wazuh Dashboard

The Windows endpoint was configured to communicate with the Wazuh Manager at:

```text
Wazuh Manager: 192.168.56.20
Windows Endpoint: 192.168.56.10
