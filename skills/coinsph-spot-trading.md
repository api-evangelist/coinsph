---
name: Place and manage a spot order on Coins Pro
description: Authenticate, inspect the market, place a spot order, then track or cancel it on the Coins.ph exchange.
api: openapi/coinsph-spot-openapi.json
operations: [get_exchange_info, test_new_order, create_new_order, query_order, get_open_orders, cancel_order]
---

# Place and manage a spot order (Coins Pro)

Base URL: `https://api.pro.coins.ph` (sandbox: `https://api.9001.pl-qa.coinsxyz.me`).

## Auth
Every request carries three headers: `X-COINS-APIKEY` (your key), `Timestamp` (Unix ms), and
`Signature` (HMAC-SHA256 of the query string using your API secret). See
`authentication/coinsph-authentication.yml` and `conventions/coinsph-conventions.yml`.

## Steps
1. `get_exchange_info` — read trading rules and the symbol you want (e.g. `BTCPHP`), including lot-size and price filters.
2. `test_new_order` — validate the order payload without placing it; fix any filter violations first.
3. `create_new_order` — place the real order (symbol, side, type, quantity/price). Record the returned `orderId`.
4. `query_order` — poll the order by `orderId`/`symbol` for fill status.
5. `get_open_orders` — list still-open orders for the symbol.
6. `cancel_order` — cancel by `orderId` if it must not fill.

## Rules
- Sync `Timestamp` using `check_server_time` (system API) when local clock skew is a risk; bound with `recvWindow`.
- Errors return `{ code, msg }`; `429` means rate-limited — back off. See `errors/coinsph-problem-types.yml`.
