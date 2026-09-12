# SOC-INC-001 — RDP Brute Force

## Incident
Multiple Failed RDP Login Attempts

## Severity
Medium

## Source
Kali Linux — 192.168.249.129

## Target
Windows 11 SOC Endpoint — 192.168.249.128

## Detection
Windows Security Event ID 4625 was observed in Splunk.

A controlled Hydra test generated multiple failed RDP
authentication attempts against the Windows endpoint.

## Investigation
Splunk was used to correlate the failed authentication events
with the source IP address of the Kali Linux test machine.

11 failed remote login events were observed during the investigation.

## Verdict
Brute Force Confirmed

## Response
- Preserve authentication evidence
- Identify source IP
- Review related authentication activity
- Escalate to SOC L2 for further investigation

## Lab Note
This activity was intentionally generated inside an isolated
SOC home lab for detection and investigation practice.
