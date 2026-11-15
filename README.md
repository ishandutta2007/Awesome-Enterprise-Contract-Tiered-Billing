# Awesome-Enterprise-Contract-Tiered-Billing

# Top Enterprise Contract & Tiered Billing Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on Usage-Based Rating, Tiered Pricing Engines & Self-Hosted Monetization Infrastructure*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Enterprise Contract & Tiered Billing**. These tools help organizations model and bill complex pricing structures—tiered, stairstep, volume, usage-based, and hybrid contracts—covering everything from enterprise billing suites that handle multi-entity hierarchies to open-source engines that meter usage and enforce entitlements without per-subscriber fees.

**Examples** include Chargebee Enterprise, Zuora, Gotransverse, CSG International, Amdocs, Aria Systems, OpenMeter, and Autumn (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted metered billing, open-source tiered pricing engines, and community-driven subscription infrastructure—ideal for organizations seeking data sovereignty and avoiding percentage-of-revenue pricing that compounds as billing volume grows. The open-source landscape is genuinely emerging: **OpenMeter** provides a CNCF-sandbox metering and billing engine with tiered pricing support [citation:7], and **Autumn** offers an open-source layer between Stripe and your application for custom plans and overages [citation:14].

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Chargebee](https://www.chargebee.com/)** | Subscription and usage-based billing platform with **native support for Flat Fee, Tiered, Stairstep, Volume, Usage, and Seat-Based pricing models** [citation:1]. **Enterprise tier** is built for global scale with **multi-entity support, parent-child account hierarchies, and up to 500M usage events/month** [citation:1]. Performance tier at $7,188/year covers up to $100K billing/month [citation:8]. | Performance: **$7,188/year** (up to $100K/mo billing); Enterprise: **custom quote** [citation:8] | **Starter**: $0 for first $225K cumulative billing, then 0.75% [citation:15] |
| **[Zuora](https://www.zuora.com/)** | Enterprise subscription order-to-cash platform with **Growth, Enterprise, and Nine editions** [citation:9]. Supports consumption revenue recognition, usage overage handling, and complex contract modifications. **Zuora CPQ** and **Collections** are separate add-ons [citation:9]. **Enterprise edition** handles high-volume transactions with additional capacity purchasable. | Quote-only (edition-based; add-ons for CPQ, Collections) | No free tier; demo via sales |
| **[Gotransverse](https://www.gotransverse.com/)** | Cloud-based billing platform **specializing in usage-based pricing and monetization at large scale** [citation:10]. Users note the **Usage Rating Engine is powerful and advanced**, processing large volumes in real-time [citation:10]. **Pricing is not publicly disclosed**—SelectHub lists a starting range of $10–$100 with custom quote required [citation:3]. | Quote-only (custom; SelectHub range $10–$100) [citation:3] | **Free trial** available [citation:3] |
| **[CSG International](https://www.csgi.com/)** | Billing and revenue management for telecom and subscription businesses. **Supports subscription, usage, hybrid, and B2B2X models on a single platform** [citation:12]. Cloud-native, modular architecture with **real-time rating and charging** [citation:12]. Claims **85% faster service launches** and **80% reduction in third-party billing tools** [citation:12]. | Quote-only (enterprise contract) | No free tier; demo via sales |
| **[Amdocs](https://www.amdocs.com/)** | **ConnectX** platform with five price types (Upfront, Subscription, One-Time, Recurring, Usage) and multiple pricing methods including **Tier based and Volume based** . Supports conditional pricing and commitment fee waivers . | Quote-only (custom pricing via Microsoft Marketplace placeholder) [citation:11] | No free tier; demo via sales |
| **[Aria Systems](https://www.ariasystems.com/)** | Enterprise recurring and usage billing platform. Positioned for complex monetization at scale. | Quote-only (enterprise contract) | No free tier; demo via sales |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[OpenMeter](https://github.com/openmeterio/openmeter)** | [![Stars](https://img.shields.io/github/stars/openmeterio/openmeter?style=social&color=white)](https://github.com/openmeterio/openmeter/stargazers) | **The most complete open-source metering and billing engine for usage-based and tiered pricing.** Apache-2.0, CNCF Sandbox project [citation:7]. **Meters high-volume events, models products with versioned plans and flat/recurring/per-unit/tiered/package/dynamic prices, controls feature access and usage limits, and runs the invoice lifecycle** [citation:7]. **API-first** with REST API, JavaScript/Python/Go SDKs, and webhooks. Works with your existing payment and tax providers. **Trade-offs**: releases are beta and may include breaking changes; the local Docker Compose stack is for evaluation, not production topology [citation:7]. **Best for AI, API, and usage-based products** that need one source of truth for consumption without per-subscriber fees. |
| **[Autumn](https://github.com/Jellypod-Inc/autumn)** | [![Stars](https://img.shields.io/github/stars/Jellypod-Inc/autumn?style=social&color=white)](https://github.com/Jellypod-Inc/autumn/stargazers) | **Open-source pricing and billing layer between Stripe and your application.** Supports **subscriptions, credit systems and top-ups, usage-based models with overages, and custom plans for large customers** [citation:14]. **Three core functions** handle all billing logic: `/attach` (purchase flows), `/check` (feature access and usage limits), and `/track` (record usage events) [citation:14]. **Decouples billing logic from app logic**—pricing changes don't require DB migrations or rebuilding in-app flows. **Trade-offs**: depends on Stripe for payments; self-hosting requires multiple services and team assistance for local instances [citation:14]. **Best for teams wanting Stripe-native custom pricing** without building metering and entitlement logic from scratch. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Chargebee Starter (Free Tier)](https://www.chargebee.com/pricing/)** | — | **Not open-source, but the most accessible free entry point for tiered billing.** **$0 for first $225K cumulative billing**, then 0.75%—pay-as-you-go with no annual commitment [citation:15]. Supports all pricing models including Tiered, Stairstep, Volume, and Usage [citation:1]. **Best for validating tiered billing before committing to a paid plan.** |

**Frameworks for building custom systems**: Choose **OpenMeter** for a CNCF-backed metering engine with tiered pricing and entitlement enforcement [citation:7], or **Autumn** for a Stripe-native billing layer with custom plans and overages [citation:14] —both without per-subscriber or percentage-of-revenue fees that compound as billing volume grows.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Enterprise billing platforms handle payment credentials and financial data; enforce PCI DSS compliance, audit logging, and reconciliation controls. **Tiered pricing calculation errors can cause revenue leakage or customer disputes.**
- **Pricing transparency varies dramatically in this category.** **Chargebee publishes tiered plan structures** with a free starter tier and Performance at $7,188/year [citation:8][citation:15]. **Gotransverse, Zuora, CSIG, Amdocs, and Aria Systems are quote-only**—Gotransverse's SelectHub listing shows a $10–$100 range but acknowledges specific pricing is not publicly disclosed [citation:3]. **Open-source tiered billing is genuinely emerging but not yet mature.** **OpenMeter is CNCF Sandbox** with a powerful metering engine, but its releases are **beta and may include breaking changes**—the Docker Compose stack is explicitly for evaluation, not production [citation:7]. **Autumn decouples billing logic from app code** but depends on Stripe and requires multiple services to self-host [citation:14]. **Validate tier boundary logic, proration handling, and invoice accuracy** against your actual contract structures before committing.

---

**Made for revenue operations teams, billing engineers, and organizations building monetization infrastructure.**  
Let's make enterprise contract and tiered billing more open, accurate, and cost-predictable.
