# Sami Ali

Cybersecurity student at George Mason University (B.S. Information Technology, cybersecurity minor, expected May 2028), based in Northern Virginia. I'm looking for a **Summer 2027 security engineering internship**.

CompTIA Security+ and AWS Certified Cloud Practitioner. Summer 2026: intern on the DHS/CBP Vulnerability Assessment Team. Studying for OSCP and the AWS Security Specialty.

I build small defensive tools and test whether they work, including where they don't.

## Featured projects

- **[tripline](https://github.com/samiali38183/tripline)**: a test gate for security detection rules. On every pull request it replays recorded attack activity through each rule and fails the build if a rule stops catching it. In its first recording, a stock community rule caught 0 of 2 real attack events. [Live report](https://samiali38183.github.io/tripline/).
- **[sinkline](https://github.com/samiali38183/sinkline)**: a scanner for Python web apps that follows user input to dangerous calls to find injection-style bugs. I measured it against Bandit on a public benchmark and wrote up where it does badly, including a high false-positive rate. [Sample report](https://samiali38183.github.io/sinkline/).
- **[fuzzdiff](https://github.com/samiali38183/fuzzdiff)**: a memory-safe Rust rewrite of a C HTTP parser, checked against the original with tens of millions of random inputs. It found 0 differences, and it caught all 5 bugs I planted to test the checker.

## More

- [kevgate-admit](https://github.com/samiali38183/kevgate-admit): a Kubernetes webhook that blocks container images with known-exploited vulnerabilities, tested on a real cluster in CI.
- [kevgate](https://github.com/samiali38183/kevgate): an API that ranks vulnerability findings by known exploitation, EPSS, severity and asset criticality.
- [vulnlab](https://github.com/samiali38183/vulnlab): three small vulnerable services, each with an exploit proof, a fix and a detection rule.
- [kev-risk-prioritization](https://github.com/samiali38183/kev-risk-prioritization): a small scoring study on real KEV and EPSS data, with its limits stated.
- [call-kettle](https://github.com/samiali38183/call-kettle): an AI phone receptionist where booking rules are enforced in code, with a security evaluation of the AI's tool access.

## Contact

[Portfolio](https://samiali38183.github.io) · [Resume (PDF)](https://samiali38183.github.io/resume.pdf) · [LinkedIn](https://www.linkedin.com/in/sami-ali-1a4b89345) · [samiali38183@gmail.com](mailto:samiali38183@gmail.com)
