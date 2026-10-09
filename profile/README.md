<p align="center">
  <img src="https://github.com/juli-os.png" width="120" alt="Juli OS logo" />
</p>

<h1 align="center">Juli OS</h1>

<p align="center"><b>The layered agent OS — adopt at your altitude.</b></p>

<p align="center">
  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img alt="License: Apache-2.0" src="https://img.shields.io/badge/license-Apache--2.0-D97C26.svg"></a>
  <img alt="Node" src="https://img.shields.io/badge/node-%E2%89%A522.18-1A1A1A.svg">
  <img alt="Status" src="https://img.shields.io/badge/status-early%20%2F%20pre--release-B8681A.svg">
</p>

Juli OS is an open ladder of **independently usable layers** for building trustworthy AI agent systems. Grab a single layer for the problem you have today, or adopt the whole OS — every layer stands on its own.

## The ladder

| Layer | Package | What you get |
|---|---|---|
| **L0** Execution substrate | `@juli-labs/agents` · upcoming | tmux-based agent session runtime with delivery confirmation and self-healing |
| **L1** Ledger | [`@juli-labs/ledger`](../ledger) · pre-release | the append-only record of agent work — workflows, steps, case files, token usage. Zero npm dependencies (Node built-in SQLite) |
| **L2** Artifacts | `@juli-labs/artifacts` · upcoming | hash-registered deliverables with provenance — content stays schema-free, metadata is the only structure |
| **L3** Gates | `@juli-labs/gates` · upcoming | human approval flows with content-hash binding — nothing leaves without a sign-off |
| **L4** Routing | `@juli-labs/routing` · upcoming | multi-agent dispatch decisions as pure functions |
| **L5** Orchestrator | `@juli-labs/core` · upcoming | the full agent OS — composition root of the ladder |
| **L6** Surfaces | `@juli-labs/web` · `@juli-labs/ios` · upcoming | web cockpit, iOS remote, CLI |

## Principles

- **Adopt at your altitude** — every layer is useful alone; the whole is assembled, not required
- **Dependencies point strictly downward** — layers talk through ports, never around them
- **Humans stay in the loop** — approval gates wherever money or reputation is on the line
- **Zero-dependency first** — Node built-ins over packages whenever possible

## Status

Early days. **L1 (`@juli-labs/ledger`) is the first layer out of the gate** — currently in private pre-release while we finish the export pipeline. The ladder grows bottom-up: artifacts, gates, and routing follow the same recipe.

## Contact

- Open an issue in any repo under this org
- Email: [contact@juliasia.cn](mailto:contact@juliasia.cn)

---

<p align="center"><sub>Built by <b>Juli</b> · Apache-2.0</sub></p>
