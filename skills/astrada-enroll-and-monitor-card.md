---
name: Enroll a card and monitor its transactions
description: Provision a subaccount, enroll a corporate card via the Card Enrollment SDK, confirm the enrolled card, and read the real-time transactions it produces.
api: openapi/astrada-openapi-original.json
operations: [CreateSubaccount, EnrollmentMethods, ListCards, GetCard, GetCardholder, GetTransactions, GetTransactionById]
---

# Enroll a card and monitor its transactions

Astrada delivers real-time, structured card transaction data for enrolled cards. This skill
covers the happy path from subaccount setup to reading transactions.

## Prerequisites
- OAuth2 **client_credentials** token (Client ID / Secret / Account ID from Astrada support).
  POST to `https://api.astrada.co/auth/realms/{accountId}/protocol/openid-connect/token`, then
  send `Authorization: Bearer <token>`. Tokens expire (~300s) — refresh as needed.
- See `conventions/astrada-conventions.yml` (HAL pagination, problem+json errors) and
  `scopes/astrada-scopes.yml`.

## Steps
1. **Create a subaccount** with the networks/regions you need — `CreateSubaccount`
   (POST `/subaccounts`). Configure `verificationPolicy.sandbox: true` for testing.
2. **Check enrollment methods** available for the subaccount — `EnrollmentMethods`
   (POST `/enrollment-methods`).
3. **Enroll the card**: launch the hosted Card Enrollment SDK
   (`https://sdk.astrada.co/v1/cardEnrollmentSdk.js`, `CardEnrollmentSdk.openForm({ subaccountId })`)
   so the cardholder completes 3DS verification. See `components/astrada-components.yml`.
4. **Confirm the enrolled card** — `ListCards` (GET `/cards`, offset pagination) then
   `GetCard` (GET `/cards/{cardId}`); optionally `GetCardholder` (GET `/cards/{cardId}/cardholder`).
5. **Read transactions** — `GetTransactions` (GET `/transactions`) and `GetTransactionById`
   (GET `/transactions/{transactionId}`). For push delivery, subscribe to `transaction.created`
   webhooks (see the webhook skill).

## Testing
Use the sandbox test-card matrix in `sandbox/astrada-sandbox.yml` (e.g. `4242424242424242`
for frictionless success). Only published test cards enroll in the sandbox environment.
