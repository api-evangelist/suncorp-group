# Suncorp Group (suncorp-group)

Suncorp Group Limited (ASX: SUN) is an Australian general insurance group headquartered in Brisbane, Queensland, serving customers across Australia and New Zealand. Following the sale of Suncorp Bank to ANZ on 31 July 2024 it operates as a pure-play insurer, underwriting personal lines (motor, home and contents, caravan, landlord) and commercial lines (SME packages, commercial motor and motor fleet, property/ISR, liability, professional and financial risks, workers' compensation, surety, and specialty lines including residential strata and equipment breakdown) through a portfolio of brands: in Australia AAMI, Apia, Bingle, CIL, GIO, Essentials by AAI, Shannons, Suncorp, Terri Scheer and Vero, and in New Zealand Vero and AA Insurance.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/suncorp-group/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/suncorp-group/refs/heads/main/apis.yml)

## Tags

- Insurance
- Australia
- Property and Casualty
- General Insurance
- Carrier
- Personal Lines
- Commercial Lines
- Claims
- Underwriting
- Broker
- Partner Gated
- New Zealand

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

None. Suncorp Group publishes **no public API**.

As of a 2026-07-25 review there is no first-party developer portal, no API reference, and no downloadable OpenAPI or Swagger definition on `suncorpgroup.com.au` or on any Suncorp brand domain.

- `developer.`, `developers.`, `docs.` and `api.suncorpgroup.com.au` do not resolve (DNS NXDOMAIN).
- `https://www.vero.com.au/developers`, `https://www.vero.com.au/api`, `https://www.suncorp.com.au/developers` and `https://www.suncorp.com.au/api` all return **HTTP 404**.
- The corporate sitemap (803 URLs) and the Suncorp, GIO, AAMI and Vero brand sitemaps (2,007 URLs combined) contain **zero** developer, API or integration paths.
- `developer.bingle.com.au` and `api.bingle.com.au` survive only as dangling CNAMEs to decommissioned AWS `ap-southeast-2` load balancers — no live host.

The only machine-to-machine integration surface is intermediated and behind a login:

- **VeroEdge / Vero Intermediary Portal** — [https://www.vero.com.au/secure/veroedge.html](https://www.vero.com.au/secure/veroedge.html) (HTTP 200), redirecting to an identity-provider login form at `https://online.verocentral.com.au/idp/channel/vero-portal`. Broker quote, bind, policy lifecycle, renewals and document access live here. Access is granted by a dedicated Vero Representative under the [Access Single ID (SID)](https://www.vero.com.au/terms-sid.html) terms.
- **Engineers PI & Strata Portal** — `https://EngineersPIandStrataPortal.vero.com.au/` (HTTP 200), a third-party "Uniwriter" underwriting application.
- **Broker Management System connections** — Vero's own [broker tools page](https://www.vero.com.au/broker/tools.html) states that the VeroEdge portal is for "brokers who don't access Vero Edge through their own Broker Management System," and Suncorp Group's 22 June 2026 newsroom release places new Vero products "via the Steadfast SCTP platform and Vero Underwriting portal … with future availability across Sunrise."

### ACORD posture

**No ACORD reference found.** Nothing on Suncorp Group or its brand properties mentions ACORD, AL3, ACORD XML, ACORD certification or NGDS. Australia's broker-to-insurer transaction seam is not ACORD/IVANS but the Steadfast Client Trading Platform (SCTP), Sunrise Exchange, and direct Broker Management System integration.

### Why the absence is the finding

Australia has the legal machinery for open insurance and no live obligation. The Consumer Data Right that already opened banking and energy was designated to extend to general insurance and then deferred, so no mandate produces a public product or quoting endpoint for a general insurer. The contrast is visible inside this same network: the sibling record [api-evangelist/suncorp-bank](https://github.com/api-evangelist/suncorp-bank) — the banking arm sold to ANZ in 2024 — does expose a live, unauthenticated CDR Product Reference Data API, because banking was mandated. Suncorp Group has none, because insurance was not.

## Common Properties

- [Website](https://www.suncorpgroup.com.au/)
- [About](https://www.suncorpgroup.com.au/about)
- [Brands](https://www.suncorpgroup.com.au/about/brands)
- [News](https://www.suncorpgroup.com.au/news/news)
- [Investor Centre](https://www.suncorpgroup.com.au/investors)
- [Partner Portal (VeroEdge)](https://www.vero.com.au/secure/veroedge.html)
- [Support](https://www.suncorpgroup.com.au/contact)
- [Privacy Policy](https://www.suncorpgroup.com.au/about/corporate-governance/privacy-policy)
- [Terms of Service](https://www.suncorpgroup.com.au/disclaimer)
- [Governance](https://www.suncorpgroup.com.au/about/corporate-governance)
- [GitHub Organization](https://github.com/SuncorpGroup)
- [LinkedIn](https://www.linkedin.com/company/suncorp/)

## Review

See [review.yml](review.yml) for the full 2026-07-25 API Evangelist reviewer finding, including every probe URL and HTTP status.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
