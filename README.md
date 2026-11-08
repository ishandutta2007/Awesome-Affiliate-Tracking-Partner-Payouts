# Awesome-Affiliate-Tracking-Partner-Payouts

# Awesome-Affiliate-Tracking-Partner-Payouts
**Top Affiliate Tracking Partner Payouts (Opensource) 🌟 Star if you like it! 🌟**

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Click Attribution, Commission Management, Fraud Detection & Self-Hosted Partner Payouts*
**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Affiliate Tracking & Partner Payouts**. These tools enable businesses to run their own affiliate and partner programs—tracking clicks, attributing conversions, calculating commissions, and paying partners—from fully managed SaaS platforms with marketplace discovery to open-source engines that give organizations full control over their partner data and payout logic.

**Examples** include Chargebee Affiliate Management, Impact.com, PartnerStack, Everflow, TUNE, Rewardful, Tapfiliate, FirstPromoter, Refersion, and LeadDyno (the category leaders in commercial space).

**Open-source emphasis**: This section is expanded with every relevant project for self-hosted affiliate tracking, commission engines, and open payout infrastructure. **Critical note**: The open-source landscape has matured significantly—**AffiliateTracking** is the most complete open-source alternative to Rewardful and FirstPromoter, with fraud rules, double-entry commission ledgers, and PayPal/Wise payout files . **Simple KUMA** focuses on media-buyer tracking with cost sync from Meta and Google Ads . **Numok** offers a stable Stripe-integrated affiliate platform . No open-source project matches Impact.com's partner discovery or PartnerStack's ecosystem depth, but for core tracking and payouts, the options are production-capable.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **Impact.com**
  **Enterprise partnership management** platform with affiliate tracking, influencer programs, and fraud detection. **Pricing**: **Pro from $500/month**; Enterprise quote-only . **Free tier**: None. **Best for**: large brands managing complex partner ecosystems across affiliates, influencers, and B2B partners—**trade-off**: enterprise pricing; implementation complexity.

- **PartnerStack**
  **Partner ecosystem platform** for SaaS companies with affiliate, reseller, and referral programs. **Pricing**: Quote-only; tiered by partner volume . **Free tier**: None. **Best for**: SaaS businesses building channel and affiliate partner programs—**trade-off**: sales-led evaluation.

- **Everflow**
  **Partner marketing platform** with real-time analytics and fraud prevention. **Pricing**: Quote-only. **Free tier**: None. **Best for**: performance marketers and networks needing granular tracking and attribution—**trade-off**: quote-only; enterprise focus.

- **Rewardful**
  **Affiliate and referral software for Stripe-native SaaS**. **Pricing**: **Starter $49/month** (covers up to $7,500 monthly affiliate revenue); **Growth $99/month**; **Enterprise** custom. **Managed Payouts** adds **3% processing fee** on payouts . **Free tier**: 14-day trial. **Best for**: Stripe subscription businesses wanting simple affiliate tracking—**trade-off**: revenue-band caps force upgrades as you grow.

- **Tapfiliate**
  **Affiliate tracking software** with customizable commissions and partner portals. **Pricing**: **Launch $89/month** or **$890/year**; **Scale $179/month** or **$1,790/year**; Enterprise custom . **Free tier**: 7-day trial (Launch) or 14-day trial (Scale). **Best for**: e-commerce and SaaS businesses wanting flexible affiliate program management—**trade-off**: click/conversion metering on lower tiers.

- **FirstPromoter**
  **Affiliate and referral tracking for SaaS** with multiple billing integrations. **Pricing**: **Starter $49/month**; **Business $99/month**; **Enterprise** custom . **Free tier**: Trial available. **Best for**: SaaS founders wanting affiliate tracking across Stripe and other billing providers—**trade-off**: campaign limits on Starter.

- **Refersion**
  **Affiliate marketing software** for e-commerce with Shopify and BigCommerce integrations. **Pricing**: **Freemium** marketplace listing; **Growth** and **Scale** tiers available; paid plans start at **$39/month** . **Free tier**: Yes, marketplace listing. **Best for**: e-commerce merchants wanting affiliate management within their stack—**trade-off**: paid tiers required for advanced tracking and API access.

- **Chargebee Affiliate Management**
  **Affiliate tracking within Chargebee** billing platform. **Pricing**: Included with Chargebee subscriptions; quote-based for advanced. **Free tier**: Limited. **Best for**: Chargebee customers wanting affiliate tracking tied to subscription billing—**trade-off**: requires Chargebee billing platform.

- **TUNE**
  **Partner marketing platform** (formerly HasOffers) with network and advertiser solutions. **Pricing**: Quote-only. **Free tier**: None. **Best for**: affiliate networks and large advertisers needing scalable tracking infrastructure.

- **LeadDyno**
  **Affiliate marketing and referral tracking** for e-commerce and SaaS. **Pricing**: Tiered by monthly revenue and affiliates; quote-based. **Free tier**: Trial available. **Best for**: SMBs wanting affiliate tracking with referral program features.

## Open-Source GitHub Projects

- **AffiliateTracking (affiliate-engine)**
  **Open-source affiliate tracking software you host yourself** (AGPL-3.0) — **the most complete open-source alternative to Rewardful, FirstPromoter, Tapfiliate, and Tolt** found in this research . **Features**: **Affiliate links and coupon codes**; **Sales from Stripe, Paddle, Chargebee, Lemon Squeezy, Polar, and Recurly**; **Recurring commissions, refunds, and chargebacks** handled automatically; **13 fraud rules**—self-referrals, click floods, coupon hijacking, bot and datacenter traffic; flagged commissions held before payout; **double-entry commission ledger** so partners see how their balance adds up; **payouts in batches** with PayPal and Wise bulk-pay files and tax form collection; **multi-tier commissions**, usage-based commissions, and partner leaderboards; **JSON API with scoped keys** plus **MCP server** for AI assistants; **GDPR export and erasure** . **Performance**: ~10,000 affiliate link redirects/second in load testing; SQLite built in, Postgres supported when you outgrow it . **Tech stack**: Go, SQLite/Postgres. **Deploy**: Single binary or Docker (`ghcr.io/thebigasif/affiliate-engine:latest`) . **Trade-off**: **Newer project**—community validation limited compared to SaaS platforms; Shopify/WordPress integrations are separate products not in the repo . **Best for**: SaaS and e-commerce businesses wanting full control over affiliate data and payouts without per-revenue fees or vendor lock-in.

- **Simple KUMA**
  **Self-hosted affiliate and media-buyer tracking** (AGPL-3.0) — **the most feature-rich open-source tracker for performance marketers**, built with PHP + MySQL for shared hosting or VPS . **Features**: **Campaign management** with multi-step wizard; **traffic sources** with token mapping (Facebook, Google/YouTube, TikTok, native, custom); **landing pages and offers** with weighted/rotation flows; **postbacks and pixels** for conversions; **Meta/Facebook cost sync** and **Google Ads API cost sync**; **pre-aggregated stats tables** for speed at scale; **REST API** with Bearer keys for CRUD and reporting; **GeoIP and device detection** bundled; **dark mode** admin UI; CSRF protection and login rate limiting . **Tech stack**: PHP, MySQL/MariaDB. **Deploy**: Self-hosted (web server with document root at `public/`) . **Trade-off**: **Media-buyer focused**—built for tracking paid traffic and affiliate campaigns, not SaaS partner programs with recurring commissions or partner portals . **Best for**: performance marketers and media buyers wanting a self-hosted tracker with ad platform cost sync, without SaaS subscription fees.

- **Numok**
  **Open-source affiliate program platform with Stripe integration** (open source, stable v1.0.0) — **the most stable open-source Stripe-native affiliate platform** . **Features**: **Full affiliate platform**—tracking and commission management; **Stripe integration** with real-time webhook support; **admin dashboard** for programs, partners, and analytics; **partner portal** for affiliates to track performance and earnings; **Docker support** for easy deployment; **stable API and database schema** with migration support . **Tech stack**: PHP 8.1+, MySQL. **Deploy**: Docker (recommended) or manual installation . **Trade-off**: **Stripe-only billing integration**—no Paddle, Chargebee, or other billing providers; smaller feature set than AffiliateTracking (no fraud rules or MCP server) . **Best for**: SaaS businesses on Stripe wanting a stable, self-hosted affiliate platform with partner portal—without the complexity of a full tracking suite.

