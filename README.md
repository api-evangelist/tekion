# Tekion (tekion)

Tekion is a cloud-native, AI-native automotive retail platform. Its flagship **Automotive Retail Cloud (ARC)** is a modern dealer management system (DMS) spanning sales, service, parts, inventory, F&I, accounting, and CRM for franchise dealerships and OEMs. Tekion exposes its data and workflows to technology partners through the **Automotive Partner Cloud (APC)** — an open, OpenAPI-standard partner API program with REST APIs and webhooks that give approved partners near real-time access to a dealership's sales, service, inventory, and parts data.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tekion/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tekion/refs/heads/main/apis.yml)

## Access Model (Important)

The APC API is **partner-gated**. The technical API reference, credentials, and endpoints are only available after partner approval:

1. **Register** at [apc.tekioncloud.com/user/register](https://apc.tekioncloud.com/user/register) with minimal fields and legal-terms acceptance.
2. **Submit** a use case and select the APIs you need; applications are reviewed (typically within ~48 hours).
3. **Access** the API documentation dashboard, credentials, and endpoints once approved.

Access is **tiered**:

- **Standard** — foundational open APIs (near real-time sales, service, inventory, parts), webhooks, standard rate limits.
- **Enterprise (Elevated)** — additional APIs, higher rate limits, enhanced read/write and reference-data access.
- **Strategic (Premium)** — customized development, Premium APIs and API mapping, specialized workflows, and go-to-market support.

Dealers separately control which partners may access their data via the APC **Integration Hub**, and can track who accesses what.

Because the full technical reference is behind partner authentication, the APIs below are **honestly modeled by data domain** (`EndpointsModeled: true`) rather than transcribed from a public specification. No OpenAPI document, Postman collection, or concrete endpoint list was fabricated. Contact `APCintegrations@tekion.com` for partner enablement.

## Tags

- Automotive
- Dealership
- DMS
- Automotive Retail Cloud
- Partner API
- Sales
- Service
- Inventory
- Parts
- Webhooks
- Gated

## Timestamps

- **Created:** 2026-07-10
- **Modified:** 2026-07-10

## APIs (Modeled by Data Domain)

### Tekion Sales and Deals API

Near real-time access to a dealership's sales and deal data — deal jackets, desking, F&I products, and sold-vehicle records — through the Automotive Partner Cloud. Endpoints are published inside the gated APC dashboard after approval.

- **Human URL:** [https://tekion.com/products/apc](https://tekion.com/products/apc)
- **Base URL (representative):** `https://api.tekioncloud.com`

### Tekion Inventory API

New and used vehicle inventory — stock, VIN-level detail, pricing, and availability — exposed to approved partners via APC standard open APIs and webhooks.

- **Human URL:** [https://tekion.com/products/apc](https://tekion.com/products/apc)
- **Base URL (representative):** `https://api.tekioncloud.com`

### Tekion Service API

Fixed-operations and service data — repair orders, service appointments, labor operations, and status updates — available to approved partners through APC APIs and webhooks.

- **Human URL:** [https://tekion.com/products/apc](https://tekion.com/products/apc)
- **Base URL (representative):** `https://api.tekioncloud.com`

### Tekion Parts API

Parts inventory, catalog lookup, pricing, and ordering data (including electronic parts catalog / EPC integration) exposed to approved partners via APC.

- **Human URL:** [https://tekion.com/products/apc](https://tekion.com/products/apc)
- **Base URL (representative):** `https://api.tekioncloud.com`

### Tekion Customers API

Customer and CRM records — contact, ownership, and relationship data tied to sales and service activity — made available to approved partners through APC, subject to the dealer's data-sharing authorizations.

- **Human URL:** [https://tekion.com/products/apc](https://tekion.com/products/apc)
- **Base URL (representative):** `https://api.tekioncloud.com`

### Tekion Webhooks

Server-to-endpoint webhooks that keep partner systems in sync as dealership data changes across sales, service, inventory, and parts. Webhooks POST event payloads to a partner-registered HTTP endpoint (not a WebSocket).

- **Human URL:** [https://tekion.com/products/apc](https://tekion.com/products/apc)
- **Base URL (representative):** `https://api.tekioncloud.com`

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/tekion)
- [Website](https://tekion.com)
- [Documentation](https://tekion.com/products/apc)
- [Portal](https://apc.tekioncloud.com)
- [Sign Up](https://apc.tekioncloud.com/user/register)
- [Plans](plans/tekion-plans-pricing.yml)
- [Rate Limits](rate-limits/tekion-rate-limits.yml)
- [Fin Ops](finops/tekion-finops.yml)

## WebSocket Review

Tekion does **not** expose a documented public WebSocket API. APC delivers near real-time updates via REST APIs and webhooks (plus FTP feeds) — push-over-HTTP, not a bidirectional `wss://` transport. See [review.yml](review.yml).

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
