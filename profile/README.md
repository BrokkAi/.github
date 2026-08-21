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
| **[bifrost-policy-scan](https://github.com/BrokkAi/bifrost-policy-scan)** | GitHub Action for Bifrost policy scans: SARIF upload, diff-aware PR gating. |
| **[bifrost-extension-template](https://github.com/BrokkAi/bifrost-extension-template)** | Reference template for building your own analysis extensions on Bifrost's stable APIs. |

## Agents and runtime

| | |
|---|---|
| **[mjolnir](https://github.com/BrokkAi/mjolnir)** | Terminal client for ACP coding agents, with model-first routing and a multi-agent coding council. `GPL-3.0` · [docs](https://mjolnir.brokk.ai/) |
| **[anvil](https://github.com/BrokkAi/anvil)** | Portable Agent Client Protocol (ACP) server: model routing, tools, permissions, sandboxing, MCP. `LGPL-3.0` · [docs](https://anvil.brokk.ai/) |
| **[hel](https://github.com/BrokkAi/hel)** | ACP session manager and remote execution environment. |

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
- **You want to run coding agents from a terminal** -> [mjolnir](https://github.com/BrokkAi/mjolnir).
- **You are embedding an agent runtime in a product** -> [anvil](https://github.com/BrokkAi/anvil).
- **You are comparing models or analyzers** -> [powerrank](https://github.com/BrokkAi/powerrank), [usagebench](https://github.com/BrokkAi/usagebench), [dataflowbench](https://github.com/BrokkAi/dataflowbench).

## Community

[Discord](https://discord.gg/EpwkYEByN) · [brokk.ai](https://brokk.ai) · Issues and PRs welcome on any repository above.
