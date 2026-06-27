# Open Work Graph

Open Work Graph (OWG) is an open identity and reconciliation layer for intellectual works and related entities.

OWG exists to help libraries, publishers, archives, repositories, software systems, and individuals determine when they are talking about the same thing.

The primary product of OWG is identity.

Everything else is built on top.

---

## Start Here

If you are new to the project, read these first:

- `docs/001-vision.md`
- `docs/004-project-brief.md`

These documents explain the problem OWG is trying to solve and the overall direction of the project.

---

## Core Concepts

### Philosophy

- `docs/000-manifesto.md`
- `docs/002-non-goals.md`
- `docs/003-principles.md`

### Identity

- `docs/010-identifier-spec.md`
- `docs/020-lrm-and-ontology.md`
- `docs/021-library-science-consumption.md`

### Reconciliation

- `docs/040-reconciliation.md`

### Governance and Trust

- `docs/030-governance.md`
- `docs/031-trust-and-stewardship.md`

### Collections and Holdings

- `docs/050-local-items.md`

---

## The Three OWG Products

### 1. OWG IDs

Durable identifiers for Works, Expressions, Manifestations, Agents, Subjects, and locally managed Items.

The identifier is the stable integration point.

### 2. Public Resolver

The canonical publication point for OWG reconciliation outcomes.

The resolver publishes mappings, provenance, relationships, and stewardship decisions.

### 3. Item Servers

The bridge between OWG identity and real-world collections.

Item Servers connect physical and digital holdings to shared OWG identity.

---

## Design Principles

- Identity is the product.
- LRM owns meaning; OWG owns identity.
- Identifiers are separate from resolvers.
- Reconciliation should be transparent.
- Stewardship should occur in the open.
- Existing systems should become more useful, not less relevant.

---

## Architectural Decisions

- `docs/decisions/ADR-0001-id-is-the-product.md`
- `docs/decisions/ADR-0002-lrm-owns-meaning-owg-owns-identity.md`
- `docs/decisions/ADR-0003-identifiers-are-separate-from-resolvers.md`

---

## Status

OWG is currently in the design and stewardship phase.

The project is focused on defining durable identity, governance, reconciliation, and interoperability before implementation.