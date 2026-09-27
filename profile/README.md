<h1 align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/fathomgate/fathomgate/main/design/brand/fathomgate-horizontal-dark.svg">
    <img src="https://raw.githubusercontent.com/fathomgate/fathomgate/main/design/brand/fathomgate-horizontal-light.svg" alt="Fathomgate" width="560">
  </picture>
</h1>

<h3 align="center">Safe passage for AI on your network.</h3>

<p align="center">
  A network-aware policy checkpoint for AI-driven operations.<br>
  Source-available, with policy grounded in network commands and device roles.
</p>

<p align="center">
  <a href="https://github.com/fathomgate/fathomgate">Explore the project</a> &nbsp;·&nbsp;
  <a href="https://github.com/fathomgate/fathomgate/blob/main/ARCHITECTURE.md">Architecture</a> &nbsp;·&nbsp;
  <a href="https://github.com/fathomgate/fathomgate/blob/main/ROADMAP.md">Roadmap</a> &nbsp;·&nbsp;
  <a href="https://github.com/fathomgate/fathomgate/blob/main/CONTRIBUTING.md">How to help</a>
</p>

<!-- Maintainer: update this release status with each core release. -->
> [!IMPORTANT]
> **Current release: [v0.2.0 — M1, "Say no"](https://github.com/fathomgate/fathomgate/releases/tag/v0.2.0).** `fathomgate serve --policy` decides every tool call before the MCP server sees it, and every denial names its rule. An `allow` runs; a `hold` is not run until approvals arrive in M3. It does not yet mask secrets in device output (M2) or write the audit log (M4), so evaluate it in a lab with read-only device credentials. See the [roadmap](https://github.com/fathomgate/fathomgate/blob/main/ROADMAP.md) for what comes next.

---

## AI capability. Human authority.

Fathomgate is a source-available project building a **network-aware policy checkpoint** between AI assistants and the Model Context Protocol (MCP) servers they use to operate infrastructure.

Reading a lab switch and changing a production core router are not the same operation. Our goal is to make those differences part of the decision: what an assistant is asking to do, which device it affects, and whose authority is required.

**Our mission:** enable organizations to use AI on critical infrastructure without surrendering control.

## The control model

| Design priority | What it means |
| --- | --- |
| **Understand the operation** | Evaluate the action and its device context, not just the tool's name. |
| **Keep people in control** | Decide `allow`, `hold` or `deny` for every call under operator-defined policy; every denial names its rule. |
| **Leave verifiable evidence** | Make decisions explainable and auditable, while reducing exposure of sensitive device output. |

> **The parts that keep you safe stay public.** Anything that decides what's allowed, or proves what happened, stays in the public repository, where you can read, build and audit every line. Fathomgate is licensed under the [Functional Source License](https://github.com/fathomgate/fathomgate/blob/main/LICENSE) (`FSL-1.1-ALv2`): each version becomes Apache-2.0 two years after it is published, and v0.1.0, the example policies and the server profiles are Apache-2.0 already. A paid edition for teams adds scale and integrations; see [how it's funded](https://github.com/fathomgate/fathomgate/blob/main/ROADMAP.md#source-available-and-how-its-funded).

Policy decisions are enforced today; approvals, secret masking and the audit log are being added in stages:

```text
AI assistant → Fathomgate → Network MCP server → Infrastructure
```

## Explore Fathomgate

The **[core repository](https://github.com/fathomgate/fathomgate)** is the starting point for the code, policy examples, architecture, and development roadmap.

[Download v0.2.0](https://github.com/fathomgate/fathomgate/releases/tag/v0.2.0) · [Try an offline policy evaluation](https://github.com/fathomgate/fathomgate#try-it) · [Installation and verification](https://github.com/fathomgate/fathomgate/blob/main/docs/install.md)

## Build with us

Network engineers, automation teams, security practitioners and MCP developers can help through issues:

- Describe the tools in an MCP server you use so they can be classified in a server profile.
- Share a policy example for how your team operates.
- Try the release in a lab and report what was confusing or failed.

Fathomgate does not accept code from outside contributors for now: you bring the problem and the knowledge, and the maintainer writes the code. Start with the [contribution guide](https://github.com/fathomgate/fathomgate/blob/main/CONTRIBUTING.md) or [open an issue](https://github.com/fathomgate/fathomgate/issues/new/choose). For vulnerabilities, use the [private reporting process](https://github.com/fathomgate/fathomgate/security/advisories/new).

<p align="center">
  <sub>Source-available core · <a href="https://github.com/fathomgate/fathomgate/blob/main/LICENSE">FSL-1.1-ALv2</a> · Built around network operations</sub>
</p>
