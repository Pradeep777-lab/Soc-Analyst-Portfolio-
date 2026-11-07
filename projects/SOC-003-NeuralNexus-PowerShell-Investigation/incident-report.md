# SOC-003 — Incident report

## Case overview
TryHackMe SOC Simulator

## Executive summary
Alert 6352 showed a suspicious child process. WINWORD.EXE opened Q3_PressKit_Feedback.docm and spawned encoded PowerShell; script-block logging captured a download-and-execute command retrieving svchost_update.ps1 from paylink-cdn.thm:8067 into TEMP and attempting hidden execution. The legitimate-looking ai.exe was 0/68 on VirusTotal, which does not clear the separate PowerShell activity.

## Investigation methods
High-severity alert triage, Splunk, Sysmon Event ID 1, PowerShell Event ID 4104, process-parent correlation, hash reputation checks

## Findings
Alert 6352 showed a suspicious child process. WINWORD.EXE opened Q3_PressKit_Feedback.docm and spawned encoded PowerShell; script-block logging captured a download-and-execute command retrieving svchost_update.ps1 from paylink-cdn.thm:8067 into TEMP and attempting hidden execution. The legitimate-looking ai.exe was 0/68 on VirusTotal, which does not clear the separate PowerShell activity.

## Verdict
Escalate suspicious downloader/stager behavior; successful second-stage execution remains unconfirmed.

## Recommended actions
Preserve telemetry; correlate additional host and network evidence; escalate and contain if validated.

## Limitations
Simulated environment; only evidence-supported conclusions are stated.
