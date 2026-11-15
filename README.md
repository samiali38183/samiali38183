# Sami Ali

Security engineering student building detection, application-security and vulnerability-management tools, and testing whether they work.

- **Education:** George Mason University, B.S. Information Technology with a cybersecurity minor (expected May 2028); A.S. Information Technology, Northern Virginia Community College (May 2026).
- **Experience:** Summer 2026 intern on the DHS/CBP Vulnerability Assessment Team (HS-POWER program).
- **Looking for:** a Summer 2027 security engineering internship (detection engineering, application security, vulnerability management).

## Featured projects

- **[tripline](https://github.com/samiali38183/tripline)**: a CI gate for Sigma detection rules. It replays recorded attack telemetry through each rule on every pull request and fails the build if a rule stops firing. A SigmaHQ setuid rule matched none of 36 recorded events, two of them the attack; my replacement matches both and 0 of 488 applicable benign events. [Live report](https://samiali38183.github.io/tripline/).
- **[sinkline](https://github.com/samiali38183/sinkline)**: a static taint analyzer for Python web apps. On a frozen held-out test of 346 labeled bugs it found 88 of 219 taint-class bugs at 0.77 precision (Bandit 34, Semgrep 53) and none of 127 in other classes; recall is 40%. [Sample report](https://samiali38183.github.io/sinkline/).
- **[kevgate](https://github.com/samiali38183/kevgate)**: a FastAPI service that ranks scanner findings by CISA KEV, EPSS, CVSS and asset criticality. On a Trivy scan of four old public images (1,112 findings), all 10 KEV-listed CVEs rank in the top 10, which is expected since KEV is a score input.
- **[call-kettle](https://github.com/samiali38183/call-kettle)**: an AI phone receptionist backend where the model only proposes actions and server code authorizes each one. A scripted attacker model runs 42 attacks and 6 normal requests against the real gate; all pass.

All repositories: [github.com/samiali38183?tab=repositories](https://github.com/samiali38183?tab=repositories)

## Links

[Portfolio](https://samiali38183.github.io) · [Resume (PDF)](https://samiali38183.github.io/resume.pdf) · [LinkedIn](https://www.linkedin.com/in/sami-ali-1a4b89345) · [samiali38183@gmail.com](mailto:samiali38183@gmail.com)
