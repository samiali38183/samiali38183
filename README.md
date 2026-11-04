# Sami Ali

**Security engineering student building detection and vulnerability-management tooling.** Looking for Security Engineer / Detection & Response internships, Summer 2027.

Cybersecurity student in Northern Virginia (graduating May 2028) · CompTIA Security+ · AWS Certified Cloud Practitioner · former DHS/CBP Vulnerability Assessment Team intern (Nessus/Tenable, CISA KEV, BOD 26-04) · Public Trust.

Portfolio: [samiali38183.github.io](https://samiali38183.github.io) · LinkedIn: [sami-ali-1a4b89345](https://www.linkedin.com/in/sami-ali-1a4b89345)

<!-- TODO(flagship): add the detection-engineering project here as the first entry once the repo is public. Keep the same shape: what it does / tech / one verified metric. -->

## Projects

**[sinkline](https://github.com/samiali38183/sinkline)** — interprocedural taint analysis for Python web apps, mapped to the OWASP Top 10.
Abstract interpreter over `ast` with two-pass function summaries, CWE-scoped sanitizers and validation-guard recognition; emits SARIF for GitHub code scanning. Zero dependencies, 138 sink signatures / 42 rules. On a 109-line labeled corpus: precision 0.983 / recall 0.951 (bandit on the same corpus: F1 0.579); 0 findings on microblog, SQLi flows found across files in vulpy. Python · static analysis · SARIF · GitHub Actions CI on 3 OSes.

**[kev-risk-prioritization](https://github.com/samiali38183/kev-risk-prioritization)** — risk-based vulnerability prioritization with CISA KEV, EPSS, CVSS and asset criticality, aligned with BOD 26-04.
Case study of the methodology from my CBP internship plus a stdlib-only reference implementation that ranks findings, compares KEV vs non-KEV populations and matches against the live KEV feed. Synthetic data only; no internship figures. Python · vulnerability management · CISA KEV / EPSS / CVSS.

**[call-kettle](https://github.com/samiali38183/call-kettle)** — sanitized snapshot of a production AI voice receptionist (FastAPI, Twilio, Claude tool-use).
Security-relevant parts: Twilio request-signature validation on every webhook, server-side enforcement of booking rules the model cannot bypass, strict Pydantic config (`extra: forbid`), tenant isolation tests, cost guards. 1,100+ pytest test functions gate every change in CI. Python 3.12 · FastAPI · SQLite · Twilio.

**[cybersecurity-vault](https://github.com/samiali38183/cybersecurity-vault)** — defensive labs and small tools.
Phishing IOC Extractor (stdlib `.eml` parser → deduplicated JSON of IPs, domains, URLs, emails, hashes; 10 pytest tests) and a Wireshark lab covering TCP/DNS/HTTP/TLS-SNI/ARP with ATT&CK mapping (T1557.002). Python · packet analysis · threat intel.

## Skills

- **Vulnerability management** — Nessus/Tenable, CISA KEV, EPSS, CVSS v3.1, BOD 26-04, remediation benchmarking, NIST CSF / FedRAMP context
- **Detection & analysis** — Wireshark, IOC extraction, MITRE ATT&CK mapping, log/packet triage
- **AppSec & static analysis** — taint analysis, OWASP Top 10 / CWE, SARIF, secure-by-default input validation
- **Python** — stdlib-first CLIs, `ast`, pytest, argparse, type hints, GitHub Actions
- **Cloud / AWS** — IAM, EC2, S3, VPC, CloudTrail fundamentals (Cloud Practitioner certified)

## Certifications

CompTIA Security+ · AWS Certified Cloud Practitioner
