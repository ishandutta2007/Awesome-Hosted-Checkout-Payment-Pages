# Awesome-Hosted-Checkout-Payment-Pages

# Top Hosted Checkout & Payment Pages Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on PCI-Compliant Payment Pages, Merchant of Record Models & Self-Hosted Checkout Infrastructure*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Hosted Checkout & Payment Pages**. These tools provide pre-built, PCI-compliant payment interfaces that merchants can redirect customers to—covering everything from Stripe's industry-standard Checkout to open-source payment hosts that eliminate platform commissions and give you full control over the checkout experience.

**Examples** include Stripe Checkout, PayPal Checkout, Square Online Checkout, Shopify Checkout, Adyen Hosted Checkout, Braintree Hosted Fields, and open-source alternatives like Open Payment Host (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted checkout, open-source payment infrastructure, and community-driven merchant tooling—ideal for sellers seeking to avoid double commissions and maintain full ownership of their checkout flow and customer data. The open-source landscape is genuinely emerging: **Open Payment Host** provides a self-hosted Go service for selling digital or physical goods without the marketplace fees charged by Gumroad or Ko-fi .

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Stripe Checkout](https://stripe.com/payments/checkout)** | **The benchmark for hosted checkout.** Pre-built, PCI-compliant payment page with support for cards, wallets, and 40+ payment methods. **Base processing: 2.9% + 30¢**; **Billing adds 0.7% of recurring volume**; **Tax adds 0.5% per transaction**; **international cards +1.5%**; **currency conversion +1%** . | Processing: **2.9% + 30¢**; Billing: **0.7%** of billing volume | No monthly fee for Checkout; pay-per-transaction |
| **[PayPal Checkout](https://www.paypal.com/)** | **Highest consumer recognition in many markets.** **Standard card payments: 2.99% + 49¢**; **PayPal Checkout (wallet): 3.49% + 49¢** in the US (Oct 2026). **No separate subscription fee**—each recurring payment charged at the payment type rate; optional Recurring Billing is $10/month . **Currency conversion: 3–4% spread** on top of transaction fees . | Wallet: **3.49% + 49¢**; Card: **2.99% + 49¢** | No monthly fee for basic checkout |
| **[Square Online Checkout](https://squareup.com/)** | **Simple hosted checkout with a free plan.** **Free plan: 2.8% + 30¢ per transaction** with no monthly fee. **Plus: $36/month (2.6% + 30¢)**; **Premium: $99/month (2.5% + 30¢)** . EU/EEA cards: **1.4% + 25¢ + VAT** for Online Checkout . | Free: **2.8% + 30¢**; Plus: **$36/mo** | **Free plan**: no monthly fee, full online store builder |
| **[Shopify Checkout](https://www.shopify.com/)** | **Fully managed checkout tied to Shopify stores.** **Basic: $29/month + 2.9% + 30¢** (Shopify Payments); **Advanced: $299/month + 2.5% + 30¢** . **Third-party gateways add 0.6%–2% extra**—at $400K/month volume, that's **$28,800/year** in avoidable fees . | Basic: **$29/mo**; Advanced: **$299/mo** | Free trial available; no free plan |
| **[Adyen Hosted Checkout](https://www.adyen.com/)** | Enterprise payment platform with hosted checkout pages. **Interchange-plus pricing**—cheaper for high-ticket or B2B transactions where a small markup difference is worth real money . | Quote-only (interchange-plus) | No free tier; demo via sales |
| **[Braintree Hosted Fields](https://www.braintreepayments.com/)** | **Hosted fields for custom checkout forms** (not a full redirect). **$15 per chargeback**; **Drop-in SDK deprecated October 1, 2026**—migrate to Hosted Fields or alternative . | Quote-only (per-transaction) | No free tier; sandbox available |
| **[Chargebee Checkout](https://www.chargebee.com/)** | **Subscription billing platform with hosted checkout pages.** Integrates with Stripe, Braintree, PayPal, and other gateways. **Starting price: $299/month** . Positioned for SaaS businesses needing subscription management alongside checkout. | From **$299/month** | No free tier; trial via sales |
| **[Bold Checkout (Subscriptions)](https://www.boldcommerce.com/)** | **Subscription checkout for Shopify.** **Launch: $24.99/month + 2% transaction fee**; **Grow: $49.99 + 1%**; **Scale: $74.99 + 0.9%**; **Ultimate Retention: $399 + 0.9%** . **30-day free trial** (transaction fees still apply) . | Launch: **$24.99/mo + 2%**; Grow: **$49.99 + 1%** | **30-day free trial** |
| **[Mollie Checkout](https://www.mollie.com/)** | **European payment provider with blended pricing.** **Startup program: fee exemption up to €1,000,000** depending on funding level. **Volume discounts** for businesses processing over €100,000/month . | Blended per-transaction rate | **Startup program**: fee exemption up to €1M |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Open Payment Host](https://github.com/abishekmuthian/open-payment-host)** | [![Stars](https://img.shields.io/github/stars/abishekmuthian/open-payment-host?style=social&color=white)](https://github.com/abishekmuthian/open-payment-host/stargazers) | **The most complete open-source self-hosted checkout and payment host.** **Go-based**, **243 GitHub stars**, actively maintained (last push September 2026) . **Self-hosted alternative to Gumroad, Buy Me a Coffee, and Ko-fi**—sell digital or physical goods without **double commissions** . **Ready-to-use checkout, billing, and PSP integration APIs**: `/checkout/create`, `/subscription/create`, and webhook handling . **Bring your own PSP** (Stripe sandbox for testing, production keys for live) . **Docker Compose deployment**; PostgreSQL/MySQL support . **Trade-off**: **Medium production readiness**—suitable for prototypes, internal tools, or low-to-moderate traffic after validation; run `go vet`/`staticcheck` and review dependencies before critical production use . **Best for sellers wanting full control over their revenue stream** without marketplace fees eating into margins . |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| *(No other mature open-source hosted checkout projects identified in search results)* | — | The open-source checkout landscape is thin compared to commercial SaaS. Open Payment Host is the primary self-hosted option; most open-source payment tooling focuses on libraries (Stripe SDKs, PayPal APIs) rather than turnkey hosted checkout pages. |

**Frameworks for building custom systems**: The open-source path to hosted checkout is **bring-your-own-PSP**. **Open Payment Host** provides the checkout page, subscription logic, and webhook handling—you plug in Stripe, PayPal, or any PSP for actual processing . This eliminates marketplace commissions (Gumroad, Ko-fi) while keeping you in control of the customer relationship and data. **No open-source project replicates Stripe's 40+ payment methods or Shopify's managed tax/shipping integrations**—expect to build those layers or accept narrower scope.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Hosted checkout platforms handle payment card data and customer PII; **PCI DSS compliance is mandatory**—using a hosted checkout page (Stripe, PayPal, Square) transfers most PCI burden to the provider, while self-hosted solutions require you to validate compliance scope.
- **Hosted checkout fees compound in ways the headline rate hides.** **Stripe's 2.9% + 30¢ is only the base**—Billing adds 0.7%, Tax adds 0.5%, international cards add 1.5%, and currency conversion adds 1%, pushing effective rates toward **5–6% for global subscription businesses** . **PayPal's wallet rate is 3.49% + 49¢**—20% higher than Stripe on a $100 transaction—plus a **3–4% currency conversion spread** that costs $1,500–$2,000/month on $50K in international sales . **Shopify's third-party gateway penalty adds 0.6%–2%**—at $400K/month volume, using a non-Shopify gateway costs **$28,800/year** in avoidable fees . **Square offers the most accessible free tier** (no monthly fee, 2.8% + 30¢) . **Open Payment Host eliminates platform commissions** but is **medium production readiness**—validate stability, security, and PSP integration before relying on it for critical revenue . **Validate whether you need managed convenience (Stripe, Shopify), enterprise interchange-plus (Adyen), or self-hosted control (Open Payment Host)** before committing.

---

**Made for merchants, developers, and businesses building payment infrastructure.**  
Let's make hosted checkout and payment pages more open, transparent, and merchant-friendly.
