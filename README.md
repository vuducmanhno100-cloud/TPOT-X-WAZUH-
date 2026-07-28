# Honeypot Monitoring System with Wazuh

A Security Operations (SOC) lab that integrates an open-source Honeypot platform with Wazuh SIEM to collect, analyze and detect malicious activities from real-world attackers.

## Overview

This project aims to simulate a SOC monitoring environment by deploying a Honeypot exposed to the Internet and forwarding collected logs to Wazuh for security monitoring, alerting and attack analysis.

The system allows security analysts to observe attacker behaviors, extract Indicators of Compromise (IOCs), and evaluate the effectiveness of detection rules.

---

## Architecture

```
Internet Attacker
│
▼
T-Pot Honeypot (Cowrie, ...)
│
│ Log Events
▼
Wazuh Manager
│
├── Detection Rules
├── Log Analysis
├── IOC Extraction
▼
OpenSearch Dashboard
│
▼
Security Analyst
## Features

- Deploy Honeypot using the T-Pot platform
- Collect attack logs from real Internet attackers
- Centralize log management with Wazuh
- Build custom detection rules
- Detect SSH Brute Force attacks
- Detect Successful Login events
- Detect Command Execution after compromise
- Extract Indicators of Compromise (IP, Username, Password, Commands)
- Visualize alerts on Wazuh Dashboard
- Analyze attacker behaviors

---

## Technology Stack

| Category | Technologies |
|----------|--------------|
| SIEM | Wazuh |
| Honeypot | T-Pot, Cowrie |
| Container | Docker |
| OS | Ubuntu Linux |
| Virtualization | VMware |
| Dashboard | OpenSearch Dashboard |

---

## Detection Scenarios

Implemented detection rules include:

- SSH Brute Force
- Successful SSH Login
- Command Execution
- Suspicious Session Activity
- IOC Extraction
- Password Dictionary Analysis

---

## Log Analysis Workflow

1. Attacker connects to the Honeypot.
2. Honeypot records attacker activities.
3. Logs are forwarded to Wazuh.
4. Wazuh decodes and analyzes log events.
5. Detection Rules generate security alerts.
6. Security Analyst investigates alerts through the Dashboard.

---

## Project Outcomes

- Collected approximately **10,000+ security events per day**
- Captured real attacker payloads and commands
- Extracted Indicators of Compromise (IOC)
- Identified common brute-force usernames and passwords
- Improved detection capability through custom Wazuh rules
- Simulated SOC monitoring and incident investigation workflow

---

## Future Improvements

- Integrate Suricata IDS
- Threat Intelligence Integration
- Sigma Rule Conversion
- Automated IOC Enrichment
- Slack/Telegram Alert Notification
- MITRE ATT&CK Mapping
- Malware Sample Collection

---

## Skills Demonstrated

- Security Monitoring
- Log Analysis
- Detection Engineering
- SOC Operations
- Incident Detection
- Wazuh Rule Development
- Linux Administration
- Docker Deployment
- Threat Analysis

---

## Author

**Vũ Đức Mạnh**

Security Operations (Blue Team) | SOC Analyst Enthusiast
