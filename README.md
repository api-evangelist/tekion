# Tekion (tekion)

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
