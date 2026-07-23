---
name: Register and verify Astrada webhooks
description: Create a webhook subscription for the event types you need, then verify inbound webhook signatures using the HMAC-SHA256 scheme.
api: openapi/astrada-openapi-original.json
operations: [createWebhook, listWebhooks, getWebhook, updateWebhook, deleteWebhook]
---

# Register and verify Astrada webhooks

Astrada pushes events to your HTTPS endpoint with at-least-once delivery and signed payloads.

## Prerequisites
- OAuth2 client_credentials bearer token; `webhooks:write` / `webhooks:read` scopes.

## Steps
1. **Create a webhook** — `createWebhook` (POST `/webhooks`) with an HTTPS URL and the
   event types (see `asyncapi/astrada-events-asyncapi.yml`). Capture the returned signing
   secret — it is shown only once. Max 2500 subscriptions per subaccount.
2. **List / inspect** — `listWebhooks` (GET `/webhooks`), `getWebhook` (GET `/webhooks/{webhookId}`).
3. **Update or remove** — `updateWebhook` (PATCH `/webhooks/{webhookId}`),
   `deleteWebhook` (DELETE `/webhooks/{webhookId}`).

## Verifying inbound deliveries
Each POST carries `webhook-id`, `webhook-timestamp`, `webhook-signature` (plus
`webhook-event-type`, `webhook-subaccount-id`). Compute
`HMAC-SHA256(base64_decode(secret), "{webhook-id}.{webhook-timestamp}.{body}")`, base64-encode,
and compare to `webhook-signature` (strip the `v1,` prefix). Return **200** to acknowledge;
non-200 triggers retries (5s, 5m, 30m, 2h, 5h, 10h, 10h). Full detail in
`asyncapi/astrada-webhooks.yml`.

## Idempotency
Delivery is **at-least-once** — dedupe on `webhook-id` (stable across retries). Astrada
does not offer a client idempotency-key header (see `conventions/astrada-conventions.yml`).
