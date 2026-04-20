# APIs.json (apis-json)
APIs.json is an open, machine-readable specification that API providers can use to describe their API operations, similar to how websites use sitemap.xml. The format provides a lightweight means for individuals and organizations to document the location of their APIs, associated descriptions, human and machine-readable specifications, and ancillary information such as licensing, maintainers, and terms of service. It was created by Kin Lane and Steven Willmott in May 2014 and is maintained as an open IETF-style draft. The current stable version is 0.19, published in November 2024. APIs.json files can be placed at the root of any domain as /apis.json or /apis.yml for automated discovery. The specification defines root-level fields (name, description, url, apis, common), API-level fields (aid, humanURL, baseURL, tags, properties), and a comprehensive list of property types covering documentation, authentication, licensing, support, and governance. It is the foundation for the APIs.io search engine and API Commons initiative.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/apis-json/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - API Aggregation, API Cataloging, API Commons, API Discovery, API Governance, API Operations, Machine Readable, Specification, Standard

## Timestamps

- **Created:** 2026-03-26
- **Modified:** 2026-04-19

## APIs

### APIs.json Specification
The APIs.json specification defines a machine-readable JSON or YAML format for describing API operations. Unlike OpenAPI which describes the technical interface of a single API, APIs.json describes the surrounding operations of one or more APIs — documentation, authentication, pricing, terms of service, support, and other properties. Created by Kin Lane and Steven Willmott in May 2014, the specification is maintained as an informal IETF draft at apisjson.org. The current stable version is 0.19, published November 6, 2024. APIs.json files are placed at the domain root as /apis.json or /apis.yml for automated discovery by robots and search engines.

