---
name: Pull a customer's transactions
description: Refresh and read a linked customer's account transactions, including historic load and date-ranged retrieval, for cash-flow and decisioning use.
api: openapi/finicity-openbanking-us-openapi-original.yml
operations: [CreateToken, RefreshCustomerAccounts, LoadHistoricTransactionsForCustomerAccount, GetAllCustomerTransactions, GetCustomerAccountTransactions]
---

# Pull a customer's transactions

## Auth
- Send `Finicity-App-Key` + `Finicity-App-Token`; obtain the token via **CreateToken** (`POST /aggregation/v2/partners/authentication`).

## Steps
1. **RefreshCustomerAccounts** — `POST /aggregation/v1/customers/{customerId}/accounts` to bring balances/transactions current before reading.
2. (Optional, first pull) **LoadHistoricTransactionsForCustomerAccount** — `POST /aggregation/v1/customers/{customerId}/accounts/{accountId}/transactions/historic` to backfill history for one account.
3. **GetAllCustomerTransactions** — `GET /aggregation/v3/customers/{customerId}/transactions` across all accounts, or **GetCustomerAccountTransactions** — `GET /aggregation/v4/customers/{customerId}/accounts/{accountId}/transactions` for one account.

## Conventions
- Filter with `fromDate` / `toDate` as **UNIX epoch seconds**.
- Page with `start` + `limit` (1-based `start`).
- For real-time updates instead of polling, subscribe with TxPush (see the webhooks skill).
