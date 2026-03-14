---
layout: janus
title: Origin of Janus
permalink: /docs/architecture/origin-of-janus.md
---

# Origin of Janus

Janus originated from instability in AI-assisted development.

During the development of the Janus Workspace project, a data management system with AI-assisted code generation and dashboards, several recurring problems appeared:

- hallucinated code generation
- endless fix loops
- lack of verifiable evidence of changes
- inability to reliably audit runtime behavior

To stabilize development, a set of operational protocols was introduced.

These protocols attempted to enforce discipline in the interaction between humans and AI tools.

Over time, it became clear that the protocols were solving symptoms of a deeper problem: the absence of a minimal governance layer.

Janus Core emerged as the extraction of the invariant principles discovered during that process.

The Core defines the minimal governance primitives required to make AI-assisted development auditable, reproducible, and verifiable.
