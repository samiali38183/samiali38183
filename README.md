# Sami Ali

Cybersecurity student at George Mason University (B.S. Information Technology, cybersecurity minor, May 2028). CompTIA Security+ and AWS Certified Cloud Practitioner. Interned on the DHS/CBP Vulnerability Assessment Team in summer 2026. Studying for OSCP and the AWS Security Specialty. Northern Virginia, looking for Summer 2027 security engineering internships.

I build small defensive tools and try to measure whether they work, including where they do not. Current focus: detection engineering, application security and vulnerability management.

## Projects

- **[tripline](https://github.com/samiali38183/tripline)**: a CI gate for Sigma detection rules. It replays recorded ATT&CK telemetry (Linux, Windows, AWS) through the rules on each pull request and fails the build when an expected rule stops firing. 13 of 14 scenarios pass; the stock SigmaHQ setuid rule matched 0 of the 2 attack events in its first recording. [Live report](https://samiali38183.github.io/tripline/).
- **[sinkline](https://github.com/samiali38183/sinkline)**: a static analyzer for Python web apps that follows request data across functions and files to dangerous sinks, with SARIF output and a GitHub Action. On OWASP BenchmarkPython (10 taint categories, not the official scorer) it scores TPR 0.73 and FPR 0.21, against 0.13 and 0.06 for Bandit. The false-positive rate is high and documented. [Sample report](https://samiali38183.github.io/sinkline/).
- **[fuzzdiff](https://github.com/samiali38183/fuzzdiff)**: picohttpparser ported to safe Rust and checked against the C original with differential fuzzing. 0 divergences in 27.6 million generated inputs, and all 5 deliberately planted bugs were detected.
- **[kevgate-admit](https://github.com/samiali38183/kevgate-admit)**: a Kubernetes admission webhook in Go that denies workloads whose image digests carry CISA KEV vulnerabilities or an over-threshold risk score. Allow, deny and warn outcomes and a webhook outage (`failurePolicy` Fail and Ignore) are tested on a kind cluster in CI.
- **[kevgate](https://github.com/samiali38183/kevgate)**: a vulnerability intake API that ranks findings by CISA KEV, EPSS, CVSS and asset criticality. Packaged with a hardened container, Helm chart and Terraform; CI runs SAST, dependency, secret and image scans, a kind deploy test and a ZAP baseline, and the release image is signed with cosign.
- **[vulnlab](https://github.com/samiali38183/vulnlab)**: three small intentionally vulnerable services (SSRF, SQL injection, IDOR), each with a proof, a fix, a Sigma rule and a record of what sinkline does and does not report. 137 tests.

Also public: [kev-risk-prioritization](https://github.com/samiali38183/kev-risk-prioritization) (a small KEV-first scoring tool on synthetic data) and [call-kettle](https://github.com/samiali38183/call-kettle) (a phone-receptionist backend where booking rules are enforced in code).

## Contact

[Portfolio](https://samiali38183.github.io) · [Resume (PDF)](https://samiali38183.github.io/resume.pdf) · [LinkedIn](https://www.linkedin.com/in/sami-ali-1a4b89345) · [samiali38183@gmail.com](mailto:samiali38183@gmail.com)
