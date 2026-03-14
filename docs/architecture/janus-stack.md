---
layout: janus
title: Janus Stack
permalink: /docs/architecture/janus-stack/
---

# Janus Architecture

Janus is a micro-governance layer designed to stabilize AI-assisted development.

The architecture separates concerns into five layers:

## Core

The Core defines the invariant governance model.

It is specified through the RFC series and includes:

- Evidence model
- Omission detection
- Governance events
- Human authority
- Evaluation layer
- Log reference model

The Core is intentionally minimal and stable.

## Protocol Framework

Operational discipline for AI-assisted development.

Protocols define how agents interact under the governance model.

Examples:

- Workflow protocol
- AI communication protocol
- Debug protocol
- Release protocol

Protocols may evolve without modifying the Core.

## Runtime Layer

Runtimes implement the contracts defined by the Core.

Adapters may include:

- Node environments
- Apps Script runtimes
- CSV portable environments
- other future implementations

## Demo Suite

Reference demonstrations validating the governance model.

The demo suite provides reproducible scenarios including:

- normal operation (happy path)
- omission detection
- runtime verification

## Papers

Conceptual and theoretical framing of Janus.

- Foundational paper
- future positioning and architecture papers
