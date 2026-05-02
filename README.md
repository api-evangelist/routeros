# RouterOS

RouterOS is MikroTik's powerful network operating system designed for managing routers, switches, access points, and other network devices. It provides a comprehensive REST API (v7.1+) and a TCP-based binary API for programmatic management of IP addresses, interfaces, firewall rules, routing, VPN configurations, DHCP, DNS, and system resources. RouterOS powers MikroTik hardware and can also be deployed as a virtual machine (CHR).

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Networking, Routers, Network Management, Firewall, MikroTik

## Timestamps

- **Created:** 2024-11-07
- **Modified:** 2026-05-02

## APIs

### RouterOS REST API
The RouterOS REST API is a JSON wrapper over the RouterOS console API, available from RouterOS v7.1beta4+. It enables CRUD operations on all router configuration menus via HTTP methods. Accessible at `https://{router-ip}/rest`.

**Human URL:** [https://help.mikrotik.com/docs/spaces/ROS/pages/47579162/REST+API](https://help.mikrotik.com/docs/spaces/ROS/pages/47579162/REST+API)

#### Tags

- Networking, Router Management, REST API, Network Configuration, Firewall, DHCP, DNS

#### Properties

- [Documentation](https://help.mikrotik.com/docs/spaces/ROS/pages/47579162/REST+API)
- [Documentation](https://help.mikrotik.com/docs/spaces/ROS/pages/47579160/API)
- [OpenAPI](openapi/routeros-rest-api-openapi.yml)
- [SpectralRules](rules/routeros-rules.yml)
- [NaftikoCapabilities](capabilities/network-management.yaml)
- [JSONSchema](json-schema/routeros-ip-address-schema.json)
- [JSONSchema](json-schema/routeros-interface-schema.json)
- [JSONSchema](json-schema/routeros-firewall-filter-schema.json)
- [JSONStructure](json-structure/routeros-ip-address-structure.json)
- [JSONLDContext](json-ld/routeros-context.jsonld)
- [Example](examples/routeros-list-ip-addresses-example.json)
- [Example](examples/routeros-list-firewall-filters-example.json)
- [Example](examples/routeros-get-system-resource-example.json)
- [Vocabulary](vocabulary/routeros-vocabulary.yml)

### RouterOS TCP API
The RouterOS TCP API is the native binary protocol running on TCP:8728 (standard) and TCP:8729 (SSL). Sentence-based word protocol supporting tagged concurrent commands, streaming, and cancellation.

**Human URL:** [https://help.mikrotik.com/docs/spaces/ROS/pages/47579160/API](https://help.mikrotik.com/docs/spaces/ROS/pages/47579160/API)

#### Tags

- Networking, Router Management, TCP API, Binary Protocol

#### Properties

- [Documentation](https://help.mikrotik.com/docs/spaces/ROS/pages/47579160/API)
- [Documentation](https://wiki.mikrotik.com/wiki/Manual:API)

## Artifacts

### OpenAPI Specifications

| File | Description |
|---|---|
| [routeros-rest-api-openapi.yml](openapi/routeros-rest-api-openapi.yml) | RouterOS REST API — IP, interfaces, firewall, routing, system, DHCP, DNS, wireless |

### Spectral Rules

| File | Description |
|---|---|
| [routeros-rules.yml](rules/routeros-rules.yml) | Spectral ruleset enforcing RouterOS API conventions |

### Capabilities

| File | Description |
|---|---|
| [network-management.yaml](capabilities/network-management.yaml) | Unified network management workflow — IP, firewall, routing, DHCP, DNS, wireless (14 tools) |
| [shared/routeros-rest.yaml](capabilities/shared/routeros-rest.yaml) | Shared per-API definition for RouterOS REST API |

### JSON Schema

| File | Description |
|---|---|
| [routeros-ip-address-schema.json](json-schema/routeros-ip-address-schema.json) | IP address resource schema |
| [routeros-interface-schema.json](json-schema/routeros-interface-schema.json) | Network interface resource schema |
| [routeros-firewall-filter-schema.json](json-schema/routeros-firewall-filter-schema.json) | Firewall filter rule schema |

### JSON Structure

| File | Description |
|---|---|
| [routeros-ip-address-structure.json](json-structure/routeros-ip-address-structure.json) | IP address field documentation |

### JSON-LD

| File | Description |
|---|---|
| [routeros-context.jsonld](json-ld/routeros-context.jsonld) | JSON-LD context mapping RouterOS vocabulary to schema.org |

### Examples

| File | Description |
|---|---|
| [routeros-list-ip-addresses-example.json](examples/routeros-list-ip-addresses-example.json) | List IP addresses request/response |
| [routeros-list-firewall-filters-example.json](examples/routeros-list-firewall-filters-example.json) | List firewall filter rules request/response |
| [routeros-get-system-resource-example.json](examples/routeros-get-system-resource-example.json) | Get system resources request/response |

### Vocabulary

| File | Description |
|---|---|
| [routeros-vocabulary.yml](vocabulary/routeros-vocabulary.yml) | RouterOS domain terminology — interfaces, firewall, routing, VPN, API |

## Resources

- **Website:** https://mikrotik.com
- **Documentation:** https://help.mikrotik.com/docs/spaces/ROS
- **GitHub:** https://github.com/mikrotik
- **Forum:** https://forum.mikrotik.com
- **Wiki:** https://wiki.mikrotik.com

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
