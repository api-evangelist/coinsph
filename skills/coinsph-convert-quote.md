---
name: Convert one crypto to another via quote-and-accept
description: Fetch supported pairs, request a firm quote, accept it, and reconcile the convert order on Coins.ph.
api: openapi/coinsph-convert-openapi.json
operations: [convert_get_supported_trading_pairs, convert_get_quote, convert_accept_quote, convert_query_order_history]
---

# Convert crypto (quote-and-accept)

Base URL: `https://api.pro.coins.ph`. Auth: `X-COINS-APIKEY` + `Timestamp` + `Signature` (HMAC-SHA256).

## Steps
1. `convert_get_supported_trading_pairs` — confirm the source/target pair is convertible.
2. `convert_get_quote` — request a firm quote for an amount; capture the quote id and expiry.
3. `convert_accept_quote` — accept before the quote expires to execute the conversion.
4. `convert_query_order_history` — reconcile the executed convert order.

## Rules
- Quotes are time-boxed — accept promptly or re-quote.
- Idempotency: reuse the same partner `requestId` on retries so a conversion is not double-executed.
  See `conventions/coinsph-conventions.yml`.
