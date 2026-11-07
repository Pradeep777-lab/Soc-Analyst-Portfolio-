# SOC Analyst Portfolio | Pradeep B.

**Junior SOC Analyst / Cybersecurity Analyst candidate**  
Master of Science in Computer Science, Campbellsville University (May 2024) | TryHackMe SOC Level 1 learning path completed

## About this portfolio
I investigate simulated security incidents using a structured SOC workflow: alert triage, evidence collection, SIEM searches, endpoint and network correlation, indicator documentation, and clear incident reporting. These are **hands-on labs, not professional employment**.

## Featured investigations

| ID | Project | Focus |
|---|---|---|
| [SOC-001](projects/SOC-001-Phishing-Email-Analysis/) | Phishing Email Analysis | Email triage |
| [SOC-002](projects/SOC-002-PS-Eclipse-Endpoint-Investigation/) | PS Eclipse — Splunk Endpoint Threat Investigation | Splunk searches |
| [SOC-003](projects/SOC-003-NeuralNexus-PowerShell-Investigation/) | NeuralNexus — Suspicious PowerShell Investigation | High-severity alert triage |
| [SOC-004](projects/SOC-004-Boogeyman-1-Investigation/) | Boogeyman 1 — Phishing, PowerShell and Network Investigation | Thunderbird |

## Technical skills
**Security operations:** Alert triage, incident response fundamentals, incident documentation, IOC analysis, threat hunting, escalation, log review.  
**SIEM and telemetry:** Splunk SPL, Microsoft Sentinel (training exposure), Windows Sysmon, Windows Event Logs, PowerShell Script Block Logging.  
**Network and email:** Wireshark, packet capture analysis, HTTP streams, DNS, Thunderbird, email header and authentication analysis.  
**Supporting tools:** CyberChef, TryHackMe SOC Simulator, Linux CLI, jq, file hashing.

## Case-study workflow
1. **Triage:** Identify the alert or reported anomaly and record the initial scope.
2. **Collect:** Preserve relevant screenshots, timestamps, process details, logs and network indicators.
3. **Correlate:** Reconstruct activity using Splunk, Sysmon, PowerShell, email, or packet telemetry.
4. **Assess:** Separate confirmed observations from suspected attacker behavior and unknown outcomes.
5. **Report:** Document evidence, verdict, limitations and next investigative actions.

## Repository navigation
Each case folder includes an overview, technical incident report, evidence index, and IOC register. The `career-documents/` folder contains four Word summaries, an ATS-oriented resume, and a customizable cover letter.

## How I assess findings
I separate **observed telemetry**, **analyst inference**, and **unverified outcomes**. A benign file reputation does not clear a suspicious process chain; a script containing exfiltration commands does not by itself prove successful data transfer.

## Education and professional development
Master of Science in Computer Science — Campbellsville University, May 2024. Coursework included disaster recovery and technical reporting. Completed the TryHackMe SOC Level 1 path and documented practical exercises in incident triage and analysis.

## Contact
- Location: Cincinnati, Ohio
- LinkedIn: https://www.linkedin.com/in/pradeep-b-3285b8322/
- Email: pradeep0919191@gmail.com
- Phone: 513-606-2454
- GitHub: Add your profile URL after creating the repository.

## Disclaimer
All investigations are from controlled TryHackMe lab scenarios. Screenshots are for educational portfolio demonstration. No employer affiliation or production security incident experience is implied.
