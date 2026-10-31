# OPay

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

OPay is a Nigerian mobile money and fintech super-app operated by Blue Ridge Microfinance Bank (OPay Digital Services Limited) and majority-owned by Opera Limited with backing from SoftBank Vision Fund 2, Sequoia China, DragonBall Capital, and 9F Group. Launched in 2018 and headquartered in Lagos, OPay serves tens of millions of Nigerian consumers, merchants, and agents with wallet accounts, free interbank transfers, the OPay Debit Card, OWealth (daily-interest savings powered by OPay Microfinance Bank), bill payments, airtime/data top-ups, BNPL (OBuy / OPay Easy Buy), and the OPay POS / agent banking network. For developers and merchants, OPay exposes the OPay Cashier / OPay Checkout API — a REST API for accepting payments via 3DS bank cards, bank transfer, USSD, bank account, POS, OPay wallet QR, and reference codes, with hosted Express Checkout, server-to-server APIs, callback webhooks, refund and query operations, a PHP gateway SDK, and a WooCommerce plugin. Sandbox and production environments are available at testapi.opaycheckout.com and liveapi.opaycheckout.com, with HMAC-SHA512 signature authentication and per-merchant public/private key pairs issued from the OPay merchant dashboard.

**Areas:** Payments · Mobile Money · Fintech · Super App · Nigeria · Africa · Wallets · Savings · Buy Now Pay Later · Bank Transfers · Card Payments · USSD

## OPay on APIs.io

Everything profiled for OPay is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/opay/](https://apis.io/providers/opay/)** — or go straight to one of the APIs or properties below.

### APIs (3)

- [OPay Cashier API](https://apis.io/apis/opay/opay-cashier-api/) — The OPay Cashier API is the primary merchant payment API behind OPay Checkout. It exposes a hosted Express Checkout endpoint (cashier/create returning a…
- [OPay Payments API](https://apis.io/apis/opay/opay-payments-api/) — Server-to-server payment creation across payment methods.
- [OPay Refunds API](https://apis.io/apis/opay/opay-refunds-api/) — Refund creation and status.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Opay Agentic Access](https://apis.io/agentic-access/opay/opay-agentic-access/)

#### Collections (3)

Postman and Open Collection request collections.

- [OPay Cashier API](https://apis.io/collections/opay/open-opay-cashier-api/)
- [OPay Cashier Payments API](https://apis.io/collections/opay/open-opay-payments-api/)
- [OPay Cashier Refunds API](https://apis.io/collections/opay/open-opay-refunds-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Opay Authentication](https://apis.io/security/opay/opay-authentication/)
- [Opay Domain Security](https://apis.io/security/opay/opay-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.opayweb.com/)
- [Documentation](https://documentation.opaycheckout.com/)
- [Getting started](https://documentation.opaycheckout.com/getting-started)
- [API reference](https://documentation.opaycheckout.com/server-apis-overview)
- [Support](https://support.opaycheckout.com/support/ticket)
- [Blog](https://www.opayweb.com/newsroom/)
- [Terms of service](https://www.opayweb.com/terms-and-conditions)
- [Privacy policy](https://www.opayweb.com/privacy-policy)
- [GitHub](https://github.com/opay)

## API Evangelist rating

**Kin Score 33.0** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 50.1 |
| Contract governance | 0.0 |
| Operational transparency | 2.6 |
| Developer ergonomics | 61.9 |
| Access clarity | 13.2 |

**Agent readiness 25.8** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | unknown |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 10.7** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/opay/](https://apis.io/providers/opay/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for OPay: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/opay/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
