<h1 align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/fathomgate/fathomgate/main/design/brand/fathomgate-horizontal-dark.svg">
    <img src="https://raw.githubusercontent.com/fathomgate/fathomgate/main/design/brand/fathomgate-horizontal-light.svg" alt="Fathomgate" width="560">
  </picture>
</h1>

<h3 align="center">Safe passage for AI on your network.</h3>

<p align="center">
  Building a network-aware policy checkpoint for AI-driven operations.<br>
  Open source, with policy grounded in network commands and device roles.
</p>

<p align="center">
  <a href="https://github.com/fathomgate/fathomgate">Explore the project</a> &nbsp;·&nbsp;
  <a href="https://github.com/fathomgate/fathomgate/blob/main/ARCHITECTURE.md">Architecture</a> &nbsp;·&nbsp;
  <a href="https://github.com/fathomgate/fathomgate/blob/main/ROADMAP.md">Roadmap</a> &nbsp;·&nbsp;
  <a href="https://github.com/fathomgate/fathomgate/blob/main/CONTRIBUTING.md">Contribute</a>
</p>

<!-- Maintainer: update this release status when the enforcement milestone ships. -->
> [!IMPORTANT]
> **Current release: [v0.1.0 — pass-through preview](https://github.com/fathomgate/fathomgate/releases/tag/v0.1.0).** The live proxy forwards tool calls without policy enforcement, approvals, response redaction or decision audit logging. Evaluate it in a lab with read-only device credentials. The standalone policy evaluator and redaction tools are available today; see the [roadmap](https://github.com/fathomgate/fathomgate/blob/main/ROADMAP.md) for planned protections.

---

## AI capability. Human authority.

Fathomgate is an open-source project building a **network-aware policy checkpoint** between AI assistants and the Model Context Protocol (MCP) servers they use to operate infrastructure.

Reading a lab switch and changing a production core router are not the same operation. Our goal is to make those differences part of the decision: what an assistant is asking to do, which device it affects, and whose authority is required.

**Our mission:** enable organizations to use AI on critical infrastructure without surrendering control.

## The planned control model

| Design priority | What it means |
| --- | --- |
| **Understand the operation** | Evaluate the action and its device context, not just the tool's name. |
| **Keep people in control** | Make room for explicit allow, hold-for-approval, and deny decisions under operator-defined policy. |
| **Leave verifiable evidence** | Make decisions explainable and auditable, while reducing exposure of sensitive device output. |

> **The parts that keep you safe stay open.** Anything that decides what's allowed, or proves what happened, is Apache-2.0 and always will be. A paid edition for teams adds scale and integrations; see [how it's funded](https://github.com/fathomgate/fathomgate/blob/main/ROADMAP.md#open-source-and-how-its-funded).

The proxy already connects these components; the policy controls above are being added in stages:

```text
AI assistant → Fathomgate → Network MCP server → Infrastructure
```

## Explore Fathomgate

The **[core repository](https://github.com/fathomgate/fathomgate)** is the starting point for the code, policy examples, architecture, and development roadmap.

[Download the preview](https://github.com/fathomgate/fathomgate/releases/tag/v0.1.0) · [Try an offline policy evaluation](https://github.com/fathomgate/fathomgate#try-it) · [Installation and verification](https://github.com/fathomgate/fathomgate/blob/main/docs/install.md)

## Build with us

Network engineers, automation teams, security practitioners and MCP developers can help without writing Go:

- Describe the tools in an MCP server you use so they can be classified in a server profile.
- Share a policy example for how your team operates.
- Try the preview in a lab and report what was confusing or failed.

Start with the [contribution guide](https://github.com/fathomgate/fathomgate/blob/main/CONTRIBUTING.md) or a [good first issue](https://github.com/fathomgate/fathomgate/issues?q=is%3Aissue%20is%3Aopen%20label%3A%22good%20first%20issue%22). For vulnerabilities, use the [private reporting process](https://github.com/fathomgate/fathomgate/security/advisories/new).

<p align="center">
  <sub>Open-source core · <a href="https://github.com/fathomgate/fathomgate/blob/main/LICENSE">Apache License 2.0</a> · Built around network operations</sub>
</p>
