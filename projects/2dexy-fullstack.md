# 2DEXY Full-Stack

**Matheria · Finance · Trading-system research**

2DEXY Full-Stack is a web-based trading-system engineering and research project. It separates the operator interface, control and learning workflows, and execution so that the path from a decision to its outcome can be inspected.

[Portfolio](../README.md) · [Role and engineering approach](../ENGINEERING.md) · [Mining operations](poolboy.md)

## Problem and constraints

A responsive interface does not establish that a trading system has reliable data, credible evaluations or accounted-for execution outcomes. The project treats those as separate questions. Its research scope requires traceable inputs, explicit risk boundaries and a clear distinction between paper diagnostics and authorization for shadow or live operation.

## Documented architecture and decisions

**Next.js operator interface.** Configuration, diagnostics and research visibility sit in the web layer. That gives the operator a place to inspect the system without treating the interface itself as evidence that execution is ready.

**Python control and learning workflows.** Data workflows, orchestration and evaluation have a separate responsibility from transaction handling. Reproducible ML and signal evaluation remain part of the engineering work.

**Rust execution engine.** Transaction handling has its own execution boundary. Low latency is an engineering objective; no measured latency or execution-reliability result is claimed on this page.

The separation makes contracts between the layers part of the verification problem. A change to one layer must still be assessed against the complete decision-to-outcome chain.

## Current work and evidence boundary

The documented system has a defined three-layer structure and operating guidance. Current work continues on data collection, paper-trade outcome lineage, risk gates, accounting and recovery behavior. These are engineering priorities, not a list of completed release gates.

Repository guidance distinguishes process health, paper diagnostics and economic evidence. The public material does not establish a current passing end-to-end runtime or live-operation gate. Build success and model metrics alone do not establish trading readiness or profitability.

Further operational claims require project-specific evaluation and recovery evidence under stated conditions. Credentials, wallet records, implementation code and private trading or training records remain outside the portfolio.

## Earlier dashboard

The earlier `2dexy-dashboard` is a Flask / SQLite dashboard and control-plane implementation. Its source repository was made private on 20 October 2026. It is separate from the current Next.js / Python / Rust system; evidence or implementation from that earlier variant is not presented as a current Full-Stack release.
