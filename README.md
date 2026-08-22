# Finicity (finicity)

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

Finicity, LLC is a Utah-based financial-data aggregator and open-finance technology provider acquired by Mastercard in 2020 and now operating as Mastercard Open Banking (US) within Mastercard Open Finance. It is not a chartered bank but a consumer-permissioned data-access and decisioning platform — and an FCRA-regulated consumer reporting agency for its verification products — providing account and transaction aggregation, Verification of Assets/Income/Employment, transaction and cash-flow analysis, statements, and account validation for ACH payments. Finicity is a founding participant in the Financial Data Exchange (FDX), ships FDX-aligned data-sharing APIs, and positions its platform as an enabler of CFPB Section 1033 personal financial data rights.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/finicity/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/finicity/refs/heads/main/apis.yml)

## Open-Finance / API Posture

- **First-party developer portal (confirmed live):** [https://developer.mastercard.com/open-banking-us/documentation/](https://developer.mastercard.com/open-banking-us/documentation/) — HTTP 200. The legacy Finicity developer surfaces `developer.finicity.com` and `docs.finicity.com` both now redirect here.
- **API host (confirmed live):** `https://api.finicity.com` — HTTP 401 (auth-gated; real production host).
- **Authentication:** Finicity partner authentication — an application `Finicity-App-Key` plus Partner ID and Partner Secret are exchanged for a `Finicity-App-Token`, with consumer permissioning captured through Finicity Connect.
- **OpenAPI / spec provenance:** No machine-readable OpenAPI/Swagger specification is publicly downloadable. The documentation landing page is public, but the full API reference and any specification are partner-gated behind Mastercard Developers credentials. No spec was harvested.
- **FDX:** Founding participant in the Financial Data Exchange; data sharing is FDX-aligned.
- **CFPB Section 1033:** Positioned publicly as an enabler of consumer financial data rights / 1033 open-banking access.
- **Aggregator tier:** Finicity is itself an aggregator — for most connected institutions it is the data-access seam, alongside Plaid, MX, Akoya and others.

## Tags

- Financial Services
- Data Aggregation
- Open Finance
- Open Banking
- FDX
- United States
- Payments
- Financial Data

## Timestamps

- **Created:** 2026-07-23
- **Modified:** 2026-07-23

## APIs

### Finicity Aggregation (Accounts & Transactions) API

Consumer-permissioned account and transaction aggregation across banks, credit unions, cards, loans and investment accounts, delivering account details, balances and categorized transactions.

- **Human URL:** [https://developer.mastercard.com/open-banking-us/documentation/](https://developer.mastercard.com/open-banking-us/documentation/)
- **Base URL:** `https://api.finicity.com`

### Finicity Connect

Hosted, embeddable account-linking experience that lets a consumer authenticate to their financial institution and permission data sharing, returning the linked accounts to the partner application.

- **Human URL:** [https://developer.mastercard.com/open-banking-us/documentation/connect/](https://developer.mastercard.com/open-banking-us/documentation/connect/)
- **Base URL:** `https://api.finicity.com`

### Finicity Verification of Assets (VoA) API

Generates a consumer-permissioned Verification of Assets report from aggregated account and balance data for mortgage, lending and underwriting workflows — an FCRA-regulated consumer report product.

- **Human URL:** [https://developer.mastercard.com/open-banking-us/documentation/](https://developer.mastercard.com/open-banking-us/documentation/)
- **Base URL:** `https://api.finicity.com`

### Finicity Verification of Income & Employment (VoIE) API

Derives income streams and employment signals from permissioned transaction and payroll data to produce Verification of Income and Verification of Employment reports for lending decisions.

- **Human URL:** [https://developer.mastercard.com/open-banking-us/documentation/](https://developer.mastercard.com/open-banking-us/documentation/)
- **Base URL:** `https://api.finicity.com`

### Finicity Transaction Analysis (Cash Flow) API

Analyzes permissioned transaction history to produce cash-flow, income and expense insights used for prequalification, credit decisioning and financial-health scoring.

- **Human URL:** [https://developer.mastercard.com/open-banking-us/documentation/](https://developer.mastercard.com/open-banking-us/documentation/)
- **Base URL:** `https://api.finicity.com`

### Finicity Payments (Account Validation) API

Validates account ownership and status for ACH and account-funding flows, returning account, routing and owner verification signals to reduce returned payments and fraud.

- **Human URL:** [https://developer.mastercard.com/open-banking-us/documentation/](https://developer.mastercard.com/open-banking-us/documentation/)
- **Base URL:** `https://api.finicity.com`

### Finicity Open Banking Data Access (FDX)

FDX-aligned, consumer-permissioned open-banking data-access surface through which Finicity, as a founding Financial Data Exchange participant, shares financial data on behalf of connected institutions in support of CFPB Section 1033 data rights.

- **Human URL:** [https://developer.mastercard.com/open-banking-us/documentation/](https://developer.mastercard.com/open-banking-us/documentation/)
- **Base URL:** `https://api.finicity.com`

## Common Properties

- [Website](https://www.finicity.com/)
- [Developer Portal](https://developer.mastercard.com/open-banking-us/documentation/)
- [Documentation](https://developer.mastercard.com/open-banking-us/documentation/)
- [GitHub Organization](https://github.com/Finicity)
- [LinkedIn](https://www.linkedin.com/company/finicity/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
