---
name: Link a customer's accounts with Finicity Connect
description: Authenticate as a partner, create a customer, generate a hosted Connect URL for consumer-permissioned account linking, then refresh and read the linked accounts.
api: openapi/finicity-openbanking-us-openapi-original.yml
operations: [CreateToken, AddCustomer, GenerateConnectUrl, RefreshCustomerAccounts, GetCustomerAccounts]
---

# Link a customer's accounts with Finicity Connect

Use this to onboard a consumer and pull their permissioned accounts via the hosted Connect experience.

## Auth
- Every call sends two headers: `Finicity-App-Key` (static partner key) and `Finicity-App-Token`.
- Get the token first: **CreateToken** — `POST /aggregation/v2/partners/authentication` with `partnerId` + `partnerSecret` (and the app key header). It returns a short-lived `token`; send it as `Finicity-App-Token`. Re-auth when it expires (401).

## Steps
1. **AddCustomer** — `POST /aggregation/v2/customers/active` to create the end customer; keep the returned `id` (customerId). (In test, use **AddTestingCustomer** `POST /aggregation/v2/customers/testing`.)
2. **GenerateConnectUrl** — `POST /connect/v2/generate` with `partnerId` + `customerId`. Return/redirect the consumer to the `link` so they authenticate to their institution and grant consent.
3. **RefreshCustomerAccounts** — `POST /aggregation/v1/customers/{customerId}/accounts` after Connect completes to pull fresh account data.
4. **GetCustomerAccounts** — `GET /aggregation/v1/customers/{customerId}/accounts` to read the linked accounts (balances, types, institution ids).

## Rules
- Errors are `{ "code", "message" }` JSON; 401 = re-auth, 403 = product not entitled, 429 = back off.
- No idempotency keys — do not blind-retry writes; check state first.
- Test with FinBank: institution `102105`, credentials `profile_03` / `profile_03`.
