# SOC-001 — Phishing Email Analysis

**Platform:** TryHackMe Phishing Analysis Fundamentals  
**Type:** Simulated SOC investigation / hands-on lab  
**Status:** Documented; limitations disclosed

## Executive summary
Two training emails were inspected. One presented a claimed sender/domain inconsistency; a second included suspicious links and a PDF requiring analysis. Authentication and tracking links were evaluated in context rather than treated as standalone proof of maliciousness.

## Investigation objectives
- Triage the initial alert or reported security concern.
- Correlate source evidence and reconstruct the observable sequence.
- Distinguish confirmed facts from plausible but unverified impact.
- Produce an actionable analyst assessment and recommended next steps.

## Tools and technical skills
Email triage, sender-domain comparison, raw headers, SPF/DKIM/DMARC interpretation, URL and PDF attachment examination.

## Evidence-based findings
Two training emails were inspected. One presented a claimed sender/domain inconsistency; a second included suspicious links and a PDF requiring analysis. Authentication and tracking links were evaluated in context rather than treated as standalone proof of maliciousness.

## Verdict
**Suspicious indicators requiring review; no unsupported claim of confirmed compromise.**

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
- [Word summary](../../career-documents/SOC-001-Investigation-Summary.docx)

> This project was completed in a training environment. Findings are limited to the evidence available; no production SOC experience is claimed.
