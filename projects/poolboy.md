# PoolBoy

**Matheria · Finance · Mining operations**

PoolBoy is a Bitcoin-mining monitoring and economics dashboard. It connects operational visibility with reporting that distinguishes credited earnings, received payouts, estimated costs and invoice evidence.

[Portfolio](../README.md) · [Trading research: 2DEXY Full-Stack](2dexy-fullstack.md)

## Interface preview

![PoolBoy mining-performance panel with synthetic fixture data and withheld rewards when coverage is incomplete](../assets/previews/poolboy-mining-performance.png)

*Static preview rendered on 17 November 2026 from the project's private interface components and synthetic test data. This document-rendered view does not exercise browser interactions, data collection, account access or database behavior. It is not a live dashboard capture.*

The panel separates recorded rewards from hashrate and makes missing coverage visible. The illustrated reward total is withheld because the fixture does not establish the required provider coverage.

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

The public overview contains no real account identifiers, balances, invoices or operational records. Any values in the interface preview are synthetic fixture data. Implementation code and the preview-generation tooling remain private.

## Development status

Monitoring and evidence-aware reporting are implemented and under active refinement. Accounting completeness depends on source coverage and supplied cost evidence. Estimates are labelled; report totals are not presented as independent proof of hashing, payout receipt or investment performance.
