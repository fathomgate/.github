<h1 align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/fathomgate/fathomgate/main/design/brand/fathomgate-horizontal-dark.svg">
    <img src="https://raw.githubusercontent.com/fathomgate/fathomgate/main/design/brand/fathomgate-horizontal-light.svg" alt="Fathomgate" width="560">
  </picture>
</h1>

<h3 align="center">Safe passage for AI on your network.</h3>

<p align="center">
  Network-aware policy enforcement for AI-driven operations.<br>
  <strong>AI can act. Your rules decide how.</strong>
</p>

<p align="center">
  <a href="https://github.com/fathomgate/fathomgate">Explore the project</a> &nbsp;·&nbsp;
  <a href="https://github.com/fathomgate/fathomgate/blob/main/ARCHITECTURE.md">Architecture</a> &nbsp;·&nbsp;
  <a href="https://github.com/fathomgate/fathomgate/blob/main/ROADMAP.md">Roadmap</a> &nbsp;·&nbsp;
  <a href="https://github.com/fathomgate/fathomgate/blob/main/CONTRIBUTING.md">Contribute</a>
</p>

---

## AI capability. Human authority.

Fathomgate is an open-source project building a **network-aware policy checkpoint** between AI assistants and the Model Context Protocol (MCP) servers they use to operate infrastructure.

Reading a lab switch and changing a production core router are not the same operation. Our goal is to make those differences part of the decision: what an assistant is asking to do, which device it affects, and whose authority is required.

**Our mission:** enable organizations to use AI on critical infrastructure without surrendering control.

## The control model

| Design priority | What it means |
| --- | --- |
| **Understand the operation** | Evaluate the action and its device context, not just the tool's name. |
| **Keep people in control** | Make room for explicit allow, hold-for-approval, and deny decisions under operator-defined policy. |
| **Leave verifiable evidence** | Make decisions explainable and auditable, while reducing exposure of sensitive device output. |

Target architecture:

```text
AI assistant → Fathomgate → Network MCP server → Infrastructure
```

## Explore Fathomgate

The **[core repository](https://github.com/fathomgate/fathomgate)** is the starting point for the code, policy examples, architecture, and development roadmap.

[Try the policy engine](https://github.com/fathomgate/fathomgate#try-it) · [Installation guide](https://github.com/fathomgate/fathomgate/blob/main/docs/install.md) · [Contribution guide](https://github.com/fathomgate/fathomgate/blob/main/CONTRIBUTING.md)

<!-- Maintainer: this status reflects the main repository README reviewed on 2026-09-25. Update it when the enforcement milestone ships. -->
> [!IMPORTANT]
> **Early development.** Policy evaluation and several supporting components can be tested today. The live proxy (`fathomgate serve`) currently passes requests through unchanged and must not be relied on as a policy enforcement boundary. See the [project README](https://github.com/fathomgate/fathomgate#where-it-is-today) and [roadmap](https://github.com/fathomgate/fathomgate/blob/main/ROADMAP.md) for current capabilities and planned work.

## Build with us

We welcome network engineers, automation teams, security practitioners, and MCP developers. Help shape real-world policy examples, server profiles, testing, documentation, and operational requirements through the [contribution guide](https://github.com/fathomgate/fathomgate/blob/main/CONTRIBUTING.md).

<p align="center">
  <sub>Open-source core · <a href="https://github.com/fathomgate/fathomgate/blob/main/LICENSE">Apache License 2.0</a> · Built around network operations</sub>
</p>
