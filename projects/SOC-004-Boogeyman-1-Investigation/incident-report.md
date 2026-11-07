# SOC-004 — Incident report

## Case overview
TryHackMe Boogeyman 1

## Executive summary
An invoice-themed ZIP email was correlated with PowerShell telemetry and HTTP GET responses delivering /update and /sb.exe from files.bpakcaging.xyz. Script text referenced a KeePass database and outbound transfer mechanisms.

## Investigation methods
Thunderbird, email/MIME analysis, evidence hashing, PowerShell Event ID 4104, Wireshark HTTP stream reconstruction, IOC tracking

## Findings
An invoice-themed ZIP email was correlated with PowerShell telemetry and HTTP GET responses delivering /update and /sb.exe from files.bpakcaging.xyz. Script text referenced a KeePass database and outbound transfer mechanisms.

## Verdict
High-confidence malicious activity; successful data exfiltration remains unconfirmed.

## Recommended actions
Preserve telemetry; correlate additional host and network evidence; escalate and contain if validated.

## Limitations
Simulated environment; only evidence-supported conclusions are stated.
