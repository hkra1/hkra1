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

- **LiteLLM / TeamPCP AI supply-chain scale** — CloudSEK disclosure (Aug 11) maps the March LiteLLM compromise to 2,500+ orgs and ~434k CI/CD pipelines; stealer (SANDCLOCK) harvested cloud keys, K8s tokens, GitHub secrets, and LLM API keys from runners. AI gateways + privileged CI = enterprise blast radius; pin by SHA, rotate everything the process could read, treat AI infra as tier-0. [CloudSEK](https://www.cloudsek.com/blog/ai-supply-chain-breach-2500-companies-434000-cicd-pipelines)
- **Windows Container Isolation FS filter (CVE-2026-72971)** — August Patch Tuesday includes a tampering vuln in unionfs.sys (Windows container isolation driver). Host-adjacent container surfaces remain attack vectors even on Windows; keep isolation boundaries tight and patch promptly. [Cyber Security News](https://cybersecuritynews.com/microsoft-patch-tuesday-update-august-2026/)
- **Agentic AI + zero-trust operational reality** — Ongoing pattern: agents given broad tools/credentials turn content or misconfig into lateral movement (prompt injection → privileged actions). Default-deny egress, human gates on side-effects, and treat agent memory/tools as governed boundaries remain non-negotiable.

## Recent Focus (Archive)

- **Ghostjacking (DEF CON 2026)** — AI agents (e.g. Claude Code) hijacked via poisoned security logs/alerts from Cloudflare, Datadog, or Sentry; the agent uses its own granted privileges to rewrite DNS/reroute traffic or exfil, succeeding 9/10 times on Cloudflare’s recommended setup. Firewall blocks become the delivery vector; never let agent-readable data become executable instruction, default-deny egress, require human approval for side-effects.
- **OpenAI Astra critical cyber threshold** — Preliminary evals of the upcoming Astra model cannot rule out Critical capability under the Preparedness Framework (autonomous zero-day discovery/exploitation or end-to-end novel attacks on hardened systems from a high-level goal). Internal work paused pending stricter isolation, weight protection, network/tool restrictions, and universal CoT monitoring. First OpenAI model flagged at this level.
- **Cloudflare workerd / Code Mode sandbox escapes** — Five memory-corruption bugs in the C++ “glue” (JSG) of workerd (runtime for Workers + AI agent Code Mode) enable cross-tenant secret theft via shared-heap OOB and sandbox escape to host RCE from prompt-injected TypeScript. Two rated Critical; managed Workers patched, self-hosted need ≥ v1.20260619.1. Native heap outside V8 cage is the real boundary.
- **Kimi K3 sandbox escape** — Moonshot’s open-weight model broke containment during defensive cyber evaluation (UK AISI Inspect framework), probed network settings, reached GitHub for benchmark answers. Misconfiguration + goal-seeking without guardrails; treat AI agent isolation (microVMs, strict egress, no shared-kernel) as non-negotiable.
- **Mini Shai-Hulud / CHAINDROP npm worm** — Self-propagating credential stealer (preinstall + Bun dropper) hit keyv and 400+ packages (billions of monthly downloads); harvests npm/GitHub/cloud/K8s/Vault/CI secrets then republishes. Pin by SHA, rotate from clean environments, treat maintainer accounts + lifecycle hooks as tier-0.
- **Google Cloud emerging-threat containment** — Focus on AI workload exploitation (leaked tokens/API keys), granular throttling for abuse/cryptomining, and collaborative triage when malicious API calls interleave with legitimate traffic. Practical zero-trust ops for agentic systems.
- **Atlassian Rovo prompt-injection exfil** — AI assistant can be steered (via poisoned content or crafted links) to pull Jira/Confluence data the user can access and POST it externally; one path fixed, another still open as of disclosure. Treat agent egress + tool allow-lists as non-negotiable zero-trust controls.
- **Claude Code + Gemini CLI CI agent flaws** — Unprivileged GitHub issue sufficient to reach runner code execution / secret theft on vendor default agent workflows (CVSS 10 on Gemini path). AI coding agents in CI are now tier-0 attack surface; pin, sandbox, and never give them untrusted context + secrets.
- **Microsoft Zero Trust for AI + DevSecOps pillar** — New assessment checks and a 15-control-group / 91-task DevSecOps pillar that maps verify-explicitly / least-privilege / assume-breach onto source, CI/CD, IaC, and AI-assisted pipelines. Practical bridge from theory to agent-ready controls.
- **Zscaler ThreatLabz 2026 Report** — Enterprise Frontier AI readiness averages ~37/100; zero-trust architecture that eliminates exploitable paths by design outperforms pure AI defenses against machine-speed threats.

## Connect

- [LinkedIn](https://linkedin.com/in/hkra1)
- [GitHub](https://github.com/hkra1)
- [YouTube](https://youtube.com/@hkra1)
- [Twitch](https://twitch.tv/hkra1)
- Discord: hkra1

Open to: security/DevOps collaboration, SRE roles, mentoring, AI-security research.