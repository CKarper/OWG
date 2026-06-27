# Identifier Specification (Draft)

## Purpose

OWG identifiers provide durable identity for OWG entities.

An OWG identifier is a stable integration point that remains valid as knowledge, metadata, relationships, software systems, and stewardship evolve.

An OWG identifier identifies an entity.

It does not identify a particular description of that entity.

It does not identify a resolver.

It does not identify a database record.

## Principles

- IDs are durable.
- IDs are immutable.
- IDs are opaque.
- IDs are human-friendly.
- IDs are separate from resolvers.
- IDs are unambiguous within their authority.
- Length is an allocation policy, not an identity property.

## Authority Models

OWG defines two authority models.

### Global Authority

Globally managed entity types are issued by OWG and are globally unique within the OWG namespace.

Initial global entity types:

- W = Work
- E = Expression
- M = Manifestation
- A = Agent
- S = Subject

### Local Authority

Locally managed entity types are issued by local authorities.

Initial local entity type:

- I = Item

The same local identifier may appear in multiple namespaces without conflict.

For local entities, identity is established by:

`authority + identifier`

rather than identifier alone.

## Entity Types

OWG entity types are derived from IFLA LRM and OWG authority policies.

Conceptually:

`LRM Entity + Authority Scope = OWG Type`

Examples:

| OWG Type | LRM Entity | Authority Scope |
|----------|------------|-----------------|
| W | Work | Global |
| E | Expression | Global |
| M | Manifestation | Global |
| I | Item | Local |
| A | Agent | Global |
| S | Subject | Global |

OWG does not redefine the meaning of these entities.

LRM defines semantics.

OWG defines identity and authority.

## Logical Format

Logical format:

`T-XXXXXXXXC`

Example:

`W-8K4-P9D-2MQ`

Where:

- `W` = entity type
- `8K4P9D2M` = opaque payload
- `Q` = check character

The check character is always the final character of the identifier.

The current allocation policy begins with an 8-character payload.

Future allocation policies may increase payload length without changing the namespace.

Consumers MUST NOT assume a fixed payload length.

Consumers MUST accept identifiers longer than any currently issued identifier.

## Display Grouping

Separators are display-only.

Canonical display SHOULD group payload and check characters for readability.

Initial allocation example:

`W-8K4-P9D-2MQ`

Future valid examples:

`W-8K4-P9D-2MH-7DQ`

`W-8K4-P9D-2MH-7DX-2NQ`

Implementations should parse identifiers by removing separators, identifying the type prefix, treating the final character as the check character, and treating the intervening characters as payload.

## Alphabet

OWG identifiers use a restricted Base32 alphabet derived from Crockford Base32.

Payload alphabet:

`0123456789ABCDEFGHJKMNPQRSTVWXYZ`

Excluded characters:

- I
- L
- O

These exclusions reduce transcription errors.

## Alias Decoding

Implementations SHOULD accept the following aliases when parsing payloads:

- O -> 0
- I -> 1
- L -> 1

Implementations MUST emit canonical forms.

## Type Prefixes

Type prefixes use a separate alphabet from payload characters.

For example:

`I-A73-F8S-74W`

is valid because the leading `I` occupies the type position.

The same character would not be valid within the payload portion of the identifier.

## Resolver Independence

An OWG identifier is not a URL.

The canonical OWG resolver may publish information about an identifier.

For example:

`https://openworkgraph.org/W-8K4-P9D-2MQ`

The URL is a publication mechanism.

The identifier is the identity.

If the resolver changes, the identifier remains unchanged.

## Guarantees

OWG guarantees:

- Durability
- Immutability
- Resolver independence
- Unambiguous identity within an authority

OWG does not guarantee:

- Metadata correctness
- Consensus
- Permanent resolver implementations
- Availability of any particular source system

## Open Questions

- How should check characters be calculated?
- Should identifiers be case-insensitive?
- How should merged or split entities be represented?
- How should Item Server interoperability work?