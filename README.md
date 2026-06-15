# OPay (opay)

OPay is a Nigerian mobile money and fintech super-app operated by Blue Ridge Microfinance Bank (OPay Digital Services Limited) and majority-owned by Opera Limited with backing from SoftBank Vision Fund 2, Sequoia China, DragonBall Capital, and 9F Group. Launched in 2018 and headquartered in Lagos, OPay serves tens of millions of Nigerian consumers, merchants, and agents with wallet accounts, free interbank transfers, the OPay Debit Card, OWealth (daily-interest savings powered by OPay Microfinance Bank), bill payments, airtime/data top-ups, BNPL (OBuy / OPay Easy Buy), and the OPay POS / agent banking network. For developers and merchants, OPay exposes the OPay Cashier / OPay Checkout API — a REST API for accepting payments via 3DS bank cards, bank transfer, USSD, bank account, POS, OPay wallet QR, and reference codes, with hosted Express Checkout, server-to-server APIs, callback webhooks, refund and query operations, a PHP gateway SDK, and a WooCommerce plugin. Sandbox and production environments are available at testapi.opaycheckout.com and liveapi.opaycheckout.com, with HMAC-SHA512 signature authentication and per-merchant public/private key pairs issued from the OPay merchant dashboard.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/opay/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/opay/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- Payments
- Mobile Money
- Fintech
- Super App
- Nigeria
- Africa
- Wallet
- Savings
- BNPL
- Bank Transfer
- Card Payments
- USSD
- Agent Banking
- POS
- Bill Payments
- Airtime
- Cashier
- Checkout
- Merchant Acquiring

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### OPay Cashier API

The OPay Cashier API is the primary merchant payment API behind OPay Checkout. It exposes a hosted Express Checkout endpoint (cashier/create returning a cashierUrl), server-to-server payment creation for 3DS bank cards, bank transfer, bank USSD, bank account, POS, OPay wallet QR, and reference code payments, plus status queries, cancel, refund, and refund-status operations. Authentication uses an Authorization Bearer token — the public key for cashier/create and an HMAC-SHA512 signature over the JSON body (signed with the merchant's private key) for all other endpoints — along with a MerchantId header.

- **Human URL:** [https://documentation.opaycheckout.com/](https://documentation.opaycheckout.com/)
- **Base URL:** `https://liveapi.opaycheckout.com/api/v1/international`

#### Tags

- Payments
- Cashier
- Checkout
- Cards
- Bank Transfer
- USSD
- Wallet
- Refunds

#### Properties

- [Documentation](https://documentation.opaycheckout.com/)
- [Getting Started](https://documentation.opaycheckout.com/getting-started)
- [Authentication](https://documentation.opaycheckout.com/payment-authentication)
- [API Reference](https://documentation.opaycheckout.com/server-apis-overview)
- [Webhooks](https://documentation.opaycheckout.com/payment-notifications)
- [Sandbox](https://testapi.opaycheckout.com/api/v1/international)
- [Production](https://liveapi.opaycheckout.com/api/v1/international)
- [Errors](https://documentation.opaycheckout.com/error-codes)
- [Signature Calculator](https://documentation.opaycheckout.com/signature-calculator)
- [OpenAPI](openapi/opay-cashier-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/opay-cashier-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/opay-cashier-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.opayweb.com/)
- [Portal](https://documentation.opaycheckout.com/)
- [Documentation](https://documentation.opaycheckout.com/)
- [Getting Started](https://documentation.opaycheckout.com/getting-started)
- [API Reference](https://documentation.opaycheckout.com/server-apis-overview)
- [Authentication](https://documentation.opaycheckout.com/payment-authentication)
- [Webhooks](https://documentation.opaycheckout.com/payment-notifications)
- [Errors](https://documentation.opaycheckout.com/error-codes)
- [Sandbox](https://testapi.opaycheckout.com/api/v1/international)
- [Sign Up](https://merchant.opaycheckout.com/register)
- [Console](https://merchant.opaycheckout.com/login)
- [Dashboard](https://merchant.opaycheckout.com/login)
- [Support](https://support.opaycheckout.com/support/ticket)
- [Business Solutions](https://opaybusiness.opayweb.com/)
- [GitHub Organization](https://github.com/opay)
- [SDK](https://github.com/opay/lib.gateway.php)
- [Plugin](https://documentation.opaycheckout.com/woocommerce)
- [Privacy Policy](https://www.opayweb.com/privacy-policy)
- [Terms of Service](https://www.opayweb.com/terms-and-conditions)
- [Twitter](https://twitter.com/OPay_NG)
- [LinkedIn](https://www.linkedin.com/company/opayinc/)
- [YouTube](https://www.youtube.com/@OPayNigeria)
- [Facebook](https://www.facebook.com/OPayNigeria/)
- [Instagram](https://www.instagram.com/opaynigeria/)
- [App Store](https://apps.apple.com/ng/app/opay-mobile-money-app/id1500386156)
- [Play Store](https://play.google.com/store/apps/details?id=team.opay.pay)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
