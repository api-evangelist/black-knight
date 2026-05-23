# Black Knight (Acquired by ICE — Now ICE Mortgage Technology)

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
