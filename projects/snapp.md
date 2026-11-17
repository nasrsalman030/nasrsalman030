# Snapp

**Messaging prototypes · iOS · Prototype under active development**

Snapp explores an iOS messaging workflow with account linking, persistent connection state and controlled message delivery. The central engineering problem is continuity: after an interruption, the operator needs to understand the connection state, what happened to each delivery and what can safely resume.

[Portfolio](../README.md) · [Engineering overview](../ENGINEERING.md) · [YEP](yep.md)

## Design goals

The prototype's requirements focus on explicit state and recoverable work:

- **Account and connection state:** distinguish a linked account from an available connection, and make unavailable or interrupted states visible.
- **Delivery records:** retain inspectable progress so a restart can account for work already accepted and work still pending.
- **Operator control:** make stop and restart behavior explicit, with bounded recovery and observable pacing.
- **Persistence:** preserve the relevant connection and delivery state across relaunch, with clear handling when saved state is no longer usable.

These are design goals. Their implementation and behavior require evidence from the specific build being assessed.

## Evidence status

An **owner-reported development receipt dated 8 November 2026**, identified as revision `0e710eb`, described passing behavior and HTTP checks, native send checks and a build. It also reported synthetic stop/restart coverage and no duplicate accepted records in the covered scenarios.

The report excluded the full release gate, device/provider tests and the complete fault matrix. Its original artifacts were not independently inspected or the checks rerun for this portfolio. Current build/device verification and genuine interface captures are not included, so the historical report does not establish present delivery reliability.

## Next verification targets

The next evidence needed is a named build with scoped persistence, interruption and recovery checks, followed by separate device and provider validation. A successful synthetic scenario establishes only the behavior exercised under its recorded conditions.

Snapp remains a prototype. Implementation code, test tooling and detailed development records remain private.
