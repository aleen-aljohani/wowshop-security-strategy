# WowShop — Enterprise Cybersecurity Strategy

A comprehensive, organization-wide **cybersecurity strategy** for *WowShop*, a fictional online retailer. Written from the perspective of the company's **CISO**, the strategy defines the assets to protect, analyzes threats, and maps concrete security controls to recognized frameworks — **NIST Cybersecurity Framework**, **NIST SP 800-53**, **CIS Controls v8**, and **ISO/IEC 27001 / 27005**.

> 🎓 Course project for **EMCS601 – Cyber Security Fundamentals**, Executive Master in Cyber Security, King Abdulaziz University (Fall 2025). Completed as a team project; published here with the team's consent. Teammates' names, contact details, and all student IDs have been removed for privacy.

📄 [Full Strategy Presentation (PDF)](WowShop_Cybersecurity_Strategy.pdf)

---

## The Organization

**WowShop** — a small online clothing retailer (~100 employees) running a hybrid-cloud environment: 3,000–10,000 daily visitors (up to 30,000 at peak), PCI-compliant payment gateways (PayPal, Apple Pay, Mada), cloud hosting, and logistics partners (Aramex, DHL). Key stakeholders span the Board, CTO, CISO/CSO, IT infrastructure, SOC, and GRC teams.

---

## Strategy Structure (NIST CSF Functions)

The strategy is organized around the core NIST Cybersecurity Framework functions:

### 🔎 Identify
- Classify all assets (devices, data, applications, cloud)
- Map critical business processes and establish cybersecurity governance
- Conduct regular risk assessments and evaluate third-party / vendor risk

### 🛡️ Protect
- Access controls: **MFA** and **RBAC**
- Encrypt data in transit and at rest (**TLS 1.3, AES-256**)
- Security awareness training, patch management, protective tooling (EDR, firewalls, DLP)

### 📡 Detect
- Continuous monitoring with **SIEM**
- Log analysis (firewall, IDS/IPS), anomaly detection, regular scans
- Defined alert levels and escalation paths

### 🚨 Respond & Recover
- Incident response procedures and disciplinary processes
- Business continuity & disaster recovery planning

---

## Risk Analysis

Key risks to WowShop's systems and customer data are identified, evaluated, and prioritized using a structured risk analysis aligned with **ISO 27005** and **NIST SP 800-30**, covering software, physical/infrastructure, and human-resource domains.

### Software Threats & Controls
Identified threats include **SQL Injection**, **XSS**, **CSRF**, weak/misused APIs, outdated third-party libraries, cloud misconfigurations, and weak session/authentication controls — mapped to NIST SP 800-53 controls (SI-10, AC-2, SC-7, RA-5, SI-2, CM-2) and CIS Controls v8 (2, 4, 5, 6, 8, 16).

### OS Hardening
**Windows Server 2022** hardened against misuse, misconfiguration, and undetected events using selected CIS Controls (inventory, secure configuration, account & access management, audit logging, application security).

### Physical & Infrastructure Security
Controls for office/warehouse, server room, workstations, network, hybrid cloud, and IoT devices — access cards, biometric access, environmental controls, full-disk encryption, firewall hardening, 24/7 monitoring, VLAN segmentation.

### HR Security (ISO 27001)
Controls across the employment lifecycle: identity & background checks and confidentiality agreements **before hiring**; awareness training and strict least-privilege access **during employment**; immediate deactivation, asset collection, and log review **at end of employment / role change**.

---

## Controls Categorization

Implemented controls are categorized as:

| Category | Examples |
|---|---|
| **Management** | Security policies, risk management plan, BCP/DR, security governance |
| **Operational** | Employee training, incident response, log review, physical security, backups |
| **Technical** | NGFW firewalls, IDS/IPS, encryption, MFA & RBAC, EDR, payment tokenization, network segmentation |

---

## Frameworks & Standards Referenced

`NIST Cybersecurity Framework` · `NIST SP 800-53` · `NIST SP 800-30` · `CIS Controls v8` · `ISO/IEC 27001` · `ISO/IEC 27005` · `PCI DSS`

## Skills & Concepts

`Security Strategy` · `Security Governance` · `Risk Assessment` · `Defense in Depth` · `OS Hardening` · `Access Control` · `SIEM / Monitoring` · `Physical Security` · `HR Security`
