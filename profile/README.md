<div align="center">
  <img src="https://avatars.githubusercontent.com/u/276850807?v=4" width="120" alt="ShieldNet 360" />

  # ShieldNet 360

  **Privacy-first, open-source security for the AI era.**

  We build endpoint protection that keeps sensitive data on the device — stopping
  secrets and PII from leaking into AI tools, without shipping your activity to the cloud.

  [![Website](https://img.shields.io/badge/website-shieldnet360.com-2b6cb0)](https://shieldnet360.com)
  [![Docs](https://img.shields.io/badge/docs-online-blue)](https://shieldnet-360.github.io/secure-edge-dlp/)
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ShieldNet-360/secure-edge-dlp/blob/main/LICENSE)
  [![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/ShieldNet-360/secure-edge-dlp/badge)](https://scorecard.dev/viewer/?uri=github.com/ShieldNet-360/secure-edge-dlp)
</div>

---

## What we build

ShieldNet 360 is an open-source security project focused on **Data Leakage Prevention (DLP)
for the age of AI assistants**. As employees paste code, credentials, and customer data into
chatbots and AI tools, the boundary that used to be "our network" is now "every browser tab."
Our software moves that control point back to the endpoint — and keeps it private.

## Flagship: Secure Edge

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

## Repositories

- **[secure-edge-dlp](https://github.com/ShieldNet-360/secure-edge-dlp)** — the DLP agent, extension, and desktop app.
- **[secure-edge](https://github.com/ShieldNet-360/secure-edge)** — supporting project.

## Get involved

We welcome contributions — new detection patterns and domain lists are a great first PR. See
the [contributing guide](https://github.com/ShieldNet-360/secure-edge-dlp/blob/main/CONTRIBUTING.md)
and [report security issues responsibly](https://github.com/ShieldNet-360/secure-edge-dlp/blob/main/SECURITY.md).

<div align="center">
  <sub>

  [shieldnet360.com](https://shieldnet360.com) · [Documentation](https://shieldnet-360.github.io/secure-edge-dlp/) · MIT Licensed

  </sub>
</div>
