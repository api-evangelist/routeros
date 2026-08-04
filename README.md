# RouterOS (routeros)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

RouterOS is MikroTik's powerful network operating system designed for managing routers, switches, access points, and other network devices. It provides a comprehensive REST API (v7.1+) and a TCP-based binary API for programmatic management of IP addresses, interfaces, firewall rules, routing, VPN configurations, DHCP, DNS, and system resources. RouterOS powers MikroTik hardware and can also be deployed as a virtual machine (CHR).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Networking
- Routers
- Network Management
- Firewall
- MikroTik

## Timestamps

- **Created:** 2024-11-07
- **Modified:** 2026-05-19

## APIs

### RouterOS REST API

The RouterOS REST API is a JSON wrapper over the RouterOS console API, available from RouterOS v7.1beta4+. It enables create, read, update, and delete operations on all RouterOS configuration menus via standard HTTP methods (GET, PUT, PATCH, DELETE, POST). Authentication uses HTTP Basic Auth with console credentials. Supports filtering, property selection (.proplist), and complex queries. Accessible at https://{router-ip}/rest.

- **Human URL:** [https://help.mikrotik.com/docs/spaces/ROS/pages/47579162/REST+API](https://help.mikrotik.com/docs/spaces/ROS/pages/47579162/REST+API)
- **Base URL:** `https://{router-ip}/rest`

#### Tags

- Networking
- Router Management
- REST API
- Network Configuration
- Firewall
- DHCP
- DNS

#### Properties

- [Documentation](https://help.mikrotik.com/docs/spaces/ROS/pages/47579162/REST+API)
- [Documentation](https://help.mikrotik.com/docs/spaces/ROS/pages/47579160/API)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-rest-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Spectral Rules](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/rules/routeros-rules.yml)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/json-schema/routeros-ip-address-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/json-schema/routeros-interface-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/json-schema/routeros-firewall-filter-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/json-structure/routeros-ip-address-structure.json)
- [J S O N L D Context](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/json-ld/routeros-context.jsonld)
- [Example](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/examples/routeros-list-ip-addresses-example.json)
- [Example](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/examples/routeros-list-firewall-filters-example.json)
- [Example](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/examples/routeros-get-system-resource-example.json)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/vocabulary/routeros-vocabulary.yml)
- [Postman Collection](collections/routeros-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/routeros-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### RouterOS TCP API

The RouterOS TCP API is the native binary protocol for RouterOS, running on TCP port 8728 (standard) and TCP port 8729 (SSL/TLS). It uses a sentence-based word protocol with variable-length encoding, supporting tagged concurrent commands, streaming changes via /listen, and cancellation. Used by most RouterOS client libraries (Python, PHP, Java, Go, etc.).

- **Human URL:** [https://help.mikrotik.com/docs/spaces/ROS/pages/47579160/API](https://help.mikrotik.com/docs/spaces/ROS/pages/47579160/API)
- **Base URL:** `tcp://{router-ip}:8728`

#### Tags

- Networking
- Router Management
- TCP API
- Binary Protocol

#### Properties

- [Documentation](https://help.mikrotik.com/docs/spaces/ROS/pages/47579160/API)
- [Documentation](https://wiki.mikrotik.com/wiki/Manual:API)
- [Postman Collection](collections/routeros-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/routeros-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://mikrotik.com)
- [Documentation](https://help.mikrotik.com/docs/spaces/ROS)
- [Git Hub Org](https://github.com/mikrotik)
- [Forum](https://forum.mikrotik.com)
- [Wiki](https://wiki.mikrotik.com)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/vocabulary/routeros-vocabulary.yml)
- [J S O N L D Context](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/json-ld/routeros-context.jsonld)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
