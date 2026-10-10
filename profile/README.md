<p align="center">
  <img src="logo.png" width="140" alt="Juli OS logo" />
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
| **L0** Execution substrate | [`@juli-os/agents`](https://github.com/juli-os/agents) <a href="https://www.npmjs.com/package/@juli-os/agents"><img src="https://img.shields.io/npm/v/@juli-os/agents.svg?color=D97C26"></a> | tmux-based agent session runtime with delivery confirmation and self-healing. Zero npm dependencies |
| **L1** Ledger | [`@juli-os/ledger`](https://github.com/juli-os/ledger) <a href="https://www.npmjs.com/package/@juli-os/ledger"><img src="https://img.shields.io/npm/v/@juli-os/ledger.svg?color=D97C26"></a> | the append-only record of agent work — workflows, steps, case files, token usage. Zero npm dependencies (Node built-in SQLite) |
| **L2** Artifacts | [`@juli-os/artifacts`](https://github.com/juli-os/artifacts) <a href="https://www.npmjs.com/package/@juli-os/artifacts"><img src="https://img.shields.io/npm/v/@juli-os/artifacts.svg?color=D97C26"></a> | hash-registered deliverables with provenance — content stays schema-free, metadata is the only structure |
| **L3** Gates | built into [`juli-os/juli`](https://github.com/juli-os/juli) · live | human approval flows with content-hash binding — nothing leaves without a sign-off — ships as part of the engine, not a separate package |
| **L4** Routing | [`@juli-os/routing`](https://github.com/juli-os/routing) <a href="https://www.npmjs.com/package/@juli-os/routing"><img src="https://img.shields.io/npm/v/@juli-os/routing.svg?color=D97C26"></a> | multi-agent dispatch decisions as pure functions, replayable offline |
| **L5** Orchestrator | [`juli-os/juli`](https://github.com/juli-os/juli) · live | the full agent OS — chat a task in, Claude Code runs it in tmux, you approve at the gate; engine + web cockpit + deploy recipes |
| **L6** Surfaces | [`juli-os/ios`](https://github.com/juli-os/ios) · live · `@juli-os/web` · upcoming | iOS remote (SwiftUI), web cockpit, CLI |

## Surfaces today

The iOS remote is live and talking to a real engine — screenshots below were taken
against a seeded instance, not mockups (see the [tour](https://github.com/juli-os/ios#the-tour)):

<p align="center">
  <a href="https://github.com/juli-os/ios#the-tour"><img src="https://raw.githubusercontent.com/juli-os/ios/main/Screenshots/gate-approval.png" width="240" alt="Send gate — checks, approve or reject"></a>
  <a href="https://github.com/juli-os/ios#the-tour"><img src="https://raw.githubusercontent.com/juli-os/ios/main/Screenshots/agents-mesh.png" width="240" alt="Agents mesh — live topology"></a>
  <a href="https://github.com/juli-os/ios#the-tour"><img src="https://raw.githubusercontent.com/juli-os/ios/main/Screenshots/casefile-route.png" width="240" alt="Casefile — route chain and original email"></a>
</p>

## Principles

- **Adopt at your altitude** — every layer is useful alone; the whole is assembled, not required
- **Dependencies point strictly downward** — layers talk through ports, never around them
- **Humans stay in the loop** — approval gates wherever money or reputation is on the line
- **Zero-dependency first** — Node built-ins over packages whenever possible

## Status

Early days, moving bottom-up. **Three layers are live on npm** — [ledger](https://www.npmjs.com/package/@juli-os/ledger), [artifacts](https://www.npmjs.com/package/@juli-os/artifacts), [routing](https://www.npmjs.com/package/@juli-os/routing) — each installable on its own, all consumed by the engine we run in production. The [iOS remote](https://github.com/juli-os/ios) is the first surface out, and the full engine ([juli](https://github.com/juli-os/juli)) is now public — a 30-minute docker-compose quickstart, human approval gates included. Gates are a built-in of the engine rather than a separate package — approval verbs without an execution engine have no subject.

## Contact

- Open an issue in any repo under this org
- Email: [contact@juliasia.cn](mailto:contact@juliasia.cn)

---

<p align="center"><sub>Built by <b>Juli</b> · Apache-2.0</sub></p>
