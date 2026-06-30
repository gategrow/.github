# GateGrow

> AI agents grow through gates. Gates grow by catching failures.

GateGrow is an open-source ecosystem of tools, methodologies, and patterns for making AI coding assistants **reliable at scale**. Each repo tackles one dimension of the problem — from session-level quality gates to cross-session learning loops.

## The Ecosystem

| Repo | Role | Elevator Pitch |
|------|------|----------------|
| **[delivery-gate](https://github.com/gategrow/delivery-gate)** | 🔒 Output enforcer | Mechanical dual-layer gate: process monitor + output blocker. No AI judgment — deterministic checks only |
| **[checkgrow](https://github.com/gategrow/checkgrow)** | 🧠 Methodology hub | Failure-driven design: 10 documented failure patterns, each traced to a real session. Every gate rule earns its place |
| **[self-audit](https://github.com/gategrow/self-audit)** | 🩺 Self-audit CLI | `pip install`-able tool. Four-dimension audit (Completeness/Consistency/Groundedness/Honesty) on any text output. Zero dependencies |
| **[dual-pool-review](https://github.com/gategrow/dual-pool-review)** | 🔬 Review system | Named-persona adversarial review with dual-pool architecture: fixed pool (convergence) + random pool (divergence). Quote-first, symmetric burden |
| **[session-cost](https://github.com/gategrow/session-cost)** | 📊 Cost intelligence | L0→L3 layered analysis: collect → observe → analyze → auto-generate optimization reports. Know when your tool habits change |

## How They Fit Together

```
┌─────────────┐
│ session-cost │  ←── Measures what happened
└──────┬───────┘
       │ feeds data to
       ▼
┌─────────────┐
│delivery-gate │  ←── Enforces what must happen
└──────┬───────┘
       │ catches failures → feeds
       ▼
┌─────────────┐
│  checkgrow   │  ←── Learns from failures
└──────┬───────┘
       │ supplies patterns to
       ▼
┌─────────────┐     ┌─────────────┐
│dual-pool-review│◄──│  self-audit │  ←── Verify before shipping
└─────────────┘     └─────────────┘
```

## Philosophy

- **Mechanical where possible, reasoning where necessary** — deterministic checks never hallucinate
- **Failure-driven design** — every rule traces to a documented, reproducible failure
- **Open loop tracking** — every check leaves a record, every decision links to evidence
- **Dual-pool thinking** — convergence (deep expertise) + divergence (fresh eyes) cross-orchestrated

## Getting Started

1. **[delivery-gate](https://github.com/gategrow/delivery-gate)** — Install first. Catches incomplete work before you close the session.
2. **[checkgrow](https://github.com/gategrow/checkgrow)** — Read `docs/failure-patterns.md`. See what gates are catching.
3. **[self-audit](https://github.com/gategrow/self-audit)** — `pip install git+https://github.com/gategrow/self-audit.git`. Audit any output.
4. **[dual-pool-review](https://github.com/gategrow/dual-pool-review)** — Use before merging. Named-engineer perspectives catch what bots miss.
5. **[session-cost](https://github.com/gategrow/session-cost)** — Collect 15+ sessions, then check the auto-generated report.

## Contributing

Each repo has its own `CONTRIBUTING.md`. General principles:
- Open an issue before writing code
- One concern per PR
- Cite real failures, not hypothetical risks
- Cross-repo changes: update docs in all affected repos

## License

Each repo is MIT licensed unless noted otherwise.
