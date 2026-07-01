# GateGrow

Personal AI agent tools — zero-dependency Python scripts for Claude Code users.

## Frameworks

| Repo | What it is |
|------|-----------|
| **[checkgrow](https://github.com/gategrow/checkgrow)** | Unified quality framework — methodology, failure patterns, decision flow. The canonical source for the CheckGrow thesis. Start here to understand how all the tools connect. |

## Tools

| Repo | What it does |
|------|-------------|
| **[delivery-gate](https://github.com/gategrow/delivery-gate)** | Stop hook: process monitor + quality gate. Blocks session close when learning capture is stale. |
| **[self-audit](https://github.com/gategrow/self-audit)** | `pip install`-able CLI. Four-dimension text consistency audit (regex-based, no LLM). |
| **[session-cost](https://github.com/gategrow/session-cost)** | Session cost tracker. L0→L3 layered thresholds, auto monthly reports. |

## Methodologies

| Repo | What it is |
|------|-----------|
| **[dual-pool-review](https://github.com/gategrow/dual-pool-review)** | AI code review using **real people's documented principles**, not abstract roles. Fixed pool (convergence) + random pool (divergence), cross-orchestrated. Principle-first with confidence levels — never fabricate a quote. |

## License

Each repo is MIT licensed.
