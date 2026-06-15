# RouterOS (routeros)

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
