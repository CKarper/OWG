# AGENTS.md

## Repository-First Workflow

Before making changes, review the repository structure, `README.md`, relevant documents under `docs/`, and any ADRs under `docs/decisions/` that affect the task.

Refine existing documents before creating new ones. Preserve the current numbered document structure unless a change is explicitly requested.

Do not introduce new terminology casually. Preserve established Open Work Graph and OWG terminology.

## Core OWG Commitments

Open Work Graph (OWG) is an open identity and reconciliation layer for intellectual works and related entities.

Identity is the product. The primary product of OWG is durable identity.

LRM owns meaning; OWG owns identity. OWG adopts IFLA LRM rather than inventing a new ontology.

Identifiers are separate from resolvers. An OWG identifier is not a URL. Resolver URLs are publication mechanisms layered on top of durable identity.

Reconciliation should be transparent. Preserve source identifiers, source assertions, provenance, reconciliation history, stewardship decisions, and the current OWG position.

Stewardship should occur in the open. Decisions should be public, evidence-based, attributable, and open to disagreement.

Existing systems should become more useful, not less relevant. OWG should make libraries, publishers, archives, repositories, Wikidata, Open Library, DOI, ISBN, and other systems easier to connect and reuse.

Prefer interoperability over replacement. OWG reconciles and connects existing systems. It is not a bookstore, publisher, ebook reader, DRM platform, catalog replacement, universal knowledge graph, or social network.

## Examples

Use *The Hobbit* for identity and reconciliation examples.

Use Chris's Library for Item Server and local holdings examples.

Use NYPL for institutional stewardship examples.

## Documentation Guidelines

When changing documentation:

1. Check whether an existing document should be updated first.
2. Keep documents focused on their current purpose.
3. Preserve the distinction between public identity and local holdings.
4. Preserve the distinction between source assertions and OWG reconciliation.
5. Preserve the distinction between identifiers and resolvers.
6. Avoid implying OWG replaces existing systems.
7. Keep public-facing documents readable by librarians, archivists, publishers, repository operators, metadata specialists, and software developers.

## Change Discipline

Do not create implementation details that contradict accepted ADRs.

If a proposed change affects identity, resolver behavior, LRM alignment, reconciliation, governance, or namespace authority, review the ADRs first and add or update an ADR when the decision is durable.

Keep maintenance burden low. This repository is currently documentation-first.
