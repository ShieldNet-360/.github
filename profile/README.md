<div align="center">
  <img src="https://avatars.githubusercontent.com/u/276850807?v=4" width="120" alt="ShieldNet 360" />

  # ShieldNet 360

  **Security made simple.**

  We take the complexity out of cybersecurity so business owners and lean IT teams
  can stay protected without a dedicated security team — and we open-source the
  privacy-first engine that powers it.

  [![Website](https://img.shields.io/badge/website-shieldnet360.com-2b6cb0)](https://shieldnet360.com)
  [![Docs](https://img.shields.io/badge/docs-online-blue)](https://shieldnet-360.github.io/secure-edge-dlp/)
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ShieldNet-360/secure-edge-dlp/blob/main/LICENSE)
  [![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/ShieldNet-360/secure-edge-dlp/badge)](https://scorecard.dev/viewer/?uri=github.com/ShieldNet-360/secure-edge-dlp)
</div>

---

## What we do

ShieldNet 360 is a cybersecurity company built for the people who don't have a SOC.
We explain security in plain language — *what happened, why it matters, and what we're
doing about it* — and automate the response so protection doesn't add to your workload.
Our platform spans threat detection, access control, and network security — Data Leakage
Prevention is one capability within a broader 360° approach.

> **Our mission:** leverage technology to serve and grow with businesses of every size —
> making enterprise-grade protection simple, intelligent, and accessible.

### The platform

| Product | What it does |
|---------|--------------|
| **[ShieldNet Defense](https://shieldnet360.com/products/defense)** | AI-powered 24/7 detection & response — automatically detects, analyzes, and stops malware, exploits, and unauthorized access. *"Handle cyber threats in a smart and simple way."* |
| **[ShieldNet Access](https://shieldnet360.com/products/access)** | Identity & access management — verifies user, device, and conditions so only the right people reach the right systems, and keeps everything else hidden. *"The right people. The right access. No extra work."* |
| **[ShieldNet Gateway](https://shieldnet360.com/products/gateway)** | Network security — a protective barrier around your traffic that filters malicious content and keeps sensitive data private. *"Browse, work, and connect without worrying about what's lurking online."* |

Integrates with the tools you already run — AWS, GCP, Microsoft 365, Google Workspace, and Kubernetes.

## Open source: Secure Edge

The privacy-first DLP engine behind our platform is open source.

**[secure-edge-dlp](https://github.com/ShieldNet-360/secure-edge-dlp)** — a privacy-first DLP
agent for desktop. It blocks unauthorized AI tools at the DNS layer and inspects content sent
to approved tools through a multi-layer detection pipeline, all on-device.

- **163 real-world secret patterns** across 13 categories — AWS, GCP, Azure, GitHub, OpenAI,
  Stripe, Slack, PEM keys, JWTs, and PII.
- **Adversary-resistant matching** — normalizes away homoglyphs, zero-width characters, and
  base64 encoding that humans and LLMs use to sneak a secret past a regex.
- **Zero data persistence** — only aggregate counters and policy ever touch disk. No URLs,
  domains, IPs, or match contents are ever logged. ([privacy audit](https://github.com/ShieldNet-360/secure-edge-dlp/blob/main/docs/PRIVACY-AUDIT-v0.8.0.md))
- **Cross-platform** — macOS, Windows, and Linux.

| Component | What it does |
|-----------|--------------|
| **Go agent** | Embedded DNS resolver + DLP pipeline + local HTTP API |
| **Browser extension** | Intercepts pastes/uploads in-page (Chrome, Firefox, Safari) |
| **Electron tray app** | Lightweight system-tray UI for status and policy |

### Try it in 30 seconds

```bash
go install github.com/ShieldNet-360/secure-edge-dlp/agent/cmd/edge-dlp@latest
```

Or grab a signed installer from the [latest release](https://github.com/ShieldNet-360/secure-edge-dlp/releases).

## Built to be trusted

Security software has to earn trust, so we ship the receipts: **CodeQL** SAST, **OpenSSF
Scorecard**, **SLSA** build provenance, **Sigstore**-signed releases, **reproducible agent
builds**, and a published **CycloneDX SBOM** on every release.

## From the blog

Practical security guidance for lean teams — [more on shieldnet360.com](https://shieldnet360.com/resources/blog):

- [EDR vs MDR: which should an SME choose?](https://shieldnet360.com/resources/blog/edr-vs-mdr-which-should-an-sme-choose-en-950)
- [Account Takeover Prevention: A Practical Guide for SMEs](https://shieldnet360.com/resources/blog/account-takeover-prevention-a-practical-guide-for-smes-en-1138)
- [What Are Shared Password Security Risks? An SME IT Guide](https://shieldnet360.com/resources/blog/what-are-shared-passwords-security-risks-sme-it-guide-en-1137)
- [How to Prevent Insider Threats with Smarter Access Controls](https://shieldnet360.com/resources/blog/how-to-prevent-insider-threats-with-smarter-access-controls-en-958)
- [Incident triage for lean teams: prioritize what matters fast](https://shieldnet360.com/resources/blog/incident-triage-for-lean-teams-prioritize-what-matters-fast-en-967)

## Repositories

- **[secure-edge-dlp](https://github.com/ShieldNet-360/secure-edge-dlp)** — the open-source DLP agent, extension, and desktop app.
- **[secure-edge](https://github.com/ShieldNet-360/secure-edge)** — supporting project.

## Get involved

We welcome contributions — new detection patterns and domain lists are a great first PR. See
the [contributing guide](https://github.com/ShieldNet-360/secure-edge-dlp/blob/main/CONTRIBUTING.md)
and [report security issues responsibly](https://github.com/ShieldNet-360/secure-edge-dlp/blob/main/SECURITY.md).

<div align="center">
  <sub>

  [Website](https://shieldnet360.com) · [Documentation](https://shieldnet-360.github.io/secure-edge-dlp/) · [LinkedIn](https://www.linkedin.com/showcase/shieldnet360) · [X](https://x.com/ShieldNet360) · [Facebook](https://www.facebook.com/ShieldNet360/) · MIT Licensed

  </sub>
</div>
