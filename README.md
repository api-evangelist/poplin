# Poplin (poplin)

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
