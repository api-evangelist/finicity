# Finicity (finicity)

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
