# Coins.ph

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

Coins.ph is a BSP-regulated Philippine fintech super app combining a licensed crypto exchange (Coins Pro), an e-wallet for pesos and 170+ cryptocurrencies, and a merchant/partner payments platform. Its public developer platform exposes a Partner Integration / Payment API (QRPH collections, checkout, disbursements, refunds, virtual accounts, reconciliation) and the Coins Pro exchange API (spot trading, wallets, market data, convert, sub-accounts, and a WebSocket user-data stream), plus an on/off ramp API. All requests are authenticated with an API key and HMAC-SHA256 request signing (X-COINS-APIKEY, Timestamp, Signature). Backed by Pantera Capital and Ribbit Capital.

**Areas:** Company · Cryptocurrency · Cryptocurrency Exchange · Payments · Fintech · Wallets · Philippines · Trading

## Coins.ph on APIs.io

Everything profiled for Coins.ph is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/coinsph/](https://apis.io/providers/coinsph/)** — or go straight to one of the APIs or properties below.

### APIs (26)

- [Coins.ph Account API](https://apis.io/apis/coinsph/coinsph-account-api/) — Account management APIs.
- [Coins.ph Account Validation API](https://apis.io/apis/coinsph/coinsph-account-validation-api/) — The Account Validation API from Coins.ph — 2 operation(s) for account validation.
- [Coins.ph Checkout API](https://apis.io/apis/coinsph/coinsph-checkout-api/) — Checkout creation and management
- [Coins.ph Checkout Refund API](https://apis.io/apis/coinsph/coinsph-checkout-refund-api/) — Checkout refund operations
- [Coins.ph Collections - Crypto API](https://apis.io/apis/coinsph/coinsph-collections-crypto-api/) — Crypto deposit address
- [Coins.ph Collections - QRPH API](https://apis.io/apis/coinsph/coinsph-collections-qrph-api/) — QRPH code generation and management
- [Coins.ph Convert API](https://apis.io/apis/coinsph/coinsph-convert-api/) — Convert quote and acceptance operations.
- [Coins.ph Disbursements API](https://apis.io/apis/coinsph/coinsph-disbursements-api/) — Cash-out and disbursement operations
- [Coins.ph General API](https://apis.io/apis/coinsph/coinsph-general-api/) — General endpoints for connectivity, server time, system status, and user IP.
- [Coins.ph Listens API](https://apis.io/apis/coinsph/coinsph-listens-api/) — Manage user data stream listenKeys for WebSocket connections. A listenKey is required to establish a private WebSocket connection for receiving real-time…
- [Coins.ph Markets API](https://apis.io/apis/coinsph/coinsph-markets-api/) — Market data APIs.
- [Coins.ph ON/OFF Ramp API](https://apis.io/apis/coinsph/coinsph-on-off-ramp-api/) — Fiat-to-crypto and crypto-to-fiat ramp operations
- [Coins.ph Order History API](https://apis.io/apis/coinsph/coinsph-order-history-api/) — Order history and details
- [Coins.ph Ramp Callback API](https://apis.io/apis/coinsph/coinsph-ramp-callback-api/) — Webhook callbacks sent to the merchant's configured callback URL when order status changes
- [Coins.ph Reconciliation API](https://apis.io/apis/coinsph/coinsph-reconciliation-api/) — Reconciliation report
- [Coins.ph Refund API](https://apis.io/apis/coinsph/coinsph-refund-api/) — Refund operations
- [Coins.ph Scan to Pay API](https://apis.io/apis/coinsph/coinsph-scan-to-pay-api/) — QR code scan-to-pay payment operations
- [Coins.ph Spot API](https://apis.io/apis/coinsph/coinsph-spot-api/) — Spot trading operations including order placement, querying, cancellation, and trade history.
- [Coins.ph Sub Account API](https://apis.io/apis/coinsph/coinsph-sub-account-api/) — Sub Account deposit, withdrawal, and transfer operations.
- [Coins.ph Tokenized Checkout API](https://apis.io/apis/coinsph/coinsph-tokenized-checkout-api/) — Password-free (auto-debit) checkout
- [Coins.ph Trading - Convert API](https://apis.io/apis/coinsph/coinsph-trading-convert-api/) — Convert trading operations
- [Coins.ph Trading - OTC API](https://apis.io/apis/coinsph/coinsph-trading-otc-api/) — OTC trading for Business Account
- [Coins.ph Transfers API](https://apis.io/apis/coinsph/coinsph-transfers-api/) — The Transfers API from Coins.ph — 2 operation(s) for transfers.
- [Coins.ph Utility API](https://apis.io/apis/coinsph/coinsph-utility-api/) — Account balance, transfers, and utility endpoints
- [Coins.ph Virtual Account API](https://apis.io/apis/coinsph/coinsph-virtual-account-api/) — Virtual account creation and management
- [Coins.ph Wallet API](https://apis.io/apis/coinsph/coinsph-wallet-api/) — Convert, Deposit, Withdraw, Transfers, and Sub Account Transfer operations.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Coinsph Webhooks](https://apis.io/asyncapis/coinsph/coinsph-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [coinsph](https://apis.io/servers/coinsph/coinsph/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Coinsph Agentic Access](https://apis.io/agentic-access/coinsph/coinsph-agentic-access/)

#### Collections (26)

Postman and Open Collection request collections.

- [TRADING Account API](https://apis.io/collections/coinsph/open-coinsph-account-api/)
- [TRADING Account Account Validation API](https://apis.io/collections/coinsph/open-coinsph-account-validation-api/)
- [TRADING Account Checkout API](https://apis.io/collections/coinsph/open-coinsph-checkout-api/)
- [TRADING Account Checkout Refund API](https://apis.io/collections/coinsph/open-coinsph-checkout-refund-api/)
- [TRADING Account Collections - Crypto API](https://apis.io/collections/coinsph/open-coinsph-collections-crypto-api/)
- [TRADING Account Collections - QRPH API](https://apis.io/collections/coinsph/open-coinsph-collections-qrph-api/)
- [TRADING Account Convert API](https://apis.io/collections/coinsph/open-coinsph-convert-api/)
- [TRADING Account Disbursements API](https://apis.io/collections/coinsph/open-coinsph-disbursements-api/)
- [TRADING Account General API](https://apis.io/collections/coinsph/open-coinsph-general-api/)
- [TRADING Account Listens API](https://apis.io/collections/coinsph/open-coinsph-listens-api/)
- [TRADING Account Markets API](https://apis.io/collections/coinsph/open-coinsph-markets-api/)
- [TRADING Account ON/OFF Ramp API](https://apis.io/collections/coinsph/open-coinsph-on-off-ramp-api/)
- [TRADING Account Order History API](https://apis.io/collections/coinsph/open-coinsph-order-history-api/)
- [TRADING Account Ramp Callback API](https://apis.io/collections/coinsph/open-coinsph-ramp-callback-api/)
- [TRADING Account Reconciliation API](https://apis.io/collections/coinsph/open-coinsph-reconciliation-api/)
- [TRADING Account Refund API](https://apis.io/collections/coinsph/open-coinsph-refund-api/)
- [TRADING Account Scan to Pay API](https://apis.io/collections/coinsph/open-coinsph-scan-to-pay-api/)
- [TRADING Account Spot API](https://apis.io/collections/coinsph/open-coinsph-spot-api/)
- [TRADING Account Sub Account API](https://apis.io/collections/coinsph/open-coinsph-sub-account-api/)
- [TRADING Account Tokenized Checkout API](https://apis.io/collections/coinsph/open-coinsph-tokenized-checkout-api/)
- [TRADING Account Trading - Convert API](https://apis.io/collections/coinsph/open-coinsph-trading-convert-api/)
- [TRADING Account Trading - OTC API](https://apis.io/collections/coinsph/open-coinsph-trading-otc-api/)
- [TRADING Account Transfers API](https://apis.io/collections/coinsph/open-coinsph-transfers-api/)
- [TRADING Account Utility API](https://apis.io/collections/coinsph/open-coinsph-utility-api/)
- [TRADING Account Virtual Account API](https://apis.io/collections/coinsph/open-coinsph-virtual-account-api/)
- …and 1 more published on APIs.io

#### Overlays (11)

OpenAPI overlays, including conversational phrasing for each operation.

- [Coinsph Account Overlay](https://apis.io/overlays/coinsph/coinsph-account-overlay/)
- [Coinsph Account Validation Overlay](https://apis.io/overlays/coinsph/coinsph-account-validation-overlay/)
- [Coinsph Convert Overlay](https://apis.io/overlays/coinsph/coinsph-convert-overlay/)
- [Coinsph Listenkey Overlay](https://apis.io/overlays/coinsph/coinsph-listenkey-overlay/)
- [Coinsph Markets Overlay](https://apis.io/overlays/coinsph/coinsph-markets-overlay/)
- [Coinsph Payment Overlay](https://apis.io/overlays/coinsph/coinsph-payment-overlay/)
- [Coinsph Ramp Overlay](https://apis.io/overlays/coinsph/coinsph-ramp-overlay/)
- [Coinsph Spot Overlay](https://apis.io/overlays/coinsph/coinsph-spot-overlay/)
- [Coinsph Sub Account Overlay](https://apis.io/overlays/coinsph/coinsph-sub-account-overlay/)
- [Coinsph System Overlay](https://apis.io/overlays/coinsph/coinsph-system-overlay/)
- [Coinsph Wallet Overlay](https://apis.io/overlays/coinsph/coinsph-wallet-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Coinsph Authentication](https://apis.io/security/coinsph/coinsph-authentication/)
- [Coinsph Domain Security](https://apis.io/security/coinsph/coinsph-domain-security/)
- [Coinsph Vulnerability Disclosure](https://apis.io/security/coinsph/coinsph-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://coins.ph/)
- [Documentation](https://api.docs.coins.ph)
- [Getting started](https://api.docs.coins.ph)
- [API reference](https://api.docs.coins.ph)
- [Pricing](https://coins.ph/en-ph/fees)
- [Support](https://support.coins.ph/hc/en-us)
- [Changelog](https://api.docs.coins.ph/changelog)
- [Blog](https://coins.ph/en-ph/blog)
- [Security](https://coins.ph/en-ph/bug-bounty)
- [Terms of service](https://coins.ph/en-ph/legal)
- [Privacy policy](https://coins.ph/en-ph/legal#privacy)
- [GitHub](https://github.com/coinsph)
- [Status](https://status.coins.ph)

## API Evangelist rating

**Kin Score 50.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 58.9 |
| Contract governance | 4.5 |
| Operational transparency | 44.7 |
| Developer ergonomics | 54.2 |
| Access clarity | 31.6 |

**Agent readiness 35.1** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | derived (partial credit) |
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
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 27.7** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/coinsph/](https://apis.io/providers/coinsph/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Coins.ph: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/coinsph/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
