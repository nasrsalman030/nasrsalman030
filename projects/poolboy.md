# PoolBoy

**Matheria · Finance · Mining operations**

PoolBoy is a Bitcoin-mining monitoring and economics dashboard. It connects operational visibility with reporting that distinguishes credited earnings, received payouts, estimated costs and invoice evidence.

[Portfolio](../README.md) · [Trading research: 2DEXY Full-Stack](2dexy-fullstack.md)

## Interface views

### Fleet overview

![PoolBoy fleet workspace with mining metrics and individual miner states using synthetic data](../assets/previews/poolboy-fleet.png)

The fleet view brings hashrate, online count, nominal power and efficiency together with individual miner states. The synthetic example includes healthy, degraded and offline machines so the operational differences are visible.

### Reliability and history

![PoolBoy reliability workspace with daily fleet hashrate and a worker evidence table using synthetic data](../assets/previews/poolboy-reliability.png)

The reliability view connects daily fleet hashrate with worker evidence. Missing samples remain gaps, and offline days are marked separately from hashrate values.

*Both views were rendered on 17 November 2026 from the project's private interface components with synthetic demonstration data. These are static document previews. Browser interactions, data collection, account access and database behavior were not exercised; the images are not live operational captures.*

## Reporting architecture

![PoolBoy separates operational observations, reward records and cost evidence before presenting health, reconciliation and reports.](../assets/diagrams/poolboy-evidence.svg)

*Reporting architecture, not a dashboard screenshot.*

## What exists

- Pool and worker-health collection with separate reward, balance and availability records.
- Economics views with cost profiles, valuation and reconciliation.
- Profitability ledgers that expose complete, partial, estimated and withheld inputs.
- Invoice-review workflows, evidence snapshots and reporting tools.
- Operational guidance and an assistant grounded in the dashboard's available evidence.

Missing coverage remains visible. A pool credit, a wallet receipt and a verified hosting cost each answer a different question; the reporting system keeps those distinctions intact.

## Engineering and evidence

**Stack:** Next.js, React, TypeScript and PostgreSQL, with collection and reporting tooling.

The **2 October 2026 source-publication record** reports a passing typecheck and **3,162 tests passing**. Five listener-dependent tests failed or timed out; the record identifies sandbox listener errors among those failures. Database integration tests, a production build and live runtime checks were outside that publication run.

The public overview contains no real account identifiers, balances, invoices or operational records. Any values in the interface views are synthetic demonstration data. Implementation code and the preview-generation tooling remain private.

## Development status

Monitoring and evidence-aware reporting are implemented and under active refinement. Accounting completeness depends on source coverage and supplied cost evidence. Estimates are labelled; report totals are not presented as independent proof of hashing, payout receipt or investment performance.
