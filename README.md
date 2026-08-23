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

![GitHub Stats] (https://github-readme-stats.vercel.app/api?username=hkra1&show_icons=true&theme=radical)
![Top Languages] (https://github-readme-stats.vercel.app/api/top-langs/?username=hkra1&layout=compact&theme=radical)

## Currently Exploring

- **Vault Secrets Operator CVE-2026-8715 (CVSS 9.6)** — AppRole `secretIDPath` lets a low-priv tenant force the operator pod to exfiltrate its own ServiceAccount token (cluster-wide Secrets read/write + serviceaccounts/token create). One hop from cluster-admin. Field removed in 1.5.0; treat operators that accept arbitrary paths/URLs as tier-0 attack surface. [Write-up](https://cherez0ff.art/blog/vault-secrets-operator-secretidpath-token-theft/) · [Advisory](https://discuss.hashicorp.com/t/hcsec-2026-28-vault-secrets-operator-vulnerable-to-arbitrary-file-read-and-credential-exfiltration-via-approle-secretidpath/)
- **Container security pivots from scan-and-patch to attack-surface reduction** — Vulnerability volume + regulatory pressure (NIST, CRA) make pure detection unsustainable. Distro Zero / minimal images (strip OS components the app never needs) remove classes of CVEs before they exist. Scanners still matter; the winning move is fewer things to scan. [SiliconANGLE / theCUBE](https://siliconangle.com/2026/08/15/container-security-attack-surface-reduction-appdevangle/)
- **Operator-as-confused-deputy pattern keeps repeating** — Vault Secrets Operator, External Secrets Operator, Argo CD, Rancher: any controller that runs with elevated privileges and accepts tenant-controlled inputs (paths, URLs, manifests) becomes a privilege-escalation oracle. Default-deny network policies + admission policies that forbid dangerous fields remain non-negotiable.

## Recent Focus (Archive)

- **llama.cpp critical memory-safety cluster (Cyera / DEF CON)** — 10 vulns (UAF, integer overflow, OOB) in the dominant local LLM runtime; two llama-server UAFs at CVSS 9.2 enable race-conditioned unauth RCE when sleep-idle is enabled. Local AI inference is now a first-class network attack surface—auth, isolation, and build pinning are mandatory. [eSecurity Planet](https://www.esecurityplanet.com/threats/def-con-34-10-vulnerabilities-put-local-ai-at-risk/) · [VulnCheck](https://www.vulncheck.com/advisories/llama-cpp-b7492-b9060-use-after-free-in-tokenization-endpoints)
- **AI-generated code security pass rate collapses to 56% (Veracode)** — 44% of generated samples contain OWASP Top 10 issues; Java fares worst at 30%. Volume without verification is just faster technical debt—treat every AI PR as untrusted until static analysis + human review + runtime proof.
- **OpenAI GPT-5.6-Cyber for defenders (Daybreak)** — Restricted cyber-permissive model answers 95% of advanced exploit/validation requests (vs ~2% for guarded variants). Capability is real; the access-control and dual-use governance problem is now acute.
- **CSA 2026 Top Threats to Cloud Computing** — Identity & access management reclaims #1; AI-Enhanced Attacks debut at #2 and AI System Compromise at #6. Traditional infra/CSP concerns drop off the list. Non-human identities, autonomous agents, and supply-chain complexity now outpace governance; treat AI systems as both weapons and high-value assets under zero-trust. [CSA Report](https://cloudsecurityalliance.org/artifacts/top-threats-to-cloud-computing-2026) · [Press](https://cloudsecurityalliance.org/press-releases/2026/08/13/ai-emerges-as-an-attack-enabler-and-target-in-csa-2026-top-threats-report)
- **SharePoint CVE-2026-55040 auth bypass actively exploited** — Critical JWT validation chain (alg:none + STS cert thumbprint + unverified actor token) lets unauthenticated attackers impersonate any site user/admin after Rapid7 PoC. Fifth SharePoint vuln exploited this year; spike in attempts Aug 12–13. Patch immediately; monitor for forged Bearer tokens. [The Hacker News](https://thehackernews.com/2026/08/attackers-exploit-sharepoint.html) · [Rapid7](https://www.rapid7.com/blog/post/ra-microsoft-sharepoint-jwt-token-authentication-bypass-cve-2026-55040/)
- **VMware vCenter CVE-2026-59310 directory traversal under active exploitation** — Network-accessible path traversal → arbitrary code + reverse_ssh persistence. 361 victim IPs across 47 countries observed post-disclosure; outbound reverse SSH bypasses inbound controls. Patch Broadcom appliances; hunt for unexpected reverse_ssh + outbound connections on vCenter hosts. [The Hacker News](https://thehackernews.com/2026/08/attackers-exploit-vmware-vcenter.html)
- **Stealing Reasoning Traces from Proprietary LLM APIs** — Encrypted CoT blocks from OpenAI, Anthropic, and Google could be replayed into weaker sibling models in the same family, recovering hidden reasoning (and secrets) in plaintext. 315k+ blocks decoded from public agent logs yielded hundreds of credentials/PII; also enables distillation and opaque prompt-injection. Providers mitigated the cross-session/oracle path; treat client-carried “encrypted” state as untrusted. [The Hacker News](https://thehackernews.com/2026/08/openai-anthropic-google-api-flaw-let.html) · [arXiv](https://arxiv.org/html/2608.09867v1)
- **LiteLLM / TeamPCP AI supply-chain scale (updated)** — CloudSEK mapping of the March LiteLLM compromise (via poisoned Trivy in CI) now ties ~2,500 orgs and ~434k CI/CD pipelines to harvested cloud keys, K8s tokens, GitHub secrets, and LLM API keys. 40-minute PyPI window; blast radius is long-lived credentials + AI gateways as privileged CI. Pin by SHA, rotate everything the runner could read, treat AI infra as tier-0. [The Hacker News](https://thehackernews.com/2026/08/malicious-litellm-releases-tied-to.html) · [CloudSEK](https://www.cloudsek.com/blog/ai-supply-chain-breach-2500-companies-434000-cicd-pipelines)
- **CrowdStrike real-time CDR + K8s control-plane detections for GKE** — Falcon Cloud Security extends real-time cloud detection/response to Google Cloud and adds Kubernetes audit-log based threat detection for the control plane (service accounts, secrets, orchestration abuse). Runtime sensors alone miss API-driven lateral movement; correlate control-plane + workload + identity. [CrowdStrike](https://www.crowdstrike.com/en-us/blog/crowdstrike-expands-real-time-cloud-detection-and-response-to-google-cloud/)
- **Windows Container Isolation FS filter (CVE-2026-72971)** — August Patch Tuesday includes a tampering vuln in unionfs.sys (Windows container isolation driver). Host-adjacent container surfaces remain attack vectors even on Windows; keep isolation boundaries tight and patch promptly.

## Connect

- [LinkedIn](https://linkedin.com/in/hkra1)
- [GitHub](https://github.com/hkra1)
- [YouTube](https://youtube.com/@hkra1)
- [Twitch](https://twitch.tv/hkra1)
- Discord: hkra1

Open to: security/DevOps collaboration, SRE roles, mentoring, AI-security research.
