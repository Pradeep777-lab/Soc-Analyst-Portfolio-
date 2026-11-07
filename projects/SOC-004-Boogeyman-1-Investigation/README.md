# SOC-004 — Boogeyman 1 — Phishing, PowerShell and Network Investigation

**Platform:** TryHackMe Boogeyman 1  
**Type:** Simulated SOC investigation / hands-on lab  
**Status:** Documented; limitations disclosed

## Executive summary
An invoice-themed ZIP email was correlated with PowerShell telemetry and HTTP GET responses delivering /update and /sb.exe from files.bpakcaging.xyz. Script text referenced a KeePass database and outbound transfer mechanisms.

## Investigation objectives
- Triage the initial alert or reported security concern.
- Correlate source evidence and reconstruct the observable sequence.
- Distinguish confirmed facts from plausible but unverified impact.
- Produce an actionable analyst assessment and recommended next steps.

## Tools and technical skills
Thunderbird, email/MIME analysis, evidence hashing, PowerShell Event ID 4104, Wireshark HTTP stream reconstruction, IOC tracking.

## Evidence-based findings
An invoice-themed ZIP email was correlated with PowerShell telemetry and HTTP GET responses delivering /update and /sb.exe from files.bpakcaging.xyz. Script text referenced a KeePass database and outbound transfer mechanisms.

## Verdict
**High-confidence malicious activity; successful data exfiltration remains unconfirmed.**

## Analyst workflow
1. Establish the trigger, relevant endpoint or email, and time window.
2. Review primary source artifacts and preserve screenshots.
3. Correlate suspicious processes, scripts, URLs, and network activity.
4. Document indicators and note evidence gaps.
5. Recommend escalation, validation, containment, or monitoring as warranted.

## Deliverables
- [Investigation report](incident-report.md)
- [Evidence index](evidence/INDEX.md)
- [Indicator register](iocs.csv)
- [Word summary](../../career-documents/SOC-004-Investigation-Summary.docx)

> This project was completed in a training environment. Findings are limited to the evidence available; no production SOC experience is claimed.
