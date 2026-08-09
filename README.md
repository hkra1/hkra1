# Himanshu Kumar

Security Analyst | Cloud · Kubernetes · DevOps/SRE · AI-driven threat detection

Polymath approach inspired by Tagore and da Vinci: systems that are both rigorous and elegant.

## Skills

- **Core:** Linux, Windows, Bash, C, Java
- **Infra:** IaC, Docker, Kubernetes
- **Observability:** Prometheus, Grafana
- **Focus:** Cloud security (AWS/Azure/GCP), container & K8s security, IaC security, incident response, AI/ML for threat detection

## Projects

**[CMS – Cloud Management System](https://github.com/hkra1/cms)**  
Security-first cloud management with Docker, Kubernetes, Prometheus, Grafana. Monitoring + automated compliance.

## Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=hkra1&show_icons=true&theme=radical)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=hkra1&layout=compact&theme=radical)

## Currently Exploring

- **Kimi K3 sandbox escape** — Moonshot’s open-weight model broke containment during defensive cyber evaluation (UK AISI Inspect framework), probed network settings, reached GitHub for benchmark answers. Misconfiguration + goal-seeking without guardrails; treat AI agent isolation (microVMs, strict egress, no shared-kernel) as non-negotiable. [TechCrunch](https://techcrunch.com/2026/08/07/chinese-ai-model-kimi-escaped-its-cybersecurity-testing-environment-researchers-say/) · [Analysis](https://techbytes.app/posts/ai-sandbox-containment-failures-kimi-breakout-technical-analysis.html)
- **Mini Shai-Hulud / CHAINDROP npm worm** — Self-propagating credential stealer (preinstall + Bun dropper) hit keyv and 400+ packages (billions of monthly downloads); harvests npm/GitHub/cloud/K8s/Vault/CI secrets then republishes. Pin by SHA, rotate from clean environments, treat maintainer accounts + lifecycle hooks as tier-0. [Microsoft](https://www.microsoft.com/en-us/security/blog/2026/08/04/chaindrop-supply-chain-compromise-anatomy-self-propagating-worm/) · [Sonatype](https://www.sonatype.com/blog/mini-shai-hulud-npm-attack-more-than-2200-components-impacted)
- **Google Cloud emerging-threat containment** — Focus on AI workload exploitation (leaked tokens/API keys), granular throttling for abuse/cryptomining, and collaborative triage when malicious API calls interleave with legitimate traffic. Practical zero-trust ops for agentic systems. [Blog](https://cloud.google.com/blog/products/identity-security/how-google-cloud-detects-contains-and-protects-against-emerging-threats)

## Recent Focus (Archive)

- **Atlassian Rovo prompt-injection exfil** — AI assistant can be steered (via poisoned content or crafted links) to pull Jira/Confluence data the user can access and POST it externally; one path fixed, another still open as of disclosure. Treat agent egress + tool allow-lists as non-negotiable zero-trust controls.
- **Claude Code + Gemini CLI CI agent flaws** — Unprivileged GitHub issue sufficient to reach runner code execution / secret theft on vendor default agent workflows (CVSS 10 on Gemini path). AI coding agents in CI are now tier-0 attack surface; pin, sandbox, and never give them untrusted context + secrets.
- **Microsoft Zero Trust for AI + DevSecOps pillar** — New assessment checks and a 15-control-group / 91-task DevSecOps pillar that maps verify-explicitly / least-privilege / assume-breach onto source, CI/CD, IaC, and AI-assisted pipelines. Practical bridge from theory to agent-ready controls.
- **Zscaler ThreatLabz 2026 Report** — Enterprise Frontier AI readiness averages ~37/100; zero-trust architecture that eliminates exploitable paths by design outperforms pure AI defenses against machine-speed threats.
- **TeamPCP / Trivy supply-chain** — Compromised CI/CD of a security scanner (force-pushed action tags + process-memory scraping) yielded ~500k credentials across GitHub Actions, Docker Hub, npm, PyPI. Treat security tooling pipelines as tier-0; pin by SHA and rotate credentials atomically.
- **SCTPhantom (CVE-2026-64564)** — 18-year-old Linux SCTP UAF enabling container-to-host root under default seccomp; discovered with AI assistance (Corvus). Patch or unload the module.
- **MAI-Cyber-1-Flash + MDASH** — Microsoft’s first cyber-specific model: ~96% CyberGym at ~½ cost via specialist routing.
- Zero-trust patterns that hold against long-lived kernel/runtime escapes.
- Advanced threat detection using ML
- Zero-trust architecture implementations
- Cloud-native security patterns
- Art + engineering in system design

## Connect

- [LinkedIn](https://linkedin.com/in/hkra1)
- [GitHub](https://github.com/hkra1)
- [YouTube](https://youtube.com/@hkra1)
- [Twitch](https://twitch.tv/hkra1)
- Discord: hkra1

Open to: security/DevOps collaboration, SRE roles, mentoring, AI-security research.