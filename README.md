# Astrada

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

Astrada is the data layer for autonomous finance, providing real-time, structured card transaction data pulled directly from the card networks rather than relying on delayed bank feeds. Its Transaction Data API lets expense management, travel, and accounting/ERP platforms enroll corporate cards (with 3DS cardholder verification), receive real-time transaction messages and enriched transactions, link bank accounts, and auto-reconcile card-to-bank activity. Founded in 2024 by Salman Syed (ex-Mastercard, Marqeta, Fidel API), Astrada is PCI DSS v4 Level 1 certified, a Mastercard Start Path and Visa Ventures portfolio company, and is backed by QED Investors.

**Areas:** Company · Fintech · Payments · Card Data · Transaction Data · Reconciliation · Expense Management · Data Infrastructure

## Astrada on APIs.io

Everything profiled for Astrada is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/astrada/](https://apis.io/providers/astrada/)** — or go straight to one of the APIs or properties below.

### APIs (15)

- [Astrada Bank Accounts API](https://apis.io/apis/astrada/astrada-bank-accounts-api/) — Manage connected bank accounts. Bank accounts are created automatically when a bank link enrollment is completed.
- [Astrada Bank Links API](https://apis.io/apis/astrada/astrada-bank-links-api/) — Manage bank enrollment links. A bank link represents an invitation for a user to connect their bank account via Plaid.
- [Astrada Bank Subscriptions API](https://apis.io/apis/astrada/astrada-bank-subscriptions-api/) — Manage bank subscriptions (Plaid connections). A subscription represents an active connection to a financial institution.
- [Astrada Bank Transactions API](https://apis.io/apis/astrada/astrada-bank-transactions-api/) — Access bank transactions synced from connected accounts. Transactions are ingested via Plaid and can be matched against card transactions.
- [Astrada Bin Lookup API](https://apis.io/apis/astrada/astrada-bin-lookup-api/) — BIN Lookup
- [Astrada Card API](https://apis.io/apis/astrada/astrada-card-api/) — Card resource
- [Astrada Card Subscription API](https://apis.io/apis/astrada/astrada-card-subscription-api/) — Card Subscription resource
- [Astrada Card Verification API](https://apis.io/apis/astrada/astrada-card-verification-api/) — Card Verification
- [Astrada Enrollment Methods API](https://apis.io/apis/astrada/astrada-enrollment-methods-api/) — Enrollment methods resource
- [Astrada Network Bulk Feeds API](https://apis.io/apis/astrada/astrada-network-bulk-feeds-api/) — Network bulk feed resource
- [Astrada Subaccounts API](https://apis.io/apis/astrada/astrada-subaccounts-api/) — Subaccount resource
- [Astrada Transaction Matches API](https://apis.io/apis/astrada/astrada-transaction-matches-api/) — Access transaction matches between bank and card transactions, including confidence scores and match reasoning.
- [Astrada Transaction Messages API](https://apis.io/apis/astrada/astrada-transaction-messages-api/) — Transaction messages resource
- [Astrada Transactions API](https://apis.io/apis/astrada/astrada-transactions-api/) — Transaction resource
- [Astrada Webhooks API](https://apis.io/apis/astrada/astrada-webhooks-api/) — Manage webhooks

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (2)

Event-driven and webhook contracts.

- [Astrada Webhook Events](https://apis.io/asyncapis/astrada/astrada-events-asyncapi/)
- [Astrada Webhooks](https://apis.io/asyncapis/astrada/astrada-webhooks/)

#### Event channels (11)

Individual events and webhooks the provider emits.

- [banklink.completed](https://apis.io/channels/astrada/banklink-completed/)
- [banktransaction.created](https://apis.io/channels/astrada/banktransaction-created/)
- [banktransaction.deleted](https://apis.io/channels/astrada/banktransaction-deleted/)
- [cardsubscription.created](https://apis.io/channels/astrada/cardsubscription-created/)
- [cardsubscription.updated](https://apis.io/channels/astrada/cardsubscription-updated/)
- [enrichment.merchant.created](https://apis.io/channels/astrada/enrichment-merchant-created/)
- [transaction.created](https://apis.io/channels/astrada/transaction-created/)
- [transaction.match.created](https://apis.io/channels/astrada/transaction-match-created/)
- [transaction.match.deleted](https://apis.io/channels/astrada/transaction-match-deleted/)
- [transaction.updated](https://apis.io/channels/astrada/transaction-updated/)
- [transactionmessage.created](https://apis.io/channels/astrada/transactionmessage-created/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [astrada](https://apis.io/servers/astrada/astrada/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Astrada Agentic Access](https://apis.io/agentic-access/astrada/astrada-agentic-access/)

#### Collections (30)

Postman and Open Collection request collections.

- [Astrada bank-accounts API](https://apis.io/collections/astrada/open-astrada-bank-accounts-api/)
- [Astrada bank-accounts bank-links API](https://apis.io/collections/astrada/open-astrada-bank-links-api/)
- [Astrada bank-accounts bank-subscriptions API](https://apis.io/collections/astrada/open-astrada-bank-subscriptions-api/)
- [Astrada bank-accounts bank-transactions API](https://apis.io/collections/astrada/open-astrada-bank-transactions-api/)
- [Astrada bank-accounts bin-lookup API](https://apis.io/collections/astrada/open-astrada-bin-lookup-api/)
- [Astrada bank-accounts card API](https://apis.io/collections/astrada/open-astrada-card-api/)
- [Astrada bank-accounts card-subscription API](https://apis.io/collections/astrada/open-astrada-card-subscription-api/)
- [Astrada bank-accounts card-verification API](https://apis.io/collections/astrada/open-astrada-card-verification-api/)
- [Astrada bank-accounts enrollment-methods API](https://apis.io/collections/astrada/open-astrada-enrollment-methods-api/)
- [Astrada bank-accounts network-bulk-feeds API](https://apis.io/collections/astrada/open-astrada-network-bulk-feeds-api/)
- [Astrada bank-accounts subaccounts API](https://apis.io/collections/astrada/open-astrada-subaccounts-api/)
- [Astrada bank-accounts transaction-matches API](https://apis.io/collections/astrada/open-astrada-transaction-matches-api/)
- [Astrada bank-accounts transaction-messages API](https://apis.io/collections/astrada/open-astrada-transaction-messages-api/)
- [Astrada bank-accounts transactions API](https://apis.io/collections/astrada/open-astrada-transactions-api/)
- [Astrada bank-accounts webhooks API](https://apis.io/collections/astrada/open-astrada-webhooks-api/)
- [Astrada bank-accounts API](https://apis.io/collections/astrada/postman-astrada-bank-accounts-api/)
- [Astrada bank-accounts bank-links API](https://apis.io/collections/astrada/postman-astrada-bank-links-api/)
- [Astrada bank-accounts bank-subscriptions API](https://apis.io/collections/astrada/postman-astrada-bank-subscriptions-api/)
- [Astrada bank-accounts bank-transactions API](https://apis.io/collections/astrada/postman-astrada-bank-transactions-api/)
- [Astrada bank-accounts bin-lookup API](https://apis.io/collections/astrada/postman-astrada-bin-lookup-api/)
- [Astrada bank-accounts card API](https://apis.io/collections/astrada/postman-astrada-card-api/)
- [Astrada bank-accounts card-subscription API](https://apis.io/collections/astrada/postman-astrada-card-subscription-api/)
- [Astrada bank-accounts card-verification API](https://apis.io/collections/astrada/postman-astrada-card-verification-api/)
- [Astrada bank-accounts enrollment-methods API](https://apis.io/collections/astrada/postman-astrada-enrollment-methods-api/)
- [Astrada bank-accounts network-bulk-feeds API](https://apis.io/collections/astrada/postman-astrada-network-bulk-feeds-api/)
- …and 5 more published on APIs.io

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Astrada Openapi Overlay](https://apis.io/overlays/astrada/astrada-openapi-overlay/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Astrada Authentication](https://apis.io/security/astrada/astrada-authentication/)
- [Astrada Domain Security](https://apis.io/security/astrada/astrada-domain-security/)
- [Astrada Trust Center](https://apis.io/security/astrada/astrada-trust-center/)
- [Astrada Vulnerability Disclosure](https://apis.io/security/astrada/astrada-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Astrada Scopes](https://apis.io/scopes/astrada/astrada-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://astrada.co/)
- [Documentation](https://docs.astrada.co/docs/home)
- [Getting started](https://docs.astrada.co/docs/getting-started-1)
- [API reference](https://docs.astrada.co/reference)
- [Sign up](https://astrada.co/company/contact)
- [Support](https://astrada.co/company/contact)
- [Blog](https://astrada.co/blog)
- [Security](https://astrada.co/security)
- [Compliance](https://astrada.co/security)
- [Terms of service](https://astrada.co/legal)
- [Privacy policy](https://astrada.co/legal)
- [Status](https://status.astrada.co)

## API Evangelist rating

**Kin Score 54.7** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 58.1 |
| Contract governance | 18.2 |
| Operational transparency | 50.0 |
| Developer ergonomics | 53.0 |
| Access clarity | 50.0 |

**Agent readiness 34.2** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | verified |
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
| Pagination Ratio | paginated |
| Operation Distinctiveness | distinct |

**Regulatory alignment 48.2** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/astrada/](https://apis.io/providers/astrada/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Astrada: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/astrada/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
