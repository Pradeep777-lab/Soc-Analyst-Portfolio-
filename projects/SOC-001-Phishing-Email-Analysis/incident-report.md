# SOC-001 — Incident report

## Case overview
TryHackMe Phishing Analysis Fundamentals

## Executive summary
Two training emails were inspected. One presented a claimed sender/domain inconsistency; a second included suspicious links and a PDF requiring analysis. Authentication and tracking links were evaluated in context rather than treated as standalone proof of maliciousness.

## Investigation methods
Email triage, sender-domain comparison, raw headers, SPF/DKIM/DMARC interpretation, URL and PDF attachment examination

## Findings
Two training emails were inspected. One presented a claimed sender/domain inconsistency; a second included suspicious links and a PDF requiring analysis. Authentication and tracking links were evaluated in context rather than treated as standalone proof of maliciousness.

## Verdict
Suspicious indicators requiring review; no unsupported claim of confirmed compromise.

## Recommended actions
Preserve telemetry; correlate additional host and network evidence; escalate and contain if validated.

## Limitations
Simulated environment; only evidence-supported conclusions are stated.
