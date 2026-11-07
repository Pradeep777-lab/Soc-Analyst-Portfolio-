# SOC-002 — PS Eclipse — Splunk Endpoint Threat Investigation

**Platform:** TryHackMe PS Eclipse  
**Type:** Simulated SOC investigation / hands-on lab  
**Status:** Documented; limitations disclosed

## Executive summary
A simulated MSSP customer reported unusual file extensions on a Windows endpoint. Investigation followed endpoint process and network telemetry and examined a possible ransom note and associated script artifacts.

## Investigation objectives
- Triage the initial alert or reported security concern.
- Correlate source evidence and reconstruct the observable sequence.
- Distinguish confirmed facts from plausible but unverified impact.
- Produce an actionable analyst assessment and recommended next steps.

## Tools and technical skills
Splunk searches, Sysmon event correlation, suspicious binaries, downloads, privilege-related commands, network connections, ransomware hypothesis.

## Evidence-based findings
A simulated MSSP customer reported unusual file extensions on a Windows endpoint. Investigation followed endpoint process and network telemetry and examined a possible ransom note and associated script artifacts.

## Verdict
**Suspicious endpoint activity investigated; ransomware impact not independently verified from supplied material.**

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
- [Word summary](../../career-documents/SOC-002-Investigation-Summary.docx)

> This project was completed in a training environment. Findings are limited to the evidence available; no production SOC experience is claimed.
