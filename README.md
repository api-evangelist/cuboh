# Cuboh (cuboh)

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
