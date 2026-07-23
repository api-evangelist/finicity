---
name: Subscribe to transaction and balance events
description: Register for real-time account events via TxPush and manage webhook notification subscriptions so the partner is pushed transaction and balance changes.
api: openapi/finicity-openbanking-us-openapi-original.yml
operations: [CreateToken, SubscribeToTxPushNotifications, CreateTxPushTestTransaction, DisableTxPushNotifications, updateWebhookSubscription]
---

# Subscribe to transaction and balance events

## Auth
- `Finicity-App-Key` + `Finicity-App-Token` (token from **CreateToken**, `POST /aggregation/v2/partners/authentication`).

## TxPush (per-account real-time push)
1. **SubscribeToTxPushNotifications** — `POST /aggregation/v1/customers/{customerId}/accounts/{accountId}/txpush` with your callback URL to receive `transaction` and `balance` events for that account.
2. **CreateTxPushTestTransaction** — `POST /aggregation/v1/customers/{customerId}/accounts/{accountId}/transactions` (test only) to inject a synthetic transaction and verify delivery.
3. **DisableTxPushNotifications** — `DELETE /aggregation/v1/customers/{customerId}/accounts/{accountId}/txpush` to stop.

## Notification Subscriptions (webhooks)
- Manage partner webhook subscriptions under `/notification-subscriptions/webhooks`; use **updateWebhookSubscription** (`PUT /notification-subscriptions/webhooks/{subscription_id}`) and per-event enable/disable + `test-subscriptions` endpoints to validate delivery.
- Note: the legacy per-customer webhook-subscription create/list operations are deprecated (see lifecycle/); prefer the notification-subscriptions surface for new work.

## Rules
- Callback endpoints must return 2xx quickly; retries are provider-side.
- Errors are `{ "code", "message" }` JSON.
