# Product status

This snapshot reflects the Pokate Labs product catalog dated **2026-10-04**. It separates implementation maturity from the target portfolio. Planned and experimental labels do not mean released or generally available.

| Area | Product | Status | User job |
| --- | --- | --- | --- |
| Control | Pokate Runtime | Experimental | Run an agent in a selected workspace without ambient computer authority. |
| Control | Pokate Mandate | Planned | Bind human delegation to a task and its exact scope. |
| Control | Pokate Arbiter | Experimental | Coordinate agents sharing computer resources. |
| State | Pokate Passport | Experimental | Continue work across agents with context you can verify. |
| State | Pokate Twin | Planned | Expose relevant, fresh machine context within granted scope. |
| State | Pokate Atlas | Planned | Discover capabilities the current host can support. |
| Safety | Pokate Branch | Planned | Stage selected changes before they reach live state. |
| Safety | Pokate Time Machine | Planned | Recover supported changes without overwriting newer human work. |
| Safety | Pokate Witness | Planned | Distinguish declared actions from independently observed effects. |
| Lab | Pokate Lab | Planned | Test agents against repeatable computer workflows. Tracks: Evaluation, Benchmarking, Certification. |
| Human control plane | Pokate Companion | Development preview | Supervise agent work through a clear conversation. |
| Capability SDK | Pokate Bridge | Planned | Build reliable, bounded application capabilities for agents. |

Mac is the current implementation focus and remains experimental. Windows and Linux adapters are planned. Product presence here is not a claim of independent release, availability, certification, or platform parity.

## What status means

- **Experimental:** a bounded implementation exists; broader product and release evidence remains open.
- **Development preview:** an existing implementation can be evaluated during development; it is not a general-availability claim.
- **Planned:** the product has a defined direction and job, while implementation and acceptance evidence remain open.

Every product needs its own acceptance scenario, accountable human owner, privacy and retention policy, tests, support and recovery behavior, and release evidence. A passing test suite or roadmap document alone does not close those gates. See [product architecture](product-architecture.md) and [roadmap direction](roadmap.md).
