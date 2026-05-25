# OPay (opay)

OPay is a Nigerian mobile money and fintech super-app operated by Blue Ridge Microfinance Bank (OPay Digital Services Limited) and majority-owned by Opera Limited with backing from SoftBank Vision Fund 2, Sequoia China, DragonBall Capital, and 9F Group. Launched in 2018 and headquartered in Lagos, OPay serves tens of millions of Nigerian consumers, merchants, and agents with wallet accounts, free interbank transfers, the OPay Debit Card, OWealth (daily-interest savings powered by OPay Microfinance Bank), bill payments, airtime/data top-ups, BNPL (OBuy / OPay Easy Buy), and the OPay POS / agent banking network. For developers and merchants, OPay exposes the OPay Cashier / OPay Checkout API — a REST API for accepting payments via 3DS bank cards, bank transfer, USSD, bank account, POS, OPay wallet QR, and reference codes, with hosted Express Checkout, server-to-server APIs, callback webhooks, refund and query operations, a PHP gateway SDK, and a WooCommerce plugin.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/opay/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Payments, Mobile Money, Fintech, Super App, Nigeria, Africa, Wallet, Savings, BNPL, Bank Transfer, Card Payments, USSD, Agent Banking, POS, Bill Payments, Airtime, Cashier, Checkout, Merchant Acquiring

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### OPay Cashier API

