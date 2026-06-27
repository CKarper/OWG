# Reconciliation

## Purpose

OWG exists to reconcile identity across disparate sources.

OWG does not replace source systems.

OWG records relationships between source identifiers and OWG identifiers so that catalogs, libraries, publishers, repositories, and software systems can determine when they are talking about the same entity.

## Sources

Sources provide assertions.

Examples include:

- ISBN registries
- DOI records
- Wikidata entities
- Open Library records
- Publisher identifiers
- Library catalogs
- Institutional repositories
- Local Item Servers

Sources remain valuable in their own right.

OWG should preserve source identity, source identifiers, and provenance whenever possible.

## Source Assertions vs OWG Reconciliation

A source assertion is a claim made by a source system.

An OWG reconciliation is the current OWG position about how source assertions relate to OWG identifiers.

OWG should not collapse disagreement into false certainty.

When sources disagree, OWG should preserve enough provenance and history for consumers and stewards to understand the basis of the reconciliation decision.

## Reconciliation Targets

An OWG identifier acts as a reconciliation target.

Multiple source identifiers may refer to the same OWG identifier.

For example:

- An ISBN may identify a published Manifestation.
- An Open Library record may describe a Work or edition.
- A Wikidata entity may describe a Work, Agent, or related entity.
- A DOI may identify a registered scholarly resource.

OWG records how these identifiers relate to OWG entities.

## Stewardship

Stewardship is the process by which OWG participants review assertions, reconcile identities, resolve disagreements, and improve mappings.

Stewardship should be collaborative, public, attributable, and evidence-based.

Where possible, improvements discovered through OWG should flow back to the systems where they belong.

OWG seeks interoperability, not isolation.

## Resolution

Resolution is a service layered on top of identity and reconciliation.

The public resolver is the canonical publication point for OWG reconciliation outcomes.

Alternative resolvers may exist, but they do not supersede the canonical OWG position unless governance explicitly changes the canonical authority.

Identity remains stable regardless of resolver implementation.

## Transparency

Consumers should be able to inspect:

- Source identifiers
- Source assertions
- Provenance
- Reconciliation history
- Stewardship decisions
- Current OWG position

## Design Test

A useful question for OWG proposals is:

Does this make identity easier to reconcile across systems?

If not, it may be outside the core mission of OWG.