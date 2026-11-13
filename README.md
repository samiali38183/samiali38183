# Sami Ali

I'm a cybersecurity student at George Mason University (B.S. Information Technology, cybersecurity minor, expected May 2028). I hold CompTIA Security+ and AWS Certified Cloud Practitioner, and I'm studying for OSCP and the AWS Security Specialty. In summer 2026 I interned on the DHS/CBP Vulnerability Assessment Team. I live in Northern Virginia and I'm looking for a Summer 2027 security engineering internship.

I build small defensive tools and check whether they work, including where they don't. Most of it is detection engineering, application security and vulnerability management.

## Projects

- [tripline](https://github.com/samiali38183/tripline) is a CI gate for Sigma detection rules. On each pull request it replays recorded ATT&CK telemetry (Linux, Windows, AWS) through the rules and fails the build if a rule that should fire stops firing. 13 of 14 scenarios pass and the suite has 212 tests. In its first recording, the stock SigmaHQ setuid rule matched 0 of the 2 attack events. [Live report](https://samiali38183.github.io/tripline/).
- [sinkline](https://github.com/samiali38183/sinkline) is a static analyzer for Python web apps. It follows request data across functions and files to dangerous sinks and writes text, JSON, SARIF or HTML, with a GitHub Action. On the 10 taint categories of OWASP BenchmarkPython (scored with my own script, not the official scorer) it gets a true-positive rate of 0.73 and a false-positive rate of 0.21. Bandit gets 0.13 and 0.06. I tuned it by reading that run's failures, so 0.73 is optimistic, and the false-positive rate is high. [Sample report](https://samiali38183.github.io/sinkline/).
- [fuzzdiff](https://github.com/samiali38183/fuzzdiff) is picohttpparser ported to safe Rust and checked against the C original with differential fuzzing. It found 0 divergences in 27.6 million generated inputs. To see whether the harness would notice a real bug, I planted 5 in the port, and it caught all 5.
- [kevgate-admit](https://github.com/samiali38183/kevgate-admit) is a Kubernetes admission webhook in Go. It denies workloads whose image digests carry CISA KEV vulnerabilities or score over a risk threshold. CI runs it on a kind cluster and checks the allow, deny and warn outcomes, then takes the webhook down to see what `failurePolicy` Fail and Ignore do.
- [kevgate](https://github.com/samiali38183/kevgate) is a vulnerability intake API that ranks findings by CISA KEV, EPSS, CVSS and asset criticality. It comes with a container image, a Helm chart and Terraform, and has 277 tests. CI runs SAST, dependency, secret and image scans, a kind deploy test and a ZAP baseline, and the release image is signed with cosign.
- [vulnlab](https://github.com/samiali38183/vulnlab) holds three small vulnerable services (SSRF, SQL injection, IDOR). Each has a proof, a fix, a Sigma rule and a note on what sinkline does and does not report. 137 tests.

Also public: [kev-risk-prioritization](https://github.com/samiali38183/kev-risk-prioritization), a small KEV-first scoring tool on synthetic data, and [call-kettle](https://github.com/samiali38183/call-kettle), a phone-receptionist backend where booking rules are enforced in code.

## Contact

[Portfolio](https://samiali38183.github.io) · [Resume (PDF)](https://samiali38183.github.io/resume.pdf) · [LinkedIn](https://www.linkedin.com/in/sami-ali-1a4b89345) · [samiali38183@gmail.com](mailto:samiali38183@gmail.com)
