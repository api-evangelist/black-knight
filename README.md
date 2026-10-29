# Black Knight

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

Black Knight, Inc. was a Jacksonville-based mortgage technology and data provider whose core franchises were MSP (the dominant US loan-servicing platform), LoanSphere (default, document, and decisioning suites), Empower LOS (mid-market loan origination), and the Optimal Blue secondary marketing / product-and-pricing engine. Intercontinental Exchange (NYSE: ICE) acquired Black Knight in September 2023 for approximately $11.7B (down from the originally-announced $13.1B in May 2022) after divesting Optimal Blue to Constellation Software's Perseus Operating Group as a condition of FTC clearance. Black Knight's product lines now sit inside ICE Mortgage Technology alongside Encompass (the ex-Ellie Mae LOS). The blackknightinc.com domain redirects to mortgagetech.ice.com, and developer surfaces have migrated to developer.ice.com (MSP DX APIs, Servicing Vault, Loss Mitigation, Payoffs, Promise To Pay) and developer.icemortgagetechnology.com (Encompass Developer Connect). Optimal Blue's APIs are now hosted at digitalmarketplace.optimalblue.com under independent Constellation Software ownership. This profile documents the API surfaces as they existed under Black Knight and tracks the post-acquisition fate of each product line.

**Areas:** Mortgage · Loan Servicing · Loan Origination · Secondary Marketing · Default Management · Investor Reporting · Product Pricing Engine · Real Estate Data · Fintech · Acquired Company · ICE Mortgage Technology

## Black Knight on APIs.io

Everything profiled for Black Knight is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/black-knight/](https://apis.io/providers/black-knight/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [MSP DX (Direct Exchange) APIs](https://apis.io/apis/black-knight/msp-dx/) — MSP (Mortgage Servicing Platform) was Black Knight's flagship product — the mainframe-rooted system of record that services the majority of US…
- [Servicing Digital / Promise To Pay APIs](https://apis.io/apis/black-knight/servicing-digital/) — Borrower-facing servicing capabilities including the Promise To Pay API, which enables clients to document borrower payment promises along with reason…
- [LoanSphere Default, Document & Decisioning Suite](https://apis.io/apis/black-knight/loansphere/) — LoanSphere was Black Knight's umbrella brand for default management (foreclosure, bankruptcy, loss-mitigation case management), document services (eClosing,…
- [Empower LOS APIs](https://apis.io/apis/black-knight/empower-los/) — Empower was Black Knight's mid-to-enterprise loan origination system. After the ICE acquisition, Empower coexists with ICE's larger Encompass LOS (from the…
- [Encompass Developer Connect (sibling product under ICE)](https://apis.io/apis/black-knight/encompass-developer-connect/) — Although Encompass came to ICE via the 2020 Ellie Mae acquisition (not Black Knight), it is now the canonical LOS API surface under ICE Mortgage Technology…
- [Optimal Blue Product & Pricing APIs (divested to Constellation)](https://apis.io/apis/black-knight/optimal-blue-ppe/) — Optimal Blue's Product & Pricing Engine (PPE) generates eligible products and pricing for any user in any format and automates loan creation, locking,…
- [Optimal Blue Loan Trading APIs (Resitrader)](https://apis.io/apis/black-knight/optimal-blue-trading/) — Workflow and data APIs for the Resitrader loan-trading application — execute trades, manage data modules, centralize trading operations. Now operated by…
- [Optimal Blue Business Intelligence APIs](https://apis.io/apis/black-knight/optimal-blue-business-intelligence/) — Data tools including 16 Mortgage Market Rate Indices, integrable into dashboards. Successor to Black Knight's Originations Market Monitor and Mortgage…
- [Optimal Blue Broker Pricing APIs (Loansifter)](https://apis.io/apis/black-knight/optimal-blue-broker-pricing/) — Loansifter is the turnkey PPE for mortgage brokers — generate and display eligible products and pricing across borrower scenarios. Originally a Black Knight…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### JSON Schema (6)

The data models the API reads and writes.

- [MSP Escrow Item](https://apis.io/schemas/black-knight/msp-escrow/)
- [MSP Loan](https://apis.io/schemas/black-knight/msp-loan/)
- [MSP Payment](https://apis.io/schemas/black-knight/msp-payment/)
- [Optimal Blue Rate Lock](https://apis.io/schemas/black-knight/optimal-blue-lock/)
- [Optimal Blue Pricing Search Result](https://apis.io/schemas/black-knight/optimal-blue-pricing/)
- [Promise To Pay](https://apis.io/schemas/black-knight/servicing-promise-to-pay/)

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Msp Loan Structure](https://apis.io/json-structure/black-knight/msp-loan-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Black Knight Context](https://apis.io/jsonld/black-knight/black-knight-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Black Knight / ICE Mortgage Technology Vocabulary](https://apis.io/vocabularies/black-knight/black-knight-vocabulary/)

#### Examples (5)

Example requests and responses.

- [Msp Loan Example](https://apis.io/examples/black-knight/msp-loan-example/)
- [Msp Payment Example](https://apis.io/examples/black-knight/msp-payment-example/)
- [Optimal Blue Lock Example](https://apis.io/examples/black-knight/optimal-blue-lock-example/)
- [Optimal Blue Pricing Example](https://apis.io/examples/black-knight/optimal-blue-pricing-example/)
- [Servicing Promise To Pay Example](https://apis.io/examples/black-knight/servicing-promise-to-pay-example/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Black Knight — jsonschema rules](https://apis.io/rules/black-knight/black-knight-jsonschema-spectral-rules/)
- [Black Knight API Rules](https://apis.io/rules/black-knight/black-knight-rules/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Black Knight Domain Security](https://apis.io/security/black-knight/black-knight-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Black Knight Plans Pricing](https://apis.io/plans/black-knight/black-knight-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Black Knight Rate Limits](https://apis.io/rate-limits/black-knight/black-knight-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Black Knight Finops](https://apis.io/finops/black-knight/black-knight-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://mortgagetech.ice.com)
- [Blog](https://mortgagetech.ice.com/blog)
- [GitHub](https://github.com/ICEMortgageTechnology)

## API Evangelist rating

**Kin Score 28.8** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 57.1 |
| Contract quality | 33.2 |
| Contract governance | 27.3 |
| Operational transparency | 10.5 |
| Developer ergonomics | 41.7 |
| Access clarity | 7.9 |

**Agent readiness 4.4** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/black-knight/](https://apis.io/providers/black-knight/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Black Knight: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/black-knight/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
