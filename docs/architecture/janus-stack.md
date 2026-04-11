---
layout: janus
title: Janus Stack
permalink: /docs/architecture/janus-stack/
---

# Janus Architecture


# Canonical Janus Architecture Stack

Janus is structured as a strict, layered architecture. Each layer is defined below according to the canonical model:

## 1. Core (Normative Layer)
Defines governance semantics, contracts, and invariants. The root of the architecture. Not executable code, not a framework, not an implementation.

## 2. RFCs (Formalization Layer)
Formalizes, evolves, and constrains the Core. Not the Core itself, nor operational code.

## 3. Framework (Operational Layer)
Reusable governance mechanisms implementing Core semantics. Not the Core, not an application, not a runtime.

## 4. Runtime(s) (Execution Layer)
Executes governed evaluation. Not the Core, not the Framework, not a demo.

## 5. Adapters (Integration Boundary Layer)
Connects external systems to Janus semantics. Not the Core, not a runtime, not a framework.

## 6. SDK / Tools (Developer Layer)
Integration-facing utilities and developer surfaces. Not normative, not the Core, not a runtime.

## 7. Implementations (Application Layer)
Real-world systems using Janus. Not the Core, not a demo, not a framework.

## 8. Demos (Validation Artifacts)
Non-authoritative demonstration systems. Not implementations, not the Core, not a runtime.

### Dependency Direction
Each layer may depend only on layers above it. No layer may depend on a layer below it. The Core is the root and has no dependencies.
- omission detection
- runtime verification

## Papers

Conceptual and theoretical framing of Janus.

- Foundational paper
- future positioning and architecture papers
