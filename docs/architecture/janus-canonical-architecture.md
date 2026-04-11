---
layout: janus
title: Canonical Janus Architecture
permalink: /docs/architecture/janus-canonical-architecture/
---

# Canonical Janus Architecture

## Purpose

This document canonizes the authoritative Janus architecture model, superseding all prior public and internal taxonomies. It establishes a single, auditable, and professional structure for all future documentation, development, and communication.

## Canonical Janus Layer Model

The Janus architecture is defined as a strict, layered model:

1. **Core (Normative Layer)**
2. **RFCs (Formalization Layer)**
3. **Framework (Operational Layer)**
4. **Runtime(s) (Execution Layer)**
5. **Adapters (Integration Boundary Layer)**
6. **SDK / Tools (Developer Layer)**
7. **Implementations (Application Layer)**
8. **Demos (Validation Artifacts)**

## Layer Definitions

### 1. Core (Normative Layer)
- **Defines:** Governance semantics, contracts, and invariants.
- **Is Not:** Executable code, framework, or implementation.

### 2. RFCs (Formalization Layer)
- **Defines:** Formalization, evolution, and constraint of Core.
- **Is Not:** The Core itself, nor operational code.

### 3. Framework (Operational Layer)
- **Defines:** Reusable governance mechanisms implementing Core semantics.
- **Is Not:** The Core, nor an application, nor a runtime.

### 4. Runtime(s) (Execution Layer)
- **Defines:** Execution of governed evaluation.
- **Is Not:** The Core, nor the Framework, nor a demo.

### 5. Adapters (Integration Boundary Layer)
- **Defines:** Connections between external systems and Janus semantics.
- **Is Not:** The Core, nor a runtime, nor a framework.

### 6. SDK / Tools (Developer Layer)
- **Defines:** Integration-facing utilities and developer surfaces.
- **Is Not:** Normative, nor the Core, nor a runtime.

### 7. Implementations (Application Layer)
- **Defines:** Real-world systems using Janus.
- **Is Not:** The Core, nor a demo, nor a framework.

### 8. Demos (Validation Artifacts)
- **Defines:** Non-authoritative demonstration systems.
- **Is Not:** Implementations, nor the Core, nor a runtime.

## Dependency Direction

Layer dependencies are strictly top-down:

- Each layer may depend only on layers above it.
- No layer may depend on a layer below it.
- The Core is the root and has no dependencies.

## Canonical Authority

- The canonical, authoritative home of the Janus Core is the `janus-governance-core` repository.
- Any copy, mirror, or derived distribution of Core material outside this repository is non-canonical unless explicitly declared otherwise.

## Superseded Taxonomies

The following prior taxonomies are hereby superseded:

- The public web taxonomy using:
  - Protocol Framework
  - Runtime Layer
  - Demo Suite
  - Papers
- Any prior incomplete model omitting:
  - RFCs
  - Adapters
  - Demos

All references to these models are non-authoritative as of this document.

## Terminology Rules

The following terms are stabilized and must be used as defined:

- **Core**: Only the normative governance layer.
- **RFCs**: Only the formalization layer for Core.
- **Framework**: Only the operational layer implementing Core semantics.
- **Runtime**: Only the execution layer.
- **Adapters**: Only the integration boundary layer.
- **SDK**: Only developer utilities and surfaces.
- **Tools**: Only developer utilities and surfaces.
- **Implementations**: Only real-world systems using Janus.
- **Demos**: Only non-authoritative demonstration systems.

Rules:
- No use of "Framework" to refer to products or Core.
- No use of "Runtime" to refer to demos or Core.
- No use of "Implementation" to refer to the implementation layer itself.

## Interpretation Rules

- Janus Core is not executable.
- Framework is not Janus itself.
- Demos are not implementations.
- SDKs are not normative.
- Runtime is not Core.

## Open Migration Note

The following areas require future alignment and are not addressed in this document:

- Web wording
- Framework wording
- Runtime wording
- Duplicated core/lite copies
- Architecture page updates

This document canonizes the architecture only. All further migration and alignment must reference this canonical model.
