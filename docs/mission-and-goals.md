# Pokate Labs: mission and goals

## What Pokate Labs is

Pokate Labs is an applied infrastructure company focused on AI agents that use real computers. Agents bring reasoning; operating systems provide computers and applications. Pokate builds the software between them: controlled execution, task continuity, coordination, recovery, and evidence.

The company develops independent products and shared standards for agent builders and, over time, organizations that need dependable control across valuable workspaces. Research becomes a product direction when a real user job and repeatable evidence support it.

## Mission

**Make agent work on real computers useful, understandable, and safe to supervise.**

People should be able to delegate computer work without handing an agent unrestricted access or losing sight of what it is doing. The host must enforce the boundaries, and people must be able to review consequential actions, follow progress, stop work, and understand the result.

## Long-term vision

A person can choose a supported agent for a task, grant it only the capabilities the task needs, and supervise the work from a clear human interface. Work can move between compatible agents and computers with its context and evidence intact, while each destination rechecks its own permissions. Supported changes can be reviewed and recovered. Product claims remain tied to evidence from the exact agents, hosts, and versions tested.

## Company goals

1. **Build a trustworthy execution boundary.** Route agent actions through typed, bounded capabilities enforced by the host. Keep policy and authoritative job state on the host.
2. **Keep people in charge.** Make progress, approvals, cancellation, and results clear. Require review for sensitive, consequential, external, destructive, account, purchase, communication, and security actions.
3. **Preserve useful context without transferring authority.** Let work continue across agents or machines while rechecking resource identity, permissions, and current evidence at the destination.
4. **Make supported work recoverable.** Provide review and recovery for changes where semantics are understood, preserve newer human edits, and explain when an outcome is unknown or cannot be undone.
5. **Make evidence honest and useful.** Distinguish agent claims, host execution records, independent observations, and verified outcomes. Show missing evidence and uncertainty.
6. **Prove each product independently.** Give every product a clear user job, contract boundary, human owner, privacy and retention policy, tests, support path, and release evidence.
7. **Measure real usefulness.** Evaluate repeated adoption, task completion with independent verification, recovery outcomes, approval friction, denied boundary attempts, compatibility, observation coverage, reproducibility, and customer demand.

These are company goals, not completed milestones. Targets, owners, and timelines require explicit review; the current portfolio has open implementation and proof gates.

## Who we serve

Our first audience is AI-native developers and agent builders integrating supported agents with valuable workspaces. Individuals experience the system through Pokate Companion. Organizations become a broader audience as local controls, recovery, product ownership, and evaluation gain independent evidence and repeated adoption.

## How we pursue the mission

Pokate organizes its product direction into Control, State, Safety, and Lab. Pokate Companion gives people one place to chat, review activity, and configure their system. Native host adapters enforce capabilities on each supported operating system. Pokate Bridge helps developers build compatible capabilities; it does not grant them authority.

Products should be independently useful. Shared interfaces should stay small and versioned. Local safety should remain useful without a required hosted backend, paid relay, or phone. See [product architecture](product-architecture.md) and [working principles](principles.md).
