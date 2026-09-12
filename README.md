# SOC-Home-Lab
# SOC Home Lab

A practical SOC Analyst L1 home lab built to practice security
monitoring, SIEM log analysis, threat detection and incident investigation.

## Lab Architecture

Kali Linux → Windows 11 → Sysmon / Windows Security / Windows Firewall → Splunk SIEM

## Environment

- Kali Linux — Attacker/Test Machine
- Windows 11 — SOC Endpoint
- Splunk Enterprise — SIEM
- Sysmon — Process and Network Telemetry
- Mailpit — Controlled Phishing Simulation

## Security Scenarios

### 1. RDP Brute Force Detection
Simulated multiple failed RDP login attempts from Kali Linux
and investigated Windows Security Event ID 4625 in Splunk.

### 2. Network Reconnaissance Detection
Performed controlled port scanning from Kali Linux and analyzed
Windows Firewall logs to identify multiple port access attempts.

### 3. Suspicious PowerShell Investigation
Generated a controlled PowerShell execution using
ExecutionPolicy Bypass and investigated the Sysmon Process Creation event.

### 4. Controlled Phishing Investigation
Delivered a simulated phishing email through a local Mailpit SMTP
environment and analyzed its headers, content and suspicious URL.

## SOC Investigation Workflow

Alert → Triage → Evidence Collection → Log Correlation
→ IOC Identification → Verdict → Response → Documentation

## Tools Used

- Splunk Enterprise
- Sysmon
- Kali Linux
- Windows 11
- Nmap
- Wireshark
- Windows Firewall
- Mailpit

## Skills Demonstrated

- SIEM Log Analysis
- Alert Triage
- Windows Event Analysis
- Network Security Monitoring
- IOC Identification
- Incident Investigation
- Detection Rule Creation
- SOC L1 Escalation

## Key Outcomes

The lab demonstrates practical SOC L1 activities including
security monitoring, alert investigation, log correlation,
threat detection and incident documentation.

## Disclaimer

All security testing in this project was performed in a
controlled home lab environment for educational purposes.
