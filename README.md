# Sami Ali

Cybersecurity student at George Mason University (B.S. Information Technology, cybersecurity minor, May 2028). CompTIA Security+ and AWS Certified Cloud Practitioner. Interned on the DHS/CBP Vulnerability Assessment Team in summer 2026. Studying for OSCP and the AWS Security Specialty. Northern Virginia. Looking for Summer 2027 security engineering internships.

[Portfolio](https://samiali38183.github.io) · [Resume (PDF)](https://samiali38183.github.io/resume.pdf) · [LinkedIn](https://www.linkedin.com/in/sami-ali-1a4b89345) · [samiali38183@gmail.com](mailto:samiali38183@gmail.com)

## Projects

**[tripline](https://github.com/samiali38183/tripline)**: a CI gate for detections. It runs ATT&CK techniques (Atomic Red Team on Linux and Windows runners, replayed Stratus Red Team and flaws.cloud logs for AWS), replays the telemetry through Sigma rules and fails the pull request when an expected rule stops firing. On its first Linux run the stock SigmaHQ setuid/setgid rule matched 0 of 36 recorded events; a custom rule closes the gap. 10 scenarios pass on recorded telemetry, 4 are pending, and prevalence-weighted coverage is 68%. [Live report](https://samiali38183.github.io/tripline/).

**[sinkline](https://github.com/samiali38183/sinkline)**: a static analyzer for Python web apps that follows request data across functions and files to SQL, shell, SSRF and deserialization sinks, and maps findings to OWASP Top 10 and CWE. SARIF output, GitHub Action, no dependencies. On its own 109-line self-labeled benchmark: precision 1.000, recall 0.984, F1 0.992, against Bandit's F1 of 0.579. [Sample report](https://samiali38183.github.io/sinkline/).

**[kevgate](https://github.com/samiali38183/kevgate)**: a vulnerability-intake API that ranks findings by CISA KEV, EPSS, CVSS and asset criticality, shipped the way a service would be: hardened container, Helm chart with network policy and restricted pod security, Terraform checked against LocalStack, and a GitHub Actions pipeline with SAST, dependency, secret, IaC and image scans, a kind-cluster deploy test and a ZAP baseline. The release image is signed with cosign.

**[kev-risk-prioritization](https://github.com/samiali38183/kev-risk-prioritization)**: the prioritization idea from my internship as a small standard-library Python tool on synthetic data. KEV matches come first, then EPSS, CVSS and asset criticality, in the spirit of CISA BOD 26-04.

## Also public

- [call-kettle](https://github.com/samiali38183/call-kettle): a phone-receptionist backend (FastAPI, Twilio) where booking rules are enforced in code, not by the model.
- [agent-engineering-lab](https://github.com/samiali38183/agent-engineering-lab): notes on working with AI coding agents and checking their output.
- [focuslog](https://github.com/samiali38183/focuslog): a small Pomodoro timer.
