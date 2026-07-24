---
name: Deposit and withdraw crypto on Coins Pro
description: Fetch a deposit address, watch deposits, and submit a whitelisted withdrawal on Coins.ph.
api: openapi/coinsph-wallet-openapi.json
operations: [wallet_get_all_coins_info, wallet_get_deposit_address, get_deposit_history, get_withdraw_address_whitelist, post_withdraw_apply, get_withdraw_history]
---

# Deposit and withdraw crypto (Coins Pro)

Base URL: `https://api.pro.coins.ph`. Auth: `X-COINS-APIKEY` + `Timestamp` + `Signature` (HMAC-SHA256).

## Steps
1. `wallet_get_all_coins_info` — list supported coins/networks and their deposit/withdraw status.
2. `wallet_get_deposit_address` — get the deposit address (and memo/tag) for a coin+network.
3. `get_deposit_history` — confirm inbound deposits credited.
4. `get_withdraw_address_whitelist` — confirm the destination is whitelisted (withdrawals require it).
5. `post_withdraw_apply` — submit the withdrawal (coin, network, address, amount).
6. `get_withdraw_history` — track the withdrawal to completion.

## Rules
- Withdrawals typically require the destination on the address whitelist; add it out-of-band first.
- Signed requests only; `401` means bad key/signature. See `errors/coinsph-problem-types.yml`.
