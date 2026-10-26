# Cuboh (cuboh)

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

Cuboh is a restaurant online-ordering management platform that consolidates third-party delivery and pickup orders (DoorDash, Uber Eats, Grubhub, and more) onto a single tablet and into the restaurant POS. For technology partners, Cuboh exposes partner-gated Direct and Connect integration APIs covering orders, menus, merchant locations, and webhooks. API access is provisioned by Cuboh during a partner onboarding and QA-certification process; there is no public self-serve signup.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cuboh/refs/heads/main/apis.yml)

## Tags

- Restaurant
- Online Ordering
- Delivery
- POS
- Order Aggregation

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Cuboh Orders API

Partner-gated order lifecycle integration. Create orders, list orders, retrieve a single order, and cancel orders or order groups under the Direct API, plus accept, complete, refund, upcharge, and cancel actions under the Connect API. Order events are delivered to partner webhook URLs.

- **Human URL:** [https://docs.cuboh.com/direct](https://docs.cuboh.com/direct)
- **Base URL:** `https://core.cuboh.net`

#### Tags

- Orders
- Delivery
- Pickup

#### Properties

- [Documentation](https://docs.cuboh.com/direct)
- [API Reference](https://docs.cuboh.com/connect)
- [OpenAPI](openapi/cuboh-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cuboh.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cuboh.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cuboh Menu API

Partner-gated menu management. Retrieve, push, create, update, and validate merchant menus, and update item and modifier availability status, so that menus stay synchronized between Cuboh and the partner platform.

- **Human URL:** [https://docs.cuboh.com/direct](https://docs.cuboh.com/direct)
- **Base URL:** `https://core.cuboh.net`

#### Tags

- Menu
- Catalog
- Synchronization

#### Properties

- [Documentation](https://docs.cuboh.com/direct)
- [API Reference](https://docs.cuboh.com/connect)
- [OpenAPI](openapi/cuboh-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cuboh.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cuboh.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cuboh Merchant Locations API

Partner-gated merchant (location) integration. Report merchant status, complete a merchant integration, and retrieve orders for a merchant identified by its external integration merchant UUID.

- **Human URL:** [https://docs.cuboh.com/direct](https://docs.cuboh.com/direct)
- **Base URL:** `https://core.cuboh.net`

#### Tags

- Locations
- Merchants
- Stores

#### Properties

- [Documentation](https://docs.cuboh.com/direct)
- [API Reference](https://docs.cuboh.com/connect)
- [OpenAPI](openapi/cuboh-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cuboh.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cuboh.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cuboh Webhooks API

Cuboh sends signed webhook events to partner-hosted URLs for order actions (accept, complete, cancel, adjust), merchant integration and status changes, and menu updates. Each event is signed with an X-Cuboh-Signature HMAC-SHA256 header and retried with exponential backoff on failure.

- **Human URL:** [https://docs.cuboh.com/direct](https://docs.cuboh.com/direct)
- **Base URL:** `https://core.cuboh.net`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.cuboh.com/direct)
- [API Reference](https://docs.cuboh.com/connect)
- [OpenAPI](openapi/cuboh-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cuboh.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cuboh.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/getcuboh)
- [Website](https://www.cuboh.com/)
- [Documentation](https://docs.cuboh.com/direct)
- [Plans](plans/cuboh-plans-pricing.yml)
- [Rate Limits](rate-limits/cuboh-rate-limits.yml)
- [Fin Ops](finops/cuboh-finops.yml)

## API Availability

Cuboh's Direct (v2.0) and Connect (v0.1) APIs are real and documented, but they are partner-gated. There is no self-serve signup or public key issuance; Cuboh provisions an integration token to approved technology partners through onboarding and QA certification (contact integrations@cuboh.com). The published pricing on cuboh.com is for the restaurant SaaS subscription, not for API access. See [review.yml](review.yml) for the full availability assessment.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
