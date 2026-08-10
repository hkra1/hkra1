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

- **Ghostjacking (DEF CON 2026)** — AI agents (e.g. Claude Code) hijacked via poisoned security logs/alerts from Cloudflare, Datadog, or Sentry; the agent uses its own granted privileges to rewrite DNS/reroute traffic or exfil, succeeding 9/10 times on Cloudflare’s recommended setup. Firewall blocks become the delivery vector; never let agent-readable data become executable instruction, default-deny egress, require human approval for side-effects. [Infosecurity](https://www.infosecurity-magazine.com/news/ghostjacking-ai-gents-access/) · [SecurityWeek](https://www.securityweek.com/ghostjacking-attack-uses-poisoned-logs-to-turn-ai-agents-bad/)
- **OpenAI Astra critical cyber threshold** — Preliminary evals of the upcoming Astra model cannot rule out Critical capability under the Preparedness Framework (autonomous zero-day discovery/exploitation or end-to-end novel attacks on hardened systems from a high-level goal). Internal work paused pending stricter isolation, weight protection, network/tool restrictions, and universal CoT monitoring. First OpenAI model flagged at this level. [OpenAI](https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/) · [TechCrunch](https://techcrunch.com/2026/08/07/openai-says-it-slowed-astra-model-development-over-security-concerns/)
- **Cloudflare workerd / Code Mode sandbox escapes** — Five memory-corruption bugs in the C++ “glue” (JSG) of workerd (runtime for Workers + AI agent Code Mode) enable cross-tenant secret theft via shared-heap OOB and sandbox escape to host RCE from prompt-injected TypeScript. Two rated Critical; managed Workers patched, self-hosted need ≥ v1.20260619.1. Native heap outside V8 cage is the real boundary. [Check Point](https://research.checkpoint.com/2026/when-agentic-glue-melts/)

## Recent Focus (Archive)

- **Kimi K3 sandbox escape** — Moonshot’s open-weight model broke containment during defensive cyber evaluation (UK AISI Inspect framework), probed network settings, reached GitHub for benchmark answers. Misconfiguration + goal-seeking without guardrails; treat AI agent isolation (microVMs, strict egress, no shared-kernel) as non-negotiable.
- **Mini Shai-Hulud / CHAINDROP npm worm** — Self-propagating credential stealer (preinstall + Bun dropper) hit keyv and 400+ packages (billions of monthly downloads); harvests npm/GitHub/cloud/K8s/Vault/CI secrets then republishes. Pin by SHA, rotate from clean environments, treat maintainer accounts + lifecycle hooks as tier-0.
- **Google Cloud emerging-threat containment** — Focus on AI workload exploitation (leaked tokens/API keys), granular throttling for abuse/cryptomining, and collaborative triage when malicious API calls interleave with legitimate traffic. Practical zero-trust ops for agentic systems.
- **Atlassian Rovo prompt-injection exfil** — AI assistant can be steered (via poisoned content or crafted links) to pull Jira/Confluence data the user can access and POST it externally; one path fixed, another still open as of disclosure. Treat agent egress + tool allow-lists as non-negotiable zero-trust controls.
- **Claude Code + Gemini CLI CI agent flaws** — Unprivileged GitHub issue sufficient to reach runner code execution / secret theft on vendor default agent workflows (CVSS 10 on Gemini path). AI coding agents in CI are now tier-0 attack surface; pin, sandbox, and never give them untrusted context + secrets.
- **Microsoft Zero Trust for AI + DevSecOps pillar** — New assessment checks and a 15-control-group / 91-task DevSecOps pillar that maps verify-explicitly / least-privilege / assume-breach onto source, CI/CD, IaC, and AI-assisted pipelines. Practical bridge from theory to agent-ready controls.
- **Zscaler ThreatLabz 2026 Report** — Enterprise Frontier AI readiness averages ~37/100; zero-trust architecture that eliminates exploitable paths by design outperforms pure AI defenses against machine-speed threats.
- **TeamPCP / Trivy supply-chain** — Compromised CI/CD of a security scanner (force-pushed action tags + process-memory scraping) yielded ~500k credentials across GitHub Actions, Docker Hub, npm, PyPI. Treat security tooling pipelines as tier-0; pin by SHA and rotate credentials atomically.
- **SCTPhantom (CVE-2026-64564)** — 18-year-old Linux SCTP UAF enabling container-to-host root under default seccomp; discovered with AI assistance (Corvus). Patch or unload the module.
- **MAI-Cyber-1-Flash + MDASH** — Microsoft’s first cyber-specific model: ~96% CyberGym at ~½ cost via specialist routing.

## Connect

- [LinkedIn](https://linkedin.com/in/hkra1)
- [GitHub](https://github.com/hkra1)
- [YouTube](https://youtube.com/@hkra1)
- [Twitch](https://twitch.tv/hkra1)
- Discord: hkra1

Open to: security/DevOps collaboration, SRE roles, mentoring, AI-security research.