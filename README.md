# Poplin (poplin)

Poplin (formerly SudShare) is a nationwide on-demand laundry pickup and delivery marketplace connecting customers with independent, work-from-home "Laundry Pros" who wash, dry, and fold laundry, serving 500+ cities and 150,000+ customers. Poplin operates two consumer-facing mobile apps - the customer app and the Laundry Pro app - plus a Laundry Pro web portal (laundry-pro.poplin.co), but it does not expose a public or partner developer API. No developer portal or API reference was found at poplin.co, and the api.poplin.co subdomain resolves but returns a bare 404 with no documentation, indicating internal-only use. Business/SMB accounts (property managers, hospitality) are onboarded through sales and an account manager rather than through self-service API keys.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/poplin/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/poplin/refs/heads/main/apis.yml)

## Access Model

Poplin has **no public, self-service developer API**. This entry documents that finding honestly rather than modeling endpoints that don't exist:

- No `developer.poplin.co`, `developers.poplin.co`, `docs.poplin.co`, or `partners.poplin.co` subdomain resolves.
- `api.poplin.co` resolves but returns a bare HTTP 404 with no documentation - consistent with an internal backend host for Poplin's own consumer and Laundry Pro apps, not a public API surface.
- The [Poplin Business](https://poplin.co/business) page (SMB / property-management / hospitality laundry) describes account-manager-led onboarding and a mobile app for ordering and tracking; it makes no mention of an API, webhook, or SDK.
- All customer ordering, Laundry Pro job matching/acceptance, scheduling, and payment happen inside Poplin's own first-party apps.

## Tags

- Laundry
- On-Demand
- Gig Economy
- Marketplace
- Delivery
- Consumer

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### Poplin API

Poplin does not expose a public, self-service API. Ordering, scheduling, Laundry Pro matching, pricing, and payment all flow through Poplin's own customer and Laundry Pro mobile apps rather than open developer endpoints. The api.poplin.co host resolves but serves no public documentation (bare 404 as of the profiling date), and no developer.poplin.co, developers.poplin.co, docs.poplin.co, or partners.poplin.co subdomain resolves at all. Any business integration (SMB / property-management accounts) is negotiated manually through sales and an account manager, not through a published API.

- **Human URL:** [https://poplin.co/about](https://poplin.co/about)

#### Tags

- Laundry
- On-Demand
- Gig Economy

#### Properties

- [x-status](https://poplin.co/about) — No public developer portal or open API documentation as of 2026-07-03; api.poplin.co returns a bare 404.

## Pricing (Consumer Service, Not API)

Poplin charges consumers per pound of laundry rather than metering any API:

- **Standard (next-day):** $1/lb in most zip codes (higher in some markets); $30 typical minimum.
- **Express (same-day/overnight):** $2/lb in most zip codes (higher in some markets); $40 typical minimum.
- **Pickup and delivery:** free.
- **Oversized items** (e.g. comforters): +$8 per item, in addition to per-pound cost.

See [plans/poplin-plans-pricing.yml](plans/poplin-plans-pricing.yml) for the full sourced breakdown, including the two-sided marketplace economics between customers and Laundry Pros.

## Common Properties

- [Website](https://poplin.co)
- [LinkedIn](https://www.linkedin.com/company/poplin-co)
- [Laundry Pro Portal](https://laundry-pro.poplin.co)
- [Help Center](https://poplin.zendesk.com/hc/en-us)
- [Business](https://poplin.co/business)
- [Plans](plans/poplin-plans-pricing.yml)
- [Rate Limits](rate-limits/poplin-rate-limits.yml)
- [Fin Ops](finops/poplin-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
