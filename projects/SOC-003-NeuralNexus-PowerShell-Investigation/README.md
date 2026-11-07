# SOC-003 — NeuralNexus — Suspicious PowerShell Investigation

**Platform:** TryHackMe SOC Simulator  
**Type:** Simulated SOC investigation / hands-on lab  
**Status:** Documented; limitations disclosed

## Executive summary
Alert 6352 showed a suspicious child process. WINWORD.EXE opened Q3_PressKit_Feedback.docm and spawned encoded PowerShell; script-block logging captured a download-and-execute command retrieving svchost_update.ps1 from paylink-cdn.thm:8067 into TEMP and attempting hidden execution. The legitimate-looking ai.exe was 0/68 on VirusTotal, which does not clear the separate PowerShell activity.

## Investigation objectives
- Triage the initial alert or reported security concern.
- Correlate source evidence and reconstruct the observable sequence.
- Distinguish confirmed facts from plausible but unverified impact.
- Produce an actionable analyst assessment and recommended next steps.

## Tools and technical skills
High-severity alert triage, Splunk, Sysmon Event ID 1, PowerShell Event ID 4104, process-parent correlation, hash reputation checks.

## Evidence-based findings
Alert 6352 showed a suspicious child process. WINWORD.EXE opened Q3_PressKit_Feedback.docm and spawned encoded PowerShell; script-block logging captured a download-and-execute command retrieving svchost_update.ps1 from paylink-cdn.thm:8067 into TEMP and attempting hidden execution. The legitimate-looking ai.exe was 0/68 on VirusTotal, which does not clear the separate PowerShell activity.

## Verdict
**Escalate suspicious downloader/stager behavior; successful second-stage execution remains unconfirmed.**

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
- [Word summary](../../career-documents/SOC-003-Investigation-Summary.docx)

> This project was completed in a training environment. Findings are limited to the evidence available; no production SOC experience is claimed.
