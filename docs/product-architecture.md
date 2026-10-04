# Pokate Labs product architecture

The portfolio has four product pillars, a human control plane, a capability SDK, and platform-specific host adapters. This describes the target architecture; it is not a release or support matrix.

```text
CONTROL                 STATE                    SAFETY                    LAB
Runtime                  Passport                 Branch                    Evaluation
Mandate                  Twin                     Time Machine              Certification
Arbiter                  Atlas                    Witness                   Benchmarking
      \                    |                         |                         /
       \___________________|_________________________|________________________/
                                   |
                       Pokate Companion
                    Chat → Activity → Settings
                                   |
                   Enforcing host adapters
                         Mac · Windows · Linux

Pokate Bridge: capability SDK feeding Atlas
```

## Product boundaries

| Area | Products | Responsibility |
| --- | --- | --- |
| Control | Runtime, Mandate, Arbiter | Enforce scoped execution, reviewed delegation, and coordination around shared resources. |
| State | Passport, Twin, Atlas | Carry task context, describe scoped machine facts, and discover compatible capabilities. Availability never grants permission. |
| Safety | Branch, Time Machine, Witness | Stage selected changes, recover supported work, and distinguish declared actions from observed effects. |
| Lab | Evaluation, Certification, Benchmarking | Evaluate repeatable scenarios, report measured comparisons, and govern any future certification separately. |
| Human control plane | Companion | Let a person ask, steer, review, approve or deny, stop, and read results. Activity projects host truth. |
| Capability SDK | Bridge | Help developers describe and integrate bounded capabilities with compatible enforcing hosts. |
| Host platform | Mac, Windows, Linux adapters | Provide operating-system-specific enforcement, permissions, execution, cancellation, and recovery evidence. |

Pokate Companion spans the four pillars. It presents one user-facing flow and does not become a second source of execution state. The host chooses the available connection path; people do not need to select a transport. Direct machine controls remain an advanced path.

## Authority and evidence

- A discovered capability, task document, lease, or observation does not grant authority.
- The host checks the caller, scope, resource, policy, and current approval before dispatch.
- Agents use declared tools; they do not receive unrestricted shell, credentials, or uncontrolled desktop access.
- Sensitive and consequential effects require clear human review.
- Receipts distinguish requested, accepted, dispatched, completed, failed, stopped, and unknown outcomes when the producer can prove those states.
- A report written by an executor is not automatically independent observation. Missing coverage and uncertainty remain visible.
- Recovery applies only to supported effects and must preserve intervening human work.

## Platform scope

Mac is the current implementation focus. Mac host work remains experimental. Windows and Linux are planned adapter workstreams; they are not equivalent verified consumer hosts. Capabilities remain unavailable where the platform cannot provide tested enforcement or recovery.

## Shared foundation

Products share small, versioned concepts such as task, principal, capability, resource, authority, effect, evidence, and recovery. This is a set of compatible standards, not a requirement for one shared hosted backend. Each product owns its adoption, contract boundary, privacy and retention, tests, and release evidence. See [product status](product-status.md), [mission and goals](mission-and-goals.md), and [working principles](principles.md).
