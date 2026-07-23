---
name: Link a bank account and reconcile card transactions
description: Create a bank link, discover bank accounts, link enrolled cards to them, and retrieve card-to-bank transaction matches for auto-reconciliation.
api: openapi/astrada-openapi-original.json
operations: [CreateBankLink, GetBankLink, ListBankAccounts, LinkEnrolledCards, SyncBankLink, ListTransactionMatches, GetTransactionMatch]
---

# Link a bank account and reconcile card transactions

Astrada's auto-reconciliation matches card transactions to bank feed entries. This skill
links a bank account and reads the resulting matches.

## Prerequisites
- OAuth2 client_credentials bearer token (see `authentication/astrada-authentication.yml`);
  banking scopes (`banking:read`, `banking:write`) from `scopes/astrada-scopes.yml`.

## Steps
1. **Create a bank link** — `CreateBankLink` (POST `/bank-links`). Poll `GetBankLink`
   (GET `/bank-links/{bankLinkId}`) or subscribe to the `banklink.completed` webhook.
2. **List discovered accounts** — `ListBankAccounts` (GET `/bank-accounts`).
3. **Link enrolled cards to a bank account** — `LinkEnrolledCards`
   (POST `/bank-accounts/link-enrolled-cards`).
4. **Refresh / sync** as needed — `SyncBankLink` (POST `/bank-links/{bankLinkId}/sync`)
   and `RefreshBankAccount` (POST `/bank-accounts/{bankAccountId}/refresh`).
5. **Read reconciliation matches** — `ListTransactionMatches`
   (GET `/transaction-matches/{subaccountId}`) and `GetTransactionMatch`
   (GET `/transaction-matches/{subaccountId}/{transactionMatchId}`).

## Events
Subscribe to `banklink.completed`, `banktransaction.created`, `transaction.match.created`
(see `asyncapi/astrada-webhooks.yml`).

## Errors
Failures use RFC 7807 problem+json — see `errors/astrada-problem-types.yml`.
