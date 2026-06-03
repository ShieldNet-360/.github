<div align="center">
  <img src="https://raw.githubusercontent.com/ShieldNet-360/.github/main/profile/assets/shieldnet360-mark.png" width="110" alt="ShieldNet 360" />

  # ShieldNet 360

  Security Open Source Projects from ShieldNet 360

  ## Security made simple.

  ShieldNet 360 is a cybersecurity suite for small and medium businesses. It integrates
  baseline controls and automation into workflows teams already run, so security doesn't
  require heavy tooling or an in-house team to operate.

  [![Website](https://img.shields.io/badge/website-shieldnet360.com-2b6cb0)](https://shieldnet360.com)
  [![Docs](https://img.shields.io/badge/docs-online-blue)](https://shieldnet-360.github.io/prompt-gate/)
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ShieldNet-360/prompt-gate/blob/main/LICENSE)
  [![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/ShieldNet-360/prompt-gate/badge)](https://scorecard.dev/viewer/?uri=github.com/ShieldNet-360/prompt-gate)
</div>

---

## OSS project

The open-source security (OSS) project extends ShieldNet 360's core principle —
*security made simple* — into AI-embedded workflows. It is a self-hosted toolkit that adds
independent security checks at the **point of egress**.

Engineering and vibe-coding teams operate on AI copilots and low-code platforms **without**
exposing proprietary data through prompts, commits, or public deploys, and **without** shipping
flaws introduced by AI-generated code. Each module installs a default protection layer, runs
policy checks at the source, and writes audit logs on demand — without blocking developer
pipelines.

## How it fits ShieldNet 360

Data leakage prevention is one capability within a broader 360° suite that also covers threat
detection, access control, and network security. The ShieldNet 360 repo is the developer-facing,
self-hosted module — the rest of the suite is cloud-managed and aimed at SMB owners and operators.

## About ShieldNet 360

ShieldNet 360 is built to make cybersecurity simple and human. Our solutions are easy to adopt,
deliver proven results, and support SMBs in expanding their businesses without trading off risk
tolerance.

| Product | How it works |
|---------|--------------|
| **ShieldNet Defense** | AI-powered 24/7 detection & response — automatically detects, analyzes, and stops malware, exploits, and unauthorized access. |
| **ShieldNet Access** | Identity & access management — verifies user, device, and conditions so only the right people reach the right systems, and keeps everything else hidden. |
| **ShieldNet Gateway** | Network security — a protective barrier around your traffic that filters malicious content and keeps sensitive data private. |

Integrates with the tools you already run — AWS, GCP, Microsoft 365, Google Workspace, and Kubernetes.

## Repositories

**[Prompt Gate](https://github.com/ShieldNet-360/prompt-gate)** — the open-source DLP agent,
browser extension, and desktop app.

It blocks unauthorized AI tools at the DNS layer and inspects content sent to approved tools
through a multi-layer detection pipeline, all on-device.

- **163 real-world secret patterns** across 13 categories — AWS, GCP, Azure, GitHub, OpenAI,
  Stripe, Slack, PEM keys, JWTs, and PII.
- **Adversary-resistant matching** — normalizes away homoglyphs, zero-width characters, and
  base64 encoding that humans and LLMs use to sneak a secret past a regex.
- **Zero data persistence** — only aggregate counters and policy ever touch disk. No URLs,
  domains, IPs, or match contents are ever logged. ([privacy & data handling](https://github.com/ShieldNet-360/prompt-gate/blob/main/docs/PRIVACY-AUDIT.md))
- **Cross-platform** — macOS, Windows, and Linux.

| Component | What it does |
|-----------|--------------|
| **Go agent** | Embedded DNS resolver + DLP pipeline + local HTTP API |
| **Browser extension** | Intercepts pastes/uploads in-page (Chrome, Firefox, Safari) |
| **Electron tray app** | Lightweight system-tray UI for status and policy |

### Give it a try

```bash
go install github.com/ShieldNet-360/prompt-gate/agent/cmd/prompt-gate@latest
```

Or grab a signed installer from the [latest release](https://github.com/ShieldNet-360/prompt-gate/releases).

## Get involved

We welcome contributions — new detection patterns and domain lists are a great first PR. See the
[contributing guide](https://github.com/ShieldNet-360/prompt-gate/blob/main/CONTRIBUTING.md) and
[report security issues responsibly](https://github.com/ShieldNet-360/prompt-gate/blob/main/SECURITY.md).

## ShieldNet 360 info

| | |
|---|---|
| 🌐 **Website** | [shieldnet360.com](https://shieldnet360.com) |
| ✉️ **Email** | [support@shieldnet360.com](mailto:support@shieldnet360.com) |
| 💼 **LinkedIn** | [showcase/shieldnet360](https://www.linkedin.com/showcase/shieldnet360) |
| 𝕏 **X** | [@ShieldNet360](https://x.com/ShieldNet360) |
| 📘 **Facebook** | [ShieldNet360](https://www.facebook.com/ShieldNet360/) |

<div align="center">
  <sub>© ShieldNet 360 · MIT Licensed</sub>
</div>