The OPay Cashier API is the primary merchant payment API behind OPay Checkout. It exposes a hosted Express Checkout endpoint (`cashier/create` returning a `cashierUrl`), server-to-server payment creation for 3DS bank cards, bank transfer, bank USSD, bank account, POS, OPay wallet QR, and reference code payments, plus status queries, cancel, refund, and refund-status operations. Authentication uses an Authorization Bearer token — the public key for `cashier/create` and an HMAC-SHA512 signature over the JSON body (signed with the merchant's private key) for all other endpoints — along with a `MerchantId` header.

**Human URL:** [https://documentation.opaycheckout.com/](https://documentation.opaycheckout.com/)

**Base URL:** `https://liveapi.opaycheckout.com/api/v1/international` (production) / `https://testapi.opaycheckout.com/api/v1/international` (sandbox)

#### Tags

 - Payments, Cashier, Checkout, Cards, Bank Transfer, USSD, Wallet, Refunds

#### Properties

- [Documentation](https://documentation.opaycheckout.com/)
- [GettingStarted](https://documentation.opaycheckout.com/getting-started)
- [Authentication](https://documentation.opaycheckout.com/payment-authentication)
- [APIReference](https://documentation.opaycheckout.com/server-apis-overview)
- [Webhooks](https://documentation.opaycheckout.com/payment-notifications)
- [Sandbox](https://testapi.opaycheckout.com/api/v1/international)
- [Errors](https://documentation.opaycheckout.com/error-codes)
- [SignatureCalculator](https://documentation.opaycheckout.com/signature-calculator)
- [OpenAPI](openapi/opay-cashier-api-openapi.yml)

## Common Properties

- [Website](https://www.opayweb.com/)
- [Portal](https://documentation.opaycheckout.com/)
- [SignUp](https://merchant.opaycheckout.com/register)
- [Console](https://merchant.opaycheckout.com/login)
- [Support](https://support.opaycheckout.com/support/ticket)
- [Business Solutions](https://opaybusiness.opayweb.com/)
- [GitHub Organization](https://github.com/opay)
- [SDK — OPay PHP Gateway Library](https://github.com/opay/lib.gateway.php)
- [Plugin — WooCommerce](https://documentation.opaycheckout.com/woocommerce)
- [PrivacyPolicy](https://www.opayweb.com/privacy-policy)
- [TermsOfService](https://www.opayweb.com/terms-and-conditions)
- [Twitter](https://twitter.com/OPay_NG)
- [LinkedIn](https://www.linkedin.com/company/opayinc/)
- [YouTube](https://www.youtube.com/@OPayNigeria)
- [App Store](https://apps.apple.com/ng/app/opay-mobile-money-app/id1500386156)
- [Play Store](https://play.google.com/store/apps/details?id=team.opay.pay)

## Features

| Name | Description |
|------|-------------|
| Express Checkout | Hosted, OPay-branded checkout page returned via `cashier/create` — customers complete payment on OPay-managed UI and are redirected back to the merchant `returnUrl`. |
| 3DS Card Payments | Direct server-to-server card acceptance with 3-D Secure step-up (`REDIRECT_3DS` nextAction) for Nigerian and international card schemes. |
| Bank Transfer | Generate a dynamic virtual account (`transferAccountNumber` + `transferBankName`) per order; OPay reconciles inbound transfer and settles the merchant. |
| Bank USSD Payment | Customer pays by dialling a `*USSD*` code on their mobile phone; common in Nigeria where USSD banking is dominant. |
| Bank Account Payment | Direct debit from the customer's bank account. |
| POS Payment | Card-present payment from an OPay POS terminal. |
| OPay Wallet QR Payment | Customer scans a QR code in the OPay app to pay from their wallet. |
| Reference Code Payment | Customer pays at an OPay agent using a reference code. |
| Refunds | Full or partial refunds with refund status query. |
| Payment Status Query | Synchronous query for order status by merchant reference or OPay orderNo. |
| Callback Webhooks | Server-to-server callback notifications on terminal transaction state changes (SUCCESS, FAIL, CLOSE), signed and retried by OPay. |
| HMAC-SHA512 Signature Authentication | All non-cashier-create endpoints authenticate via a SHA-512 HMAC signature over the JSON body using the merchant's private key, plus a `MerchantId` header. |
| Sandbox Environment | `testapi.opaycheckout.com` sandbox with trigger-error-by-amount testing. |
| WooCommerce Plugin | Drop-in WooCommerce plugin for WordPress storefronts. |
| PHP Gateway SDK | Official open-source PHP gateway library at `github.com/opay/lib.gateway.php`. |

## Use Cases

| Name | Description |
|------|-------------|
| Nigerian E-commerce Checkout | Accept local payment methods (card, bank transfer, USSD, OPay wallet) on Nigerian e-commerce sites via Express Checkout or server APIs. |
| Cross-Border Online Merchants | Sell into Nigeria from international storefronts via OPay International APIs. |
| Marketplace Payouts | Pay agents, riders, and sellers via OPay transfers. |
| Bill Payment & Airtime Aggregation | Top up airtime/data and pay utility bills from within partner apps. |
| Wallet Top-Up | Fund OPay wallets from cards or bank transfers. |
| Buy-Now-Pay-Later Checkout | Offer BNPL via OBuy / OPay Easy Buy at checkout. |
| Agent Banking & Cash-In/Cash-Out | Leverage the OPay agent network for cash deposits and withdrawals. |
| POS Acceptance | Card-present acceptance via OPay POS terminals. |

## Integrations

| Name | Description |
|------|-------------|
| WooCommerce | Official OPay WooCommerce plugin for WordPress. |
| Opera Browser | OPay was originally incubated inside Opera Limited and integrates with Opera browser payment flows. |
| Visa | Card acquiring on the Visa network. |
| Mastercard | Card acquiring on the Mastercard network. |
| Verve | Card acquiring on the Nigerian Verve network. |
| Nigerian Interbank Settlement System (NIBSS) | Bank transfer rails and USSD banking via NIBSS. |
| Wema Bank | Partner bank for virtual-account bank-transfer settlement (referenced in API responses). |

## Solutions

| Name | Description |
|------|-------------|
| OPay Personal App | Consumer super-app for wallet, transfers, OWealth savings, debit card, bill pay. |
| OPay Business | Merchant suite — Cashier API, POS terminals, agent banking, payouts. |
| OWealth | Daily-interest savings powered by OPay Microfinance Bank Limited (CBN licensed, NDIC insured). |
| OPay Debit Card | Instant-issuance debit card accepted on ATM, POS, and online. |
| OBuy / OPay Easy Buy | Buy-now-pay-later product for OPay app users. |
| OPay POS | POS terminal network for merchants and agents. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [OPay Cashier API](openapi/opay-cashier-api-openapi.yml)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
