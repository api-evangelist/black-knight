# Black Knight (Acquired by ICE — Now ICE Mortgage Technology)

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

Black Knight, Inc. was a Jacksonville-based mortgage technology and data provider whose core franchises were:

- **MSP** — the dominant US loan-servicing platform
- **LoanSphere** — default management, document services (eClosing, eVault, eRecording), decisioning
- **Empower LOS** — mid-market loan origination
- **Optimal Blue** — secondary marketing, the industry's most-used product-and-pricing engine

**Intercontinental Exchange (NYSE: ICE) acquired Black Knight in September 2023 for ~$11.7B** (down from the originally-announced $13.1B in May 2022) after **divesting Optimal Blue to Constellation Software's Perseus Operating Group** as a condition of FTC clearance.

Today:

- `blackknightinc.com` 302-redirects to `mortgagetech.ice.com`
- Black Knight's product lines now sit inside ICE Mortgage Technology alongside Encompass (the ex-Ellie Mae LOS, acquired by ICE in 2020)
- Developer surfaces have migrated to `developer.ice.com` (MSP DX APIs, Servicing Vault, Loss Mitigation, Payoffs, Promise To Pay) and `developer.icemortgagetechnology.com` (Encompass Developer Connect)
- Optimal Blue APIs are now hosted at `digitalmarketplace.optimalblue.com` under independent Constellation Software ownership

This repo documents the API surfaces as they existed under Black Knight and tracks the post-acquisition fate of each product line.

## APIs Documented

| # | API | Status | Portal |
|---|---|---|---|
| 1 | MSP DX (Direct Exchange) APIs | Active under ICE | `developer.ice.com/mortgage-servicing/catalog` |
| 2 | Servicing Digital / Promise To Pay | Active under ICE | `developer.ice.com` |
| 3 | LoanSphere Default / Document / Decisioning | Folded into ICE — no public dev portal | `mortgagetech.ice.com` |
| 4 | Empower LOS | Coexists with Encompass — partner-gated | `mortgagetech.ice.com` |
| 5 | Encompass Developer Connect (sibling) | Active — primary LOS API surface under ICE | `developer.icemortgagetechnology.com/developer-connect` |
| 6 | Optimal Blue Product & Pricing (PPE) | **Divested to Constellation Sept 2023** | `digitalmarketplace.optimalblue.com` |
| 7 | Optimal Blue Loan Trading (Resitrader) | Under Constellation | `digitalmarketplace.optimalblue.com` |
| 8 | Optimal Blue Investor Solutions | Under Constellation | `digitalmarketplace.optimalblue.com` |
| 9 | Optimal Blue Business Intelligence (16 Rate Indices) | Under Constellation | `digitalmarketplace.optimalblue.com` |
| 10 | Optimal Blue Broker Pricing (Loansifter) | Under Constellation | `digitalmarketplace.optimalblue.com` |

## Artifacts

| Type | Folder | Files |
|---|---|---|
| JSON Schema | `json-schema/` | 6 (msp-loan, msp-escrow, msp-payment, servicing-promise-to-pay, optimal-blue-pricing, optimal-blue-lock) |
| JSON Structure | `json-structure/` | 1 (msp-loan) |
| JSON-LD Context | `json-ld/` | 1 (black-knight-context) — maps to FIBO + schema.org |
| Examples | `examples/` | 5 (msp-loan, msp-payment, promise-to-pay, optimal-blue-pricing, optimal-blue-lock) |
| Naftiko Capabilities | `capabilities/` | 3 (msp-dx, loan-servicing-workflow, optimal-blue-pricing) |
| Spectral Rules | `rules/` | 1 (black-knight-rules.yml) |
| Vocabulary | `vocabulary/` | 1 (black-knight-vocabulary.yml — 17 domain terms) |
| Plans / Pricing | `plans/` | 1 (4 commercial surfaces; all partner-gated, no public price card) |
| Rate Limits | `rate-limits/` | 1 (contractual; not publicly published) |
| FinOps | `finops/` | 1 (no FOCUS export; cost via enterprise invoice) |

## Absent / Not Public

- **No OpenAPI specs published.** MSP DX, Encompass Developer Connect, and Optimal Blue all gate spec access behind portal login or ISV onboarding. Public portals list catalog categories but not downloadable specs.
- **No public price card.** All four commercial surfaces (MSP, Encompass, Optimal Blue, Simplifile) use enterprise / partner contracts.
- **No public rate-limit numbers.** Optimal Blue advertises SLOs ("search request average < 1 sec", "millions of calls daily") but not per-key quotas.
- **No FOCUS-compatible FinOps export.** Cost reconciliation flows through PDF / EDI invoices.
- **EllieMae GitHub org has 0 public repos** — only the rebranded `ICEMortgageTechnology` org carries any sample code (6 small demo repos: exp19-exp21 series, api-best-practices).

## Acquisition Timeline

- **May 2022** — ICE announces agreement to acquire Black Knight for $13.1B
- **Sept 2023** — Deal closes at ~$11.7B; **Optimal Blue divested to Constellation Software / Perseus Operating Group** as FTC condition
- **2024–** — Black Knight brand sunset; products absorbed into ICE Mortgage Technology alongside Encompass (ex-Ellie Mae, 2020 acquisition)

## Index

The full index of APIs, properties, features, use cases, integrations, and references lives in [`apis.yml`](./apis.yml).
