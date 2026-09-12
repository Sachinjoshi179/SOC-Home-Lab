# SOC-INC-002 — Controlled Phishing Email

## Incident
Suspicious Phishing Email

## Severity
High

## Detection
A controlled phishing email was delivered through the local
Mailpit SMTP environment.

## Email Indicators

Sender:
security-alert@micros0ft-security.example

Recipient:
socadmin@win-soc-01.example

Subject:
Urgent: Your account will be suspended

Suspicious URL:
https://microsoft-account-review.example/verify

## Investigation
The email headers and raw SMTP message were reviewed in Mailpit.

The sender used a look-alike domain/name and the message created
urgency by claiming that the account would be suspended.

## IOC
https://microsoft-account-review.example/verify

## Verdict
Phishing Confirmed

## Response
- Preserve email evidence
- Quarantine/delete the message
- Identify and block the suspicious IOC
- Search for related messages
- Escalate to SOC L2

## Lab Note
This was a controlled phishing simulation performed locally
using Mailpit. No real external phishing infrastructure was used.
