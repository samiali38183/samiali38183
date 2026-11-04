# Sami Ali

Cybersecurity student at George Mason University (graduating May 2028), looking for Summer 2027
security engineering and detection internships. Previously interned on the DHS/CBP Vulnerability
Assessment Team, working with Nessus/Tenable data, CISA KEV and BOD 26-04.

CompTIA Security+ · AWS Certified Cloud Practitioner

Portfolio: [samiali38183.github.io](https://samiali38183.github.io) · LinkedIn: [sami-ali-1a4b89345](https://www.linkedin.com/in/sami-ali-1a4b89345)

## Projects

**[tripline](https://github.com/samiali38183/tripline)**: tests whether detections actually fire. It replays
recorded attack telemetry (Atomic Red Team on Linux, Stratus Red Team / flaws.cloud CloudTrail) through
Sigma rules in CI and fails the PR if an expected rule stops firing. Coverage is weighted by how common
each ATT&CK technique is. The first Linux run found a gap in a SigmaHQ setuid rule, which I fixed with a
custom rule. Python · Sigma · MITRE ATT&CK · GitHub Actions

**[sinkline](https://github.com/samiali38183/sinkline)**: a static analyzer that follows user input
through Python web apps and flags it when it reaches SQL, shell commands and other dangerous calls
unsanitized. Maps to OWASP Top 10 / CWE and outputs SARIF. On a 109-line labeled benchmark: precision
0.983, recall 0.951 (Bandit F1 on the same set: 0.579). Python · static analysis · SARIF

**[kev-risk-prioritization](https://github.com/samiali38183/kev-risk-prioritization)**: the vulnerability
prioritization approach from my CBP internship, rebuilt on synthetic data. Ranks findings by KEV status,
EPSS, CVSS and asset criticality, and can pull the live KEV catalog. Python · vulnerability management

**[call-kettle](https://github.com/samiali38183/call-kettle)**: an AI phone receptionist (FastAPI,
Twilio, Claude tool use). The security side: Twilio signature checks on every webhook, booking rules
enforced in code so the model can't bypass them, strict config validation, and tenant isolation tests.

**[cybersecurity-vault](https://github.com/samiali38183/cybersecurity-vault)**: labs and small tools,
including a phishing IOC extractor (parses .eml files into IPs, domains, URLs, emails and hashes; 10
pytest tests) and a Wireshark lab covering TCP, DNS, HTTP, TLS SNI and ARP.

## Skills

- Vulnerability management: Nessus/Tenable, CISA KEV, EPSS, CVSS, BOD 26-04, NIST CSF, FedRAMP
- Detection: Sigma, MITRE ATT&CK, Wireshark, IOC extraction
- AppSec: taint analysis, OWASP Top 10 / CWE, SARIF
- Python: CLIs, pytest, GitHub Actions
- AWS: IAM, EC2, S3, VPC, CloudTrail basics
