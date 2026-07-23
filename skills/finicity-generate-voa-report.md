---
name: Generate a Verification of Assets (VoA) report
description: Produce a consumer-permissioned Verification of Assets report from a linked customer's aggregated accounts for lending and underwriting.
api: openapi/finicity-openbanking-us-openapi-original.yml
operations: [CreateToken, RefreshCustomerAccounts, GenerateVOAReport, GenerateVOAWithIncomeReport]
---

# Generate a Verification of Assets (VoA) report

Requires the customer's accounts to already be linked (see the Connect skill). VoA products are FCRA-regulated consumer reports — only run with proper permissible purpose and consumer consent.

## Auth
- `Finicity-App-Key` + `Finicity-App-Token` (token from **CreateToken**, `POST /aggregation/v2/partners/authentication`).

## Steps
1. **RefreshCustomerAccounts** — `POST /aggregation/v1/customers/{customerId}/accounts` so the report runs on current data.
2. **GenerateVOAReport** — `POST /decisioning/v2/customers/{customerId}/voa` to generate the assets report. Use **GenerateVOAWithIncomeReport** — `POST /decisioning/v2/customers/{customerId}/voaHistory` when income history is also needed.
3. Poll/read the returned report id via the Reports endpoints once status is complete.

## Rules
- 403 means the VoA product is not entitled for the partner/app.
- Errors are `{ "code", "message" }`; there are no idempotency keys, so check for an existing report before regenerating.
