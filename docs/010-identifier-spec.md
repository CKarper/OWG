# Identifier Specification (Draft)

## Principles

- IDs are immutable.
- IDs are opaque.
- IDs are human-friendly.
- IDs are globally unique within their namespace.
- IDs are separate from resolvers.

## Format

Canonical display format:

`<type>-XXX-XXX-XXXC`

Example:

`W-8K4-P9D-2MQ`

Where:

- `W` = entity type
- `8K4P9D2M` = payload
- `Q` = check character

## Variable Length

OWG identifiers are variable-length.

Consumers MUST NOT assume a fixed payload length.

Consumers MUST accept identifiers longer than any currently issued identifier.

The initial minting policy SHOULD issue identifiers with an 8-character payload.

Future allocation policies MAY issue longer payloads without introducing a new namespace generation.

## Entity Types (Initial)

- W = Work
- E = Expression
- M = Manifestation
- A = Agent
- S = Subject

## Resolver Independence

The identifier is not a URL.

The identifier is not tied to a specific resolver implementation.

A canonical OWG resolver may exist, but identifiers must remain valid independently of resolver technology.
