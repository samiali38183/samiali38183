# Sami Ali

Cybersecurity student at George Mason University (B.S. Information Technology, cybersecurity minor, May 2028). CompTIA Security+ and AWS Certified Cloud Practitioner. DHS HS-POWER intern on CBP's Vulnerability Assessment Team, summer 2026. Currently studying for OSCP and AWS Certified Security - Specialty. Based in Northern Virginia. Seeking Summer 2027 defensive security engineering internships.

I build tools that check security work instead of just doing it: detections that get tested, a static analyzer that gets benchmarked against Bandit, a vulnerability queue ordered by known exploitation.

## Proof

- **[tripline](https://github.com/samiali38183/tripline), detection testing in CI.** On the first Linux run, the stock SigmaHQ setuid/setgid rule matched **0 of 36** events from an Atomic Red Team test, because it looks for the literal text `chmod u+s`. I wrote a replacement rule that matches any setuid/setgid chmod form.
- **[sinkline](https://github.com/samiali38183/sinkline), taint analysis for Python web apps.** F1 **0.967** vs Bandit's **0.579** on a 109-line corpus (61 vulnerable, 48 safe variants). I labeled the corpus myself and Bandit was scored leniently; the repo documents both caveats and the known misses.
- **[kev-risk-prioritization](https://github.com/samiali38183/kev-risk-prioritization), CISA KEV + EPSS + CVSS ranking.** In the 20-finding sample, a CVSS 8.8 finding with no known exploitation ranks below every KEV match. Runs on synthetic data, KEV-first and consistent with CISA BOD 26-04 (EPSS and asset criticality are my own additions); 9 tests pass.

## Projects

| Repo | What it is | Stack |
|---|---|---|
| [tripline](https://github.com/samiali38183/tripline) | Detection quality gate: emulate ATT&CK techniques, replay the telemetry through Sigma rules, score coverage, fail PRs on regressions | Python, Sigma, MITRE ATT&CK, GitHub Actions |
| [sinkline](https://github.com/samiali38183/sinkline) | Interprocedural taint analysis for Python web apps, mapped to OWASP Top 10 / CWE, SARIF output, zero dependencies | Python `ast`, SARIF |
| [kev-risk-prioritization](https://github.com/samiali38183/kev-risk-prioritization) | KEV-first vulnerability prioritization using CISA KEV, EPSS and CVSS; built on synthetic data | Python (stdlib), CISA KEV, EPSS, CVSS |
| [cybersecurity-vault](https://github.com/samiali38183/cybersecurity-vault) | Phishing IOC extractor (10 pytest tests) and a Wireshark lab covering TCP, DNS, HTTP, TLS SNI and ARP | Python, Wireshark |
| [call-kettle](https://github.com/samiali38183/call-kettle) | AI phone receptionist for home-service shops. Claude proposes tool calls; code validates and runs them. Tenant isolation and Twilio signature checks are tested | FastAPI, Twilio, Claude tool use, Fly.io |
| [agent-engineering-lab](https://github.com/samiali38183/agent-engineering-lab) | How I run Hermes Agent, Claude Code and Codex in parallel on a phone-agent product deployed on Fly.io (no customers yet) and verify their work (5,300+ tests collected in the private codebase; a load test caught a real concurrency race) | Multi-agent workflow, Fly.io, SQLite |
| [focuslog](https://github.com/samiali38183/focuslog) | Pomodoro timer with session logging and a weekly dashboard | HTML, CSS, JavaScript |

## Contact

- Email: [samiali38183@gmail.com](mailto:samiali38183@gmail.com)
- LinkedIn: [sami-ali-1a4b89345](https://www.linkedin.com/in/sami-ali-1a4b89345)
- Portfolio: [samiali38183.github.io](https://samiali38183.github.io)