- **Capve**
  **Open-source, self-hosted affiliate tracking for indie and SaaS founders** (open source) — **the most modern Cloudflare-native tracking option**, deployable on Cloudflare's edge . **Features**: **Unique tracking links and click-through cookies**; **server-side conversion attribution**; **MCP server**—connect Claude Code, Cursor, or VS Code to manage campaigns, affiliates, reports, and team by chat (92 tools); **anti-fraud blocklists**, postbacks, traffic source templates, and drilldown reports; **email/password auth** with rate limiting . **Tech stack**: React, Cloudflare Workers, D1. **Deploy**: Cloudflare (one Worker + static assets) . **Trade-off**: **Cloudflare-dependent**—not a traditional VPS deployment; newer project with limited validation; no built-in payout file generation like AffiliateTracking . **Best for**: indie developers and SaaS founders already on Cloudflare wanting lightweight affiliate tracking with AI-agent management via MCP.

- **RefRef**
  **Open-source referral and affiliate platform** (open source) — **the most focused open-source referral marketing platform**, positioned as an alternative to Refersion and Tolt . **Features**: **Referral marketing** with commission flows; **self-hosted** deployment; **free tier** available; **SaaS dashboard** for managing programs . **Tech stack**: Per repository. **Deploy**: Self-hosted. **Trade-off**: **Smaller project** with limited public documentation in search results; less feature depth than AffiliateTracking or Simple KUMA . **Best for**: developers wanting a lightweight open-source referral platform foundation—willing to evaluate an early-stage project.

### Additional Strong Open-Source Options

- **django-referral-system** — Django library for referral tracking (MIT) . **Note**: **Library, not an app**—you bring the Django project and frontend; provides promoters, referral tracking, payouts, and Wise CSV export . **Best for**: Django developers wanting to embed referral tracking in their own application.
- **Dub** — Link tracking with partner program (AGPL-3.0 core; partner program under commercial ee licence) . **Note**: **Partner program is commercially licensed**—only link tracking and analytics are open source . **Best for**: teams wanting open-source link tracking with a paid partner program option.

**Frameworks for building custom systems**: Combine **AffiliateTracking** for full affiliate tracking and payouts with **Simple KUMA** for media-buyer cost tracking and **Numok** for a Stripe-native partner portal—creating a layered open-source affiliate stack. **None of these match Impact.com's partner discovery or PartnerStack's ecosystem depth**, but for core tracking, fraud detection, and payouts, the options are production-capable.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Affiliate tracking platforms handling partner data and commissions must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate fraud prevention and disclosure practices.
- **The "full affiliate platform" vs. "media-buyer tracker" vs. "Stripe-native" vs. "Cloudflare-native" distinction is critical.** **AffiliateTracking** is a **full affiliate platform**—tracking, fraud rules, commission ledger, payouts, and partner portal . **Simple KUMA** is a **media-buyer tracker**—click/cost/conversion tracking for paid traffic, not SaaS partner programs . **Numok** is **Stripe-native**—affiliate tracking tied to Stripe subscriptions . **Capve** is **Cloudflare-native**—edge-deployed tracking with MCP integration . **Choose based on whether you need full affiliate operations, media buying, Stripe integration, or edge deployment.**
- **AffiliateTracking is the most complete open-source alternative**—13 fraud rules, double-entry ledger, PayPal/Wise payout files, and MCP server . **The trade-off**: newer project; Shopify/WordPress integrations are separate products.
- **Simple KUMA is for media buyers, not SaaS affiliates**—it tracks clicks, costs, and conversions for paid traffic campaigns, with Meta and Google Ads cost sync . **Do not evaluate it for recurring SaaS commissions or partner portals.**
- **Numok is stable and Stripe-integrated**—v1.0.0 with partner portal and Docker deployment . **The trade-off**: Stripe-only; no multi-billing support like AffiliateTracking.
- **Rewardful and FirstPromoter are the SaaS benchmarks**—$49/month entry, but revenue-band caps force upgrades as affiliate revenue grows . **A program at $6K/month attributed revenue pays $990/year on FirstPromoter but $490 on Rewardful—model your growth.**
- **Tapfiliate's tiered pricing** ($89–$179/month) meters clicks and conversions—**model your volume before choosing a tier** .
- Self-hosted open-source solutions require proper infrastructure (Go for AffiliateTracking, PHP/MySQL for Simple KUMA and Numok, Cloudflare for Capve), security hardening, and ongoing maintenance. **Affiliate data includes partner PII and payment information**—ensure your deployment meets your organization's privacy and compliance requirements before processing live commissions.

---

**Made for affiliate managers, growth teams, and organizations building transparent partner tracking solutions.**
Let's make Affiliate Tracking & Partner Payouts more open, data-driven, and fraud-resistant.
