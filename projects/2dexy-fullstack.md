# 2DEXY Full-Stack

**Matheria · Finance · Trading-system research**

2DEXY Full-Stack is a web-based trading-system engineering project. It separates the operator interface, control and learning workflows, and low-latency execution so that decisions and outcomes can be inspected across the system.

[Portfolio](../README.md) · [Mining operations: PoolBoy](poolboy.md)

## System architecture

| Layer | Responsibility | Technology |
| --- | --- | --- |
| Operator interface | Configuration, diagnostics and research visibility | Next.js |
| Control and learning | Data workflows, orchestration and evaluation | Python |
| Execution engine | Low-latency transaction handling | Rust |

## Current engineering focus

- Traceable data collection and paper-trade outcome lineage.
- Explicit risk gates, accounting and recovery behavior.
- Reproducible ML / signal evaluation and profitability analysis.
- Project identity and operating guides that distinguish this web system from earlier variants.

Current work continues across those areas. The engineering question is whether the whole decision-to-outcome chain produces trustworthy evidence, rather than whether an interface looks healthy in isolation.

## Evidence and development status

This is an active development and research system. Repository guidance separates process health, paper diagnostics, economic evidence and authorization for shadow or live operation. Build success and model metrics do not establish trading readiness or profitability.

No live-readiness or return claim is made here. Credentials, wallet records and private trading / training evidence remain outside the portfolio.

## Earlier dashboard

The public [2DEXY dashboard](https://github.com/nasrsalman030/2dexy-dashboard) is an earlier Flask / SQLite dashboard and control-plane implementation. It is separate from the current Next.js / Python / Rust Full-Stack system. Its README explains that scope; its code is not a current Full-Stack release.
