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

- **Atlassian Rovo prompt-injection exfil** — AI assistant can be steered (via poisoned content or crafted links) to pull Jira/Confluence data the user can access and POST it externally; one path fixed, another still open as of disclosure. Treat agent egress + tool allow-lists as non-negotiable zero-trust controls. [Details](https://thehackernews.com/2026/08/atlassian-rovo-can-be-tricked-into.html)
- **Claude Code + Gemini CLI CI agent flaws** — Unprivileged GitHub issue sufficient to reach runner code execution / secret theft on vendor default agent workflows (CVSS 10 on Gemini path). AI coding agents in CI are now tier-0 attack surface; pin, sandbox, and never give them untrusted context + secrets. [Analysis](https://thehackernews.com/2026/08/claude-code-and-gemini-cli-flaws-let.html)
- **Microsoft Zero Trust for AI + DevSecOps pillar** — New assessment checks and a 15-control-group / 91-task DevSecOps pillar that maps verify-explicitly / least-privilege / assume-breach onto source, CI/CD, IaC, and AI-assisted pipelines. Practical bridge from theory to agent-ready controls. [Blog](https://www.microsoft.com/en-us/security/blog/2026/08/04/advance-zero-trust-for-ai-new-tools-and-guidance-to-secure-ai-agents-and-devsecops/)

## Recent Focus (Archive)

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