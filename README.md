# Open Work Graph

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

## The Gap

Knowledge about intellectual works exists across many systems.

A single work may be represented in:

- ISBN registries
- DOI records
- Wikidata
- Open Library
- Publisher metadata
- Library catalogs
- Institutional repositories
- Personal collections

Each system serves a different audience and solves a different problem.

As a result, the same reconciliation work is performed repeatedly across the ecosystem.

Libraries, publishers, archives, repositories, software systems, and individuals all spend effort answering the same question:

> Are these systems talking about the same thing?

The expertise to answer that question already exists.

The challenge is that the work is distributed across many institutions, communities, and software systems.

There is no widely adopted shared reconciliation layer for intellectual works.

OWG exists to help fill that gap.

## Why This Matters

Imagine building a catalog, repository, ebook library, discovery system, metadata service, or collection platform.

Before metadata can be improved, shared, corrected, or reused, the system must first determine whether records from different sources describe the same Work, Expression, Manifestation, Agent, or Subject.

That reconciliation work is often repeated independently by many organizations and individuals.

OWG exists to make reconciliation reusable.

The goal is not to replace existing systems.

The goal is to help them interoperate.

## What Is Open Work Graph?

Open Work Graph (OWG) is an open identity and reconciliation layer for intellectual works and related entities.

OWG focuses on:

- Durable identity
- Source mappings
- Provenance
- Reconciliation
- Stewardship
- Interoperability

OWG does not seek to replace libraries, publishers, archives, repositories, or existing knowledge graphs.

Instead, OWG provides a stable identity layer that allows those systems to interoperate.

## Why Not ISBN, DOI, Open Library, or Wikidata?

OWG builds on existing systems rather than competing with them.

Examples include:

- ISBN
- DOI
- Wikidata
- Open Library
- Library catalogs
- Publisher systems
- Institutional repositories

These systems are valuable and authoritative within their respective domains.

However, they were created for different purposes.

OWG focuses on a different question:

> How do we establish durable identity and open reconciliation across all of them?

OWG treats existing identifiers and catalogs as sources rather than competitors.

## Why Identity Comes First

A shared metadata commons requires shared identity.

Before systems can share metadata, corrections, provenance, relationships, or stewardship decisions, they must first establish that they are talking about the same entity.

OWG begins with identity because identity is the foundation upon which reconciliation becomes possible.

The primary product of OWG is identity.

Everything else is built on top.

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

## Recommended Reading Order

1. Vision
2. Project Brief
3. Principles
4. Identifier Specification
5. Reconciliation
6. Governance

## Architectural Decisions

- ADR-0001: ID is the Product
- ADR-0002: LRM Owns Meaning, OWG Owns Identity
- ADR-0003: Identifiers Are Separate From Resolvers

## Status

OWG is currently in the design and stewardship phase.

The project is focused on defining durable identity, governance, reconciliation, and interoperability before implementation.