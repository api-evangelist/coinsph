---
name: Collect a payment with a dynamic QR PH code
description: Generate a dynamic QRPH code, poll its status, and reconcile the collection on the Coins.ph Payment API.
api: openapi/coinsph-payment-openapi.json
operations: [generateDynamicQRPH, getQRPHStatus, cancelDynamicQRPH]
---

# Collect a payment via dynamic QRPH

Base URL: `https://api.pro.coins.ph` (sandbox: `https://api.9001.pl-qa.coinsxyz.me`).
Auth: `X-COINS-APIKEY` + `Timestamp` + `Signature` (HMAC-SHA256).

## Steps
1. `generateDynamicQRPH` — create a dynamic QR PH code for the amount; pass a partner `requestId` for idempotency.
2. Present the returned QR to the payer.
3. `getQRPHStatus` — poll for payment status until paid/expired.
4. `cancelDynamicQRPH` — cancel an unpaid code if the checkout is abandoned.

## Rules
- `requestId` is your idempotency key — reuse it on retries. See `conventions/coinsph-conventions.yml`.
- Settlement/refund events also arrive as HMAC-SHA256-signed webhooks — verify the signature.
  See `asyncapi/coinsph-webhooks.yml`.
