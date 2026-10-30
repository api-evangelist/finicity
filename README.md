# Finicity

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

Finicity, LLC is a Utah-based financial-data aggregator and open-finance technology provider acquired by Mastercard in 2020 and now operating as Mastercard Open Banking (US) within Mastercard Open Finance. It is not a chartered bank but a consumer-permissioned data-access and decisioning platform (and an FCRA-regulated consumer reporting agency for its verification products), providing account and transaction aggregation, Verification of Assets, Income and Employment, transaction and cash-flow analysis, statements, and account validation for ACH payments. Finicity runs a first-party developer portal (developer.mastercard.com/open-banking-us, formerly developer.finicity.com and docs.finicity.com, both of which now redirect) over the live api.finicity.com host, is a founding participant in the Financial Data Exchange (FDX) with FDX-aligned data-sharing APIs, and positions its platform as an enabler of CFPB Section 1033 personal financial data rights. Public product documentation is openly reachable, but the full API reference and any machine-readable OpenAPI specification are partner-gated behind Mastercard Developers credentials.

**Areas:** Financial Services · Data Aggregation · Open Finance · Open Banking · FDX · United States · Payments · Financial Data

## Finicity on APIs.io

Everything profiled for Finicity is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/finicity/](https://apis.io/providers/finicity/)** — or go straight to one of the APIs or properties below.

### APIs (41)

- [Finicity Connect](https://apis.io/apis/finicity/finicity-connect/) — Hosted, embeddable account-linking experience that lets a consumer authenticate to their financial institution and permission data sharing, returning the…
- [Finicity Verification of Assets (VoA) API](https://apis.io/apis/finicity/finicity-verification-of-assets-api/) — Generates a consumer-permissioned Verification of Assets report from aggregated account and balance data for mortgage, lending and underwriting workflows,…
- [Finicity Verification of Income & Employment (VoIE) API](https://apis.io/apis/finicity/finicity-verification-of-income-employment-api/) — Derives income streams and employment signals from permissioned transaction and payroll data to produce Verification of Income and Verification of…
- [Finicity Transaction Analysis (Cash Flow) API](https://apis.io/apis/finicity/finicity-transaction-analysis-api/) — Analyzes permissioned transaction history to produce cash-flow, income and expense insights used for prequalification, credit decisioning and…
- [Finicity Payments (Account Validation) API](https://apis.io/apis/finicity/finicity-payments-account-validation-api/) — Validates account ownership and status for ACH and account-funding flows, returning account, routing and owner verification signals to reduce returned…
- [Finicity Open Banking Data Access (FDX)](https://apis.io/apis/finicity/finicity-open-banking-data-access/) — FDX-aligned, consumer-permissioned open-banking data-access surface through which Finicity, as a founding Financial Data Exchange participant, shares…
- [Finicity Account Validation Assistance API](https://apis.io/apis/finicity/finicity-account-validation-assistance-api/) — Micro entries and account verification
- [Finicity Accounts API](https://apis.io/apis/finicity/finicity-accounts-api/) — Fetch or refresh customer accounts
- [Finicity Accounts (Simple) API](https://apis.io/apis/finicity/finicity-accounts-simple-api/) — Fetch simple customer accounts
- [Finicity App Registration API](https://apis.io/apis/finicity/finicity-app-registration-api/) — Register and assign apps to customers
- [Finicity Authentication API](https://apis.io/apis/finicity/finicity-authentication-api/) — Generate authentication tokens and manage credentials
- [Finicity Balance Analytics API](https://apis.io/apis/finicity/finicity-balance-analytics-api/) — Balance Analytics for businesses
- [Finicity Bank Statements API](https://apis.io/apis/finicity/finicity-bank-statements-api/) — Fetch account statements and generate reports asynchronously
- [Finicity Businesses API](https://apis.io/apis/finicity/finicity-businesses-api-api/) — Create and manage business associated with customers in order to use Balance Analytics or Cash Flow Analytics
- [Finicity Cash Flow Analytics API](https://apis.io/apis/finicity/finicity-cash-flow-analytics-api/) — Cash Flow Analytics for business
- [Finicity Cash Flow API](https://apis.io/apis/finicity/finicity-cash-flow-api/) — Generate cash flow reports asynchronously
- [Finicity Connect API](https://apis.io/apis/finicity/finicity-connect-api/) — Allow customers to log into their financial institutions and grant Finicity authorization
- [Finicity Connect Components API](https://apis.io/apis/finicity/finicity-connect-components-api/) — Allow customers to log into their financial institutions and grant Finicity authorization
- [Finicity Consumer Foresight API](https://apis.io/apis/finicity/finicity-consumer-foresight-api/) — Generate consumer foresight analytics reports
- [Finicity Consumers API](https://apis.io/apis/finicity/finicity-consumers-api/) — Create and manage consumers associated with customers in order to use report services
- [Finicity Customer Authorization Details API](https://apis.io/apis/finicity/finicity-customer-authorization-details-api/) — APIs to retrieve customer authorization details
- [Finicity Customers API](https://apis.io/apis/finicity/finicity-customers-api/) — Enroll and manage customers
- [Finicity Data Sharing Consent API](https://apis.io/apis/finicity/finicity-data-sharing-consent-api/) — Manage data sharing consents
- [Finicity Identity API](https://apis.io/apis/finicity/finicity-identity-api/) — Match the request details to the Institution account holder details
- [Finicity Institutions API](https://apis.io/apis/finicity/finicity-institutions-api/) — Search and fetch financial institutions
- [Finicity Pay Statements API](https://apis.io/apis/finicity/finicity-pay-statements-api/) — Upload pay statements
- [Finicity Payment Enablement Bundle API](https://apis.io/apis/finicity/finicity-payment-enablement-bundle-api/) — Any or all of the Payments endpoints in one API call
- [Finicity Payment History Report API](https://apis.io/apis/finicity/finicity-payment-history-report-api/) — Payment History Report for business
- [Finicity Payment Success Indicator API](https://apis.io/apis/finicity/finicity-payment-success-indicator-api/) — Predict a transaction's likelihood to settle
- [Finicity Payments API](https://apis.io/apis/finicity/finicity-payments-api/) — Fetch ACH details and account balances
- [Finicity Portfolios API](https://apis.io/apis/finicity/finicity-portfolios-api/) — Generate portfolios of the most recent reports
- [Finicity Reports API](https://apis.io/apis/finicity/finicity-reports-api/) — Fetch generated reports when ready
- [Finicity Small Business Credit Analytics API](https://apis.io/apis/finicity/finicity-small-business-credit-analytics-api/) — Fetch merchant location matches and generate reports
- [Finicity Third Party Access API](https://apis.io/apis/finicity/finicity-third-party-access-api/) — Generate and manage access keys for other partners
- [Finicity Transaction Data Enrichment API](https://apis.io/apis/finicity/finicity-transaction-data-enrichment-api/) — Enhance the transaction data set
- [Finicity Transactions API](https://apis.io/apis/finicity/finicity-transactions-api/) — Fetch customer and account transactions and generate reports asynchronously
- [Finicity Transfer API](https://apis.io/apis/finicity/finicity-transfer-api/) — Fetch details of the deposit and bill pay switches
- [Finicity Tx Push API](https://apis.io/apis/finicity/finicity-txpush-api/) — Manage TxPush subscriptions
- [Finicity Verify Assets API](https://apis.io/apis/finicity/finicity-verify-assets-api/) — Generate asset reports asynchronously
- [Finicity Verify Income and Employment API](https://apis.io/apis/finicity/finicity-verify-income-and-employment-api/) — Generate income and employment reports asynchronously
- [Finicity Webhook Subscription API](https://apis.io/apis/finicity/finicity-webhook-subscription-api/) — APIs for Managing Partner Webhook Event Subscriptions

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Finicity Webhooks](https://apis.io/asyncapis/finicity/finicity-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [finicity](https://apis.io/servers/finicity/finicity/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Finicity Openbanking Us Overlay](https://apis.io/overlays/finicity/finicity-openbanking-us-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Finicity Authentication](https://apis.io/security/finicity/finicity-authentication/)
- [Finicity Domain Security](https://apis.io/security/finicity/finicity-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.finicity.com/)
- [Documentation](https://developer.mastercard.com/open-banking-us/documentation/)
- [Getting started](https://developer.mastercard.com/open-banking-us/documentation/test-the-apis/)
- [API reference](https://developer.mastercard.com/open-banking-us/documentation/api-reference/)
- [Sign up](https://developer.mastercard.com/product/open-banking/)
- [Support](https://developer.mastercard.com/support/)
- [GitHub](https://github.com/Mastercard)
- [Status](https://developer.mastercard.com/open-banking-us/documentation/status/)

## API Evangelist rating

**Kin Score 47.2** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 59.9 |
| Contract governance | 4.5 |
| Operational transparency | 50.0 |
| Developer ergonomics | 75.6 |
| Access clarity | 13.2 |

**Agent readiness 22.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 26.0** — Banking & Open Finance

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/finicity/](https://apis.io/providers/finicity/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Finicity: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/finicity/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
