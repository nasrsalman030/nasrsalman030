# Recruiter guide

[Portfolio](README.md) · [Repository guide](REPOSITORIES.md)

**Matheria** covers work and operations through Office and Finance. **Aetheria** covers creation through Studio and Music. The six products below retain their separate source repositories and technical boundaries.

## Selected projects

| Family / domain | Product and engineering focus | Technology | Evidence to explore |
| --- | --- | --- | --- |
| Matheria / Office | [ApplyFi](projects/applyfi.md): reusable application-document workflows and review | Python; document adapters | Core implementation and a 2 October 2026 publication record reporting 37 passing core tests; renderer and release checks excluded |
| Matheria / Office | [SignalHire](projects/signalhire.md): opportunity discovery and explainable matching | Python, FastAPI, SQLite / FTS5 | Workflow diagram; 30 September 2026 record reporting 64 passing tests and browser checks |
| Matheria / Finance | [PoolBoy](projects/poolboy.md): mining monitoring and reconciliation with explicit evidence coverage | Next.js, React, TypeScript, PostgreSQL | Architecture diagram; 2 October 2026 record reporting 3,162 passing tests and five listener-related failures or timeouts; build and live checks excluded |
| Matheria / Finance | [2DEXY Full-Stack](projects/2dexy-fullstack.md): trading research with interface, control and execution boundaries | Next.js, Python, Rust | Architecture and research boundaries; no profitability or live-readiness claim |
| Aetheria / Studio | [Aetheria Studio](projects/aetheria-studio.md): website creation with workspace, generator and pipeline components | Next.js, TypeScript, Python | Component map; 4 October 2026 local record reporting 4,576 passing tests, one skipped, and build / browser checks; local work may be newer than the GitHub snapshot |
| Aetheria / Music | [Master / RACK](projects/master-rack.md): editable mastering chain and predictable audio processing | C++, Web Audio / WebAssembly, Tauri | Actual application capture dated 2 October 2026; dated maintenance evidence with a narrowly defined scope |

The linked records describe point-in-time checks. Their test counts are not new results from today's portfolio review. Implemented functionality, integration coverage and release readiness are described separately on each project page.

## Evidence without publishing source

On **20 October 2026**, an authenticated GitHub metadata check confirmed that the **eight source repositories behind these six products exist and are private**. The [repository guide](REPOSITORIES.md) maps each product to its source repositories. Studio uses three repositories for one product.

This is an owner-side repository check. Public descriptions alone are not independent verification of source contents or current runtime behavior. The portfolio provides a way to inspect scope, architecture and documented engineering evidence without exposing implementation code.

For a technical discussion, useful topics include:

- A guided product walkthrough using synthetic or sanitized inputs.
- How an architecture diagram maps to component responsibilities.
- The scope and limitations of a dated build or test record.
- Decisions about failure handling, data quality and reviewable automation.

These are discussion routes, not a promise of public source access or an already available live demo. Source access, personal documents, credentials, account sessions and operational or research data are excluded from this public portfolio.

## Supporting work

[Supporting engineering tools](projects/engineering-tools.md) covers Talos and reusable workflows. Earlier variants and upstream forks are identified in the [repository guide](REPOSITORIES.md) so they can be distinguished from the six featured products.
