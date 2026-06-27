# Local Items

## Purpose

OWG distinguishes public identity from local holdings.

The public OWG layer identifies and reconciles entities such as Works, Expressions, Manifestations, Agents, and Subjects.

Local item systems describe possession, access, lending, inventory, location, and availability.

## Items

An Item represents a specific held instance of a Manifestation.

Examples include:

- A book on a personal shelf
- A copy held by a public library
- A copy held by a university
- A digital copy managed by a local collection system
- A publisher-controlled lending unit

## Local Authority

Item data belongs to the holder or operator of the collection system.

OWG may define conventions for item interoperability, but OWG should not require all item records to live in the central OWG namespace.

## Relationship to OWG IDs

Local item records may refer to OWG identifiers for Works, Expressions, and Manifestations.

This allows many local systems to share a common identity layer without sharing private collection data.

## Item Servers

Item Servers are the bridge between OWG identity and real-world holdings.

An Item Server does not necessarily store or serve the underlying artifact.

Instead, it asserts the existence of an Item and links that Item to OWG identifiers.

An Item may refer to:

- A physical object
- A digital file
- An OPDS entry
- A checkout system
- A licensing system
- A private collection

## Federation

Item Servers are locally authoritative.

Organizations and individuals may operate their own Item Servers while participating in the shared OWG identity layer.

Examples include personal libraries, public libraries, universities, publishers, and community collections.

The OWG ecosystem may define interoperability standards for Item Servers without requiring centralized ownership of Item data.