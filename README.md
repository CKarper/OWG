# Open Work Graph

Open Work Graph (OWG) is an open identity and reconciliation layer for intellectual works and related entities.

OWG exists to help libraries, publishers, archives, repositories, software systems, and individuals determine when they are talking about the same thing.

The primary product of OWG is identity.

Everything else is built on top.

> [!NOTE]
> OWG is an early-stage design effort.
>
> The project currently consists of a proposed identity model, reconciliation model, governance model, and collection architecture.
>
> Many assumptions remain unvalidated.
>
> We are actively seeking feedback from librarians, archivists, publishers, repository operators, metadata specialists, and software developers.
>
> In particular, we are interested in:
>
> - Existing efforts we may have overlooked.
> - Incorrect assumptions about library science or stewardship.
> - Failure modes in governance or authority models.
> - Areas where existing systems already solve the problem sufficiently.
> - Opportunities for interoperability with existing ecosystems.
>
> The purpose of this phase is to expose ideas to criticism early enough that they can improve.

---

## Recommended Reading Order

1. [Vision](docs/001-vision.md)
2. [Project Brief](docs/004-project-brief.md)
3. [Principles](docs/003-principles.md)
4. [Identifier Specification](docs/010-identifier-spec.md)
5. [Reconciliation](docs/040-reconciliation.md)
6. [Governance](docs/030-governance.md)

---

## Core Concepts

### Philosophy

- [Manifesto](docs/000-manifesto.md)
- [Non-Goals](docs/002-non-goals.md)
- [Principles](docs/003-principles.md)

### Identity

- [Identifier Specification](docs/010-identifier-spec.md)
- [LRM and Ontology](docs/020-lrm-and-ontology.md)
- [Library Science Consumption](docs/021-library-science-consumption.md)

### Reconciliation

- [Reconciliation](docs/040-reconciliation.md)

### Governance and Trust

- [Governance](docs/030-governance.md)
- [Trust and Stewardship](docs/031-trust-and-stewardship.md)

### Collections and Holdings

- [Local Items and Item Servers](docs/050-local-items.md)

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

- [ADR-0001: ID is the Product](docs/decisions/ADR-0001-id-is-the-product.md)
- [ADR-0002: LRM Owns Meaning, OWG Owns Identity](docs/decisions/ADR-0002-lrm-owns-meaning-owg-owns-identity.md)
- [ADR-0003: Identifiers Are Separate From Resolvers](docs/decisions/ADR-0003-identifiers-are-separate-from-resolvers.md)

---

## Status

OWG is currently in the design and stewardship phase.

The project is focused on defining durable identity, governance, reconciliation, and interoperability before implementation.