---
layout: janus
title: Architectural Positioning
permalink: /docs/architecture/positioning/
---

# Architectural Positioning

Janus does not replace existing architectural models.

Instead, it introduces a governance layer that operates across systems.

## Comparison with existing approaches

| System | Governs |
|------|------|
| Event Sourcing | Domain state evolution |
| Observability | System behavior |
| Ledger systems | Transactions |
| Audit logs | Recorded actions |
| Janus | Governance coherence |

Janus focuses on ensuring that actions, events and omissions can be evaluated under explicit governance rules.

## Key difference

Traditional systems track what happened.

Janus also allows systems to reason about what **should have happened but did not**.

This capability enables omission detection and governance evaluation.

## Architectural role

Janus acts as a micro-governance layer positioned above runtimes and below operational workflows.
