# Awesome-Merchant-Of-Record-Mor

# Top Merchant of Record (MoR) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Global Tax Compliance, Payment Infrastructure & Self-Hosted MoR Alternatives*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Merchant of Record (MoR)** services. These platforms act as the legal seller of your software or digital products, handling global sales tax, VAT, payment processing, invoicing, and compliance—so you can focus on building instead of navigating 140+ countries' tax regimes.

**Examples** include Shopify Markets Pro, Global-e, Digital River, Paddle, FastSpring, Nexway, Cleverbridge, 2Checkout (Verifone), MerchantSpring, and PayPro Global (the category leaders).

**Open-source emphasis**: Merchant of Record is a domain where open-source tooling is **exceptionally rare but has a clear leader**. **Polar** is the only mature open-source MoR platform available—an Apache-2.0 licensed engine that explicitly handles the MoR responsibilities of billing, receipts, customer accounts, sales tax, and VAT, with 7,400+ GitHub stars and active development . **Creem** maintains open-source SDKs and integrations for its commercial MoR service, but the core platform is not open-source . **Blooms** is an early-stage MIT-licensed attempt at a LemonSqueezy/Paddle alternative, but it is incomplete and not production-ready . No other open-source project replicates the full legal and tax infrastructure of Paddle or FastSpring—MoR status requires banking relationships, tax registrations, and regulatory compliance that software alone cannot provide.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Shopify Markets Pro](https://www.shopify.com/markets)**  
  Shopify's merchant-of-record solution for cross-border selling; handles international tax compliance, duties, and fraud prevention for merchants selling globally.

- **[Global-e](https://www.global-e.com/)**  
  Cross-border ecommerce platform acting as merchant of record for international sales; handles localization, tax, duties, and payment methods across 200+ markets.

- **[Digital River](https://www.digitalriver.com/)**  
  Global commerce and merchant of record provider for software, digital products, and subscriptions; handles tax, compliance, fraud, and payments across 240+ countries.

- **[Paddle](https://www.paddle.com/)**  
  Merchant of record for SaaS and digital products; handles global sales tax, VAT, subscription billing, and compliance; widely used by indie developers and SaaS companies.

- **[FastSpring](https://fastspring.com/)**  
  Merchant of record and ecommerce platform for software and SaaS; handles global tax, payments, subscriptions, and compliance; enterprise-focused with popup/embedded checkout .

- **[Nexway](https://www.nexway.com/)**  
  Merchant of record and digital commerce platform for software, games, and digital goods; handles global tax and payment processing.

- **[Cleverbridge](https://www.cleverbridge.com/)**  
  Merchant of record and ecommerce platform for software, SaaS, and digital goods; handles global tax, compliance, and subscription management.

- **[2Checkout (Verifone)](https://www.2checkout.com/)**  
  Merchant of record and payment platform (now Verifone) for digital goods and SaaS; handles global tax and compliance.

- **[MerchantSpring](https://www.merchantspring.com/)**  
  Merchant of record platform focused on simplifying global sales tax and compliance for digital businesses.

- **[PayPro Global](https://www.payproglobal.com/)**  
  Merchant of record and ecommerce platform for software and digital products; handles global tax, payments, and compliance.

## Open-Source GitHub Projects

### MoR Platforms (Self-Hosted)

- **[Polar](https://github.com/polarsource/polar)**  
  The only mature open-source **Merchant of Record** platform available (Apache 2.0, 7,401+ GitHub stars); explicitly designed as "an open source engine for your digital products" that handles the MoR responsibilities: **billing, receipts, customer accounts, sales tax, and VAT** . Features subscriptions, digital products, license keys, GitHub repository access, Discord support channel access, and file downloads. Pricing is 4% + 40¢ with no fixed monthly costs. Stack: Python/FastAPI backend, Next.js dashboard, PostgreSQL, Redis. **The clear starting point for organizations wanting a self-hosted MoR engine**—though it is a newer entrant compared to Paddle or FastSpring, and organizations must still handle the legal/tax registrations that underpin MoR status.

### MoR-Adjacent Projects (SDKs & Integrations)

- **[Creem SDKs](https://github.com/armitage-labs/creem)**  
  Open-source TypeScript SDKs and integrations for **Creem**, a commercial MoR service (not open-source itself). Packages include `creem` (full API coverage with MCP server), `creem_io` (lightweight wrapper), `@creem_io/nextjs`, `@creem_io/better-auth`, and `@creem_io/convex` . **Useful for developers integrating with Creem's MoR service**, but the core platform is proprietary.

- **[Blooms](https://github.com/im-Kazmi/Blooms-)**  
  Early-stage open-source attempt at a LemonSqueezy/Paddle alternative (MIT); features digital product sales, subscription management, license key generation, multi-currency support, and Stripe payment processing . Stack: Hono.js, Next.js, PostgreSQL, Prisma. **Not production-ready**—last pushed January 2025, SDK incomplete, and no community traction. Listed for completeness but **not recommended for production use**.

### Additional Strong Open-Source Options

- **No other open-source MoR exists** — The legal and tax infrastructure of MoR platforms (tax registrations in 100+ jurisdictions, banking relationships, fraud liability) is not replicable by software alone. Polar is the only viable open-source starting point , and even it requires the operator to establish the underlying legal entity and tax registrations.
- **Tax calculation engines** (Cbox Tax, nexus-tax) and **billing engines** (Recurso) provide adjacent capabilities but do not confer MoR status—they calculate or manage billing without acting as the legal seller .

**Frameworks for building custom systems**: **Polar** is the only open-source MoR engine that explicitly handles tax, billing, and customer accounts as a merchant of record . For organizations not ready to establish MoR status, **Recurso** provides billing and ledger infrastructure with tax calculation (India GST, EU VAT, US sales tax) but requires the operator to handle compliance . **Creem's SDKs** are useful if using their commercial MoR service . No open-source project replaces the legal entity and tax registration layer that defines a true MoR.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Merchant of Record platforms bear legal liability for tax collection and remittance; **self-hosting a MoR engine like Polar does not automatically confer MoR status**—the operator must establish the legal entity, tax registrations, and banking relationships required to act as merchant of record. Consult legal and tax advisors before assuming MoR responsibilities.
- **Open-source MoR is extremely limited**—Polar is the only mature option , and it is a newer entrant compared to established commercial MoRs like Paddle, FastSpring, or Digital River. Blooms is incomplete and not production-ready . Organizations requiring MoR services without the legal overhead should evaluate commercial platforms.
- Verify license terms for commercial use; Polar uses Apache 2.0 , and Creem's SDKs are open-source while the core service is proprietary .

---

**Made for SaaS founders, digital product sellers, payment engineers, and global commerce operators.**  
Let's make merchant of record infrastructure more open, but with clear eyes about the legal and tax registrations that software cannot replace.
