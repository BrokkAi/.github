# Brokk

**AI for large codebases.** We build the analysis, runtime, and agent layers that
let coding agents work on repositories too big to fit in a context window.

Everything below is open source and independently usable. Start with whichever
layer matches your problem.

---

## Analysis

| | |
|---|---|
| **[bifrost](https://github.com/BrokkAi/bifrost)** | Multi-language static analysis for agents, editors, and large repositories. One IR across languages, a real query language (RQL), and MCP/LSP/CLI/Python/Rust interfaces. `Apache-2.0` · [docs](https://bifrost.brokk.ai/) |
| **[code-semantic-model-interchange](https://github.com/BrokkAi/code-semantic-model-interchange)** | Experimental, language-neutral specification for portable semantic models of code. `Apache-2.0` · [docs](https://csmi.brokk.ai/) |
| **[csmi-demo](https://github.com/BrokkAi/csmi-demo)** | Reproducible interoperability demos comparing static-analysis results with and without the same CSMI semantic pack. `Apache-2.0` |
| **[quicksilver](https://github.com/BrokkAi/quicksilver)** | Impact-selected mutation testing for Cargo workspaces: each mutant runs only the tests that execute it. `LGPL-3.0` |
| **[bifrost-policy-scan](https://github.com/BrokkAi/bifrost-policy-scan)** | GitHub Action for Bifrost policy scans: SARIF upload, diff-aware PR gating. |
| **[bifrost-extension-template](https://github.com/BrokkAi/bifrost-extension-template)** | Reference template for building your own analysis extensions on Bifrost's stable APIs. |

## Agents and runtime

| | |
|---|---|
| **[mjolnir](https://github.com/BrokkAi/mjolnir)** | Terminal client for ACP coding agents, with model-first routing and a multi-agent coding council. `GPL-3.0` · [docs](https://mjolnir.brokk.ai/) |
| **[anvil](https://github.com/BrokkAi/anvil)** | Portable Agent Client Protocol (ACP) server: model routing, tools, permissions, sandboxing, MCP. `LGPL-3.0` · [docs](https://anvil.brokk.ai/) |
| **[hel](https://github.com/BrokkAi/hel)** | ACP session manager and remote execution environment. |
| **[muse-acp](https://github.com/BrokkAi/muse-acp)** | Use a Meta Muse Code subscription from Zed, IntelliJ IDEA, and other ACP clients. |
| **[codex-acp](https://github.com/BrokkAi/codex-acp)** | ACP server for Codex CLI, maintained for smoother client and IDE integration. |

## Repository automation

Small, composable services for putting ACP agents to work on GitHub repositories.

| | |
|---|---|
| **[brokk-town](https://github.com/BrokkAi/brokk-town)** | Local browser and terminal control plane for coordinated issue, review, release, and discovery workflows. |
| **[issue-bot](https://github.com/BrokkAi/issue-bot)** | Walks GitHub issues, prepares fixes with a configurable ACP agent, and opens pull requests for review. |
| **[review-bot](https://github.com/BrokkAi/review-bot)** | Reviews pull requests with an ACP agent and independently verifies findings before posting them. |
| **[release-bot](https://github.com/BrokkAi/release-bot)** | Drives repository releases and verifies publication before recording success. |
| **[bug-bot](https://github.com/BrokkAi/bug-bot)** / **[feature-bot](https://github.com/BrokkAi/feature-bot)** | Discover useful bugs and feature opportunities, deduplicate them, and file reviewed GitHub issues. |

## Measurement

We publish our benchmarks rather than only our numbers.

| | |
|---|---|
| **[powerrank](https://github.com/BrokkAi/powerrank)** | The Brokk Power Ranking of LLM coders. |
| **[usagebench](https://github.com/BrokkAi/usagebench)** | Analyzer-neutral benchmark for finding usages of a code unit. `MIT` · [results](https://brokkai.github.io/usagebench/) |
| **[dataflowbench](https://github.com/BrokkAi/dataflowbench)** | Benchmark for value flow, taint tracking, typestate, and witness quality across languages and tools. `MIT` |

---

## Where to start

- **You want code intelligence in your own agent or editor** -> [bifrost](https://github.com/BrokkAi/bifrost), then the [ten-minute evaluation](https://bifrost.brokk.ai/evaluate-bifrost/).
- **You want portable library semantics across analyzers** -> [CSMI](https://github.com/BrokkAi/code-semantic-model-interchange), then the [interoperability demos](https://github.com/BrokkAi/csmi-demo).
- **You want faster mutation testing for a Cargo workspace** -> [quicksilver](https://github.com/BrokkAi/quicksilver).
- **You want to run coding agents from a terminal** -> [mjolnir](https://github.com/BrokkAi/mjolnir).
- **You are embedding an agent runtime in a product** -> [anvil](https://github.com/BrokkAi/anvil).
- **You want to use Muse Code or Codex through an ACP client** -> [muse-acp](https://github.com/BrokkAi/muse-acp) or [codex-acp](https://github.com/BrokkAi/codex-acp).
- **You want agents to maintain a GitHub repository** -> start with [Brokk Town](https://github.com/BrokkAi/brokk-town), or run one of the focused repository bots directly.
- **You are comparing models or analyzers** -> [powerrank](https://github.com/BrokkAi/powerrank), [usagebench](https://github.com/BrokkAi/usagebench), [dataflowbench](https://github.com/BrokkAi/dataflowbench).

## Community

[Discord](https://discord.gg/EpwkYEByN) · [brokk.ai](https://brokk.ai) · Issues and PRs welcome on any repository above.
