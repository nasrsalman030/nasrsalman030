# YEP

**Messaging prototypes · Multi-account workflows · Prototype under active development**

YEP explores messaging workflows that preserve a clear account context while coordinating campaign work. Its central design problem is separation: changing the selected account should not redirect another account's pending work, receipts or interface updates.

[Portfolio](../README.md) · [Engineering overview](../ENGINEERING.md) · [Snapp](snapp.md)

## Design goals

The intended multi-account scope is a development target. The requirements include:

- **Explicit sender identity:** show which account owns a conversation, campaign and delivery record before work proceeds.
- **Account boundaries:** keep identity, stored state, queues, events and interface state associated with the correct account.
- **Durable progress:** make pending, accepted, interrupted and resumed work inspectable across changes in connection or application state.
- **Controlled interruption:** provide observable pause and recovery behavior, with account-specific handling of delayed callbacks.

These requirements describe the intended design. They are not evidence of delivered account isolation, concurrent operation or demonstrated capacity.

## Evidence status

The project owner has reported successfully connecting an account. A **12 November 2026** local development record also reported missing native build prerequisites. The connection milestone has not been independently reproduced for a named build here, and the current resolution of those historical environment gaps has not been checked.

Current build/device verification, isolation results and genuine interface captures are not included in this portfolio. An account connection alone does not establish multi-account behavior; Snapp's results are separate from YEP evidence.

## Next verification targets

A named build and an isolated fixture workflow would allow focused checks of account switching, delayed events, persistence and interruption recovery. Device and provider behavior need their own observations. Any future capacity statement must identify the workload and conditions actually exercised.

YEP remains a prototype. Implementation code, account data, internal configuration and detailed development records remain private.