**Human URL:** [https://apisjson.org](https://apisjson.org)

#### Tags:

 - API Description, API Discovery, API Operations, Machine Readable, Specification, Standard

#### Properties

- [Documentation](https://apisjson.org/schema/)
- [Specification v0.19](https://raw.githubusercontent.com/api-evangelist/apis-json/refs/heads/main/spec/apisjson_0.19.txt)
- [JSONSchema - Schema v0.19](https://raw.githubusercontent.com/api-evangelist/apis-json/refs/heads/main/json-schema/apis-json-schema-0.19.yaml)
- [JSONSchema - Schema v0.18](https://raw.githubusercontent.com/api-evangelist/apis-json/refs/heads/main/json-schema/apis-json-schema-0.18.yaml)
- [JSONSchema - Schema v0.17](https://raw.githubusercontent.com/api-evangelist/apis-json/refs/heads/main/json-schema/apis-json-schema-0.17.yaml)
- [JSONSchema - Schema v0.20 (Draft)](https://raw.githubusercontent.com/api-evangelist/apis-json/refs/heads/main/json-schema/apis-json-schema-0.20.yaml)

## Common Properties

- [Website](https://apisjson.org)
- [Properties](https://apisjson.org/properties/)
- [Blog](https://apisjson.org/blog/)
- [GitHub Organization](https://github.com/apis-json)
- [GitHub Repository - Specification](https://github.com/apis-json/api-json)
- [GitHub Repository - Website](https://github.com/apis-json/apis-json-website)
- [GitHub Repository - Artisanal Examples](https://github.com/apis-json/artisanal)
- [GitHub Repository - Backstage Integration](https://github.com/apis-json/backstage)
- [Support](https://github.com/apis-json/api-json/issues)

## Features

| Name | Description |
|------|-------------|
| Machine-Readable API Operations | Provides a machine-readable format for documenting API operations beyond just the technical interface, covering documentation, pricing, authentication, terms of service, support, and governance. |
| Domain Root Discovery | APIs.json files can be placed at /apis.json or /apis.yml at the root of any domain, enabling automated discovery by search engines and robots without prior knowledge of the API provider. |
| Property Type System | Defines a comprehensive enumerated set of property types (OpenAPI, Documentation, Authentication, Pricing, Support, etc.) enabling consistent machine-readable indexing of API operations. |
| Federation via Include | Supports federated API directories through include references, allowing a root APIs.json to reference other APIs.json files on different servers or domains. |
| Multiple API Collections | A single APIs.json file can document multiple APIs in the apis array, with shared properties in the common section, enabling organization-wide API catalogs. |
| Authority and Non-Authority | Defines authoritative (same DNS domain) and non-authoritative entries, with conflict resolution rules giving priority to the most specific authoritative entry. |
| Overlay Support | Supports overlay specifications that can modify or extend existing APIs.json entries, enabling provider-agnostic enrichment of API metadata. |
| Version History | Maintained as a versioned specification from 0.11 through current 0.19, with full version history and diff comparisons available on GitHub and apisjson.org. |

## Use Cases

| Name | Description |
|------|-------------|
| API Discovery | API providers publish APIs.json files at their domain root so that search engines like APIs.io can automatically discover and index all their APIs without manual submission. |
| API Governance | Platform teams use APIs.json as a canonical machine-readable index of their API portfolio, enabling automated compliance checking of required operational properties like terms of service and authentication. |
| API Portal Generation | Developer portals can be automatically generated from APIs.json files by reading the properties array and presenting documentation, OpenAPI specs, getting started guides, and other resources. |
| API Commons Participation | Organizations publish APIs.json files to participate in the API Commons initiative, making their APIs discoverable and accessible to a wider developer community. |
| Internal API Catalog | Enterprises use APIs.json as the foundation for internal API catalogs, enabling discoverability of internal, partner, and public APIs using a consistent machine-readable format. |
| Backstage Integration | Teams use the APIs.json Backstage integration to import API metadata from APIs.json files into Spotify Backstage for internal developer portal use. |

## Integrations

| Name | Description |
|------|-------------|
| APIs.io | The APIs.io search engine is built entirely on the APIs.json specification, indexing submitted APIs.json files to power its API discovery and search capabilities. |
| API Commons | API Commons uses APIs.json as its core metadata format for documenting API operations across the open API ecosystem. |
| OpenAPI | APIs.json references OpenAPI specifications as a core property type, linking machine-readable API interface descriptions to their operations metadata. |
| Backstage | APIs.json files can be imported into Spotify Backstage using the apis-json/backstage integration tool for enterprise developer portal use. |
| Spectral | Spectral rulesets can validate APIs.json files against the specification schema and enforce organizational governance rules for API operations. |
| AsyncAPI | APIs.json supports AsyncAPI as a property type, allowing event-driven and message-based APIs to be documented alongside REST APIs in a single APIs.json file. |

## Artifacts

Machine-readable API specifications organized by format.

### Specification

- [APIs.json v0.19 Specification Text](spec/apisjson_0.19.txt)
- [APIs.json v0.18 Specification Text](spec/apisjson_0.18.txt)
- [APIs.json v0.17 Specification Text](spec/apisjson_0.17.txt)

### JSON Schema

- [Schema v0.20 (Draft)](json-schema/apis-json-schema-0.20.yaml)
- [Schema v0.19](json-schema/apis-json-schema-0.19.yaml)
- [Schema v0.18](json-schema/apis-json-schema-0.18.yaml)
- [Schema v0.17](json-schema/apis-json-schema-0.17.yaml)
- [Schema v0.19 (JSON)](json-schema/apis-json-schema-0.19.json)
- [Schema v0.18 (JSON)](json-schema/apis-json-schema-0.18.json)
- [Schema v0.17 (JSON)](json-schema/apis-json-schema-0.17.json)
- [Schema v0.20 (JSON)](json-schema/apis-json-schema-0.20.json)

### JSON Structure

- [Structure v0.19](json-structure/apis-json-structure-0.19-structure.json)
- [Structure v0.18](json-structure/apis-json-structure-0.18-structure.json)
- [Structure v0.17](json-structure/apis-json-structure-0.17-structure.json)
- [Structure v0.20](json-structure/apis-json-structure-0.20-structure.json)

### JSON-LD

- [APIs.json Context](json-ld/apis-json-context.jsonld)

### Examples

- [Minimal APIs.json Example](examples/apis-json-minimal-example.json)
- [Complete APIs.json Example](examples/apis-json-complete-example.json)

## Vocabulary

- [APIs.json Vocabulary](vocabulary/apis-json-vocabulary.yaml) — Normative vocabulary mapping 4 resources, 7 actions, 1 workflow, and 3 personas covering the APIs.json specification format, property type system, and conformance levels

## Rules

- [APIs.json Spectral Rules](rules/apis-json-spectral-rules.yml) — 40 rules across 8 categories enforcing APIs.json specification conformance at Minimal, Discoverable, Complete, and Production levels

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
