# soax review: What the Plan Prices Really Mean, Who Should Pay $200 a Month, and When a Cheaper Pay-As-You-Go Proxy Wins

Searching for a "soax review" usually means one of two things: you want to know whether SOAX is legit and fast, or you saw a per-GB number somewhere and you're trying to work out whether the bill will match it. The second question is the one that trips people up, because SOAX does not sell gigabytes the way most proxy providers do. It sells credits, and the rate at which those credits drain depends on which countries your traffic routes through. That single design choice changes the math for small projects more than any performance benchmark.

This review covers what SOAX actually is, what its published plan table looks like, where the pricing model hurts, and how a pay-as-you-go provider like DataImpulse compares for the workloads most people searching for a SOAX review actually have.

## What SOAX is, in one paragraph

SOAX is a UK-headquartered proxy provider (London) founded in 2019, with a team of around 60 people spread across several countries. It reports a pool of 155M+ IPs across 195+ countries, and sells four proxy types: residential, mobile, ISP (US-only) and datacenter. The company leans hard on ethical sourcing and compliance as positioning — residential nodes come through partner apps where users opt in, and the platform runs KYC checks before you can push traffic through it.

PCMag's 2025 review praised the dashboard and the monthly package structure, and noted a detail worth repeating: SOAX accounts use email plus a one-time code rather than a password. The same review also flagged that SOAX declined to name the apps its residential bandwidth comes from, and that its terms of service explicitly do not guarantee unique IP availability for targeting below country level. Both are small print items that matter if you're planning city- or ISP-level precision.

## The pricing model is the review

Here's the part worth slowing down for. SOAX publishes plans in credits, and one credit equals one dollar. The plan fee is essentially a prepayment; what the plan actually buys you is a lower per-GB rate on the traffic your credits pay for. And that rate is also governed by a three-tier country system.

- **Tier 1** (32 countries including the US, UK, Canada, Germany, Japan, Australia) is the most expensive per GB.
- **Tier 2** is roughly 60 countries, Brazil and India among them.
- **Tier 3** covers everything else and is the cheapest.

SOAX's own developer FAQ says routing through Tier 1 instead of Tier 3 can cost up to 8× more per GB on the same plan. So "SOAX costs $3/GB" and "SOAX costs $0.35/GB" can both be true statements about the same account on the same day, depending on where the traffic goes.

### SOAX published plans (Tier 1 rate)

| Plan | Monthly price | Tier 1 cost per GB | Notes |
| --- | --- | --- | --- |
| Sandbox | $0 | $5.00/GB | Starts automatically at signup; $25 minimum top-up; limited to 1 package and 1 seat |
| Builder | $200 | $3.00/GB | Cheapest plan with a monthly fee |
| Team | $500 | $2.20/GB |  |
| Scale | $1,500 | $1.50/GB |  |
| Enterprise | $3,000 | from $0.85/GB (Tier 1) | Headline rates of $0.25–$0.35/GB apply to Tier 3 traffic at this level |

A few things fall out of that table.

The cheapest paid plan is **$200 a month plus VAT**. There is no $20-a-month entry tier. If your project needs 10 GB of US traffic, you're on the Sandbox plan at $5/GB, which is $50 — or you commit to the $200 Builder plan and watch $200 of credits drain at $3/GB, which is about 66 GB of Tier 1 traffic. Paying $200 to move 10 GB works out to an effective $20/GB. That's the trap a lot of "SOAX pricing" summaries leave out.

Credits expire. SOAX states credits are valid for 60 days on monthly billing and 365 days on annual billing. Competitors like Bright Data and Oxylabs have their own rollover rules, but a 60-day window is on the tight end, and it's one of the few places where SOAX is unusually explicit about an unfavourable term.

The advertised floor isn't reachable for most buyers. The lowest figure printed on the pricing page is reserved for Enterprise customers routing Tier 3 traffic. Someone who needs US or UK IPs never gets near it.

To put the practical cost in context: at the Team rate of $2.20/GB, 500 GB of Tier 1 traffic works out to roughly $1,100 a month. Shifter's published benchmark uses the same arithmetic and arrives at the same number.

## What you get for the money

SOAX isn't selling a bad product at a bad price. It's selling an enterprise-shaped product at an enterprise-shaped minimum.

**Targeting and session control.** Country, region, city, ISP and ASN-level targeting are available, with sticky sessions configurable via port. The dashboard exposes per-package request-per-second and concurrency limits, and hitting either returns a 429 rather than degrading silently.

**Compliance machinery.** KYC verification, pre-approved use cases, abuse monitoring, GDPR and CCPA compliance statements. SOAX's trust page says it is working toward SOC 2 and ISO 27001 certifications, which is not the same as holding them, and worth reading literally.

**Support.** Live chat and email during UK business hours, plus a 24/7 chatbot. PCMag's tester described a polite, prompt email response during business hours and an after-hours interaction where a human picked up the chat — pleasant, though a round-the-clock human support line is something some competitors do offer.

**Trial options.** SOAX markets a $1.99 three-day trial with 400 MB of traffic on its residential product page. Its developer FAQ, meanwhile, describes the Sandbox plan as starting automatically with no time limit and a $25 minimum top-up. Either way, you can test before committing — just don't expect a free tier with real volume behind it.

## Who should actually pay for SOAX

SOAX makes sense if several of these are true at once: your monthly volume is in the hundreds of gigabytes or more, a meaningful share of your traffic is mobile or ISP-based, you need KYC-compliant vendor paperwork, and you want a single invoice with a support contract attached. Teams running ad verification, brand protection and social media automation at scale fit that profile.

If you're moving 5 to 50 GB a month and most of it is US or European residential traffic, the plan floor is doing more damage to your budget than any performance gap is worth. That's the point at which it's worth pricing an alternative rather than optimising within SOAX's tiers.

## The alternative worth pricing: pay-as-you-go at $1/GB

DataImpulse is the provider most often named in that comparison, and the contrast is structural rather than cosmetic. It sells residential traffic at a flat $1/GB on a pay-as-you-go basis, with no subscription and no monthly minimum, and the traffic you buy does not expire. Its pool is reported at 90M+ ethically sourced IPs across 195 countries, with HTTP(S) and SOCKS5 both supported and country targeting included at the base rate.

Since this is a review of SOAX rather than a comparison article, here's the honest part. The two vendors are not the same product.

**Where DataImpulse wins clearly:** entry cost and expiry rules. A $5 purchase gets you 5 GB of residential traffic. There's no $200 floor, so a 10 GB month costs $10 instead of $50 (Sandbox) or $200 (Builder). Unused traffic stays on your balance instead of expiring in 60 days, which matters a lot for spiky or experimental projects. Country targeting is free, and standard residential pricing doesn't shift by country tier the way SOAX's does — your per-GB math doesn't change because your targets moved from Germany to Vietnam.

**Where DataImpulse doesn't match SOAX:** there's no static ISP product (SOAX has a US-only ISP line), no managed scraping API — DataImpulse sells raw proxy access and expects you to handle rendering, retries and CAPTCHAs yourself — and independent reviewers note its pool is noticeably thinner than Bright Data or Oxylabs in Tier 3 geographies. ProxyLook's review also notes no SOC 2 or ISO 27001 certification, which can be a procurement blocker for enterprise buyers who need that paperwork.

One caveat to verify yourself: third-party write-ups disagree on whether advanced filters (state, city, ZIP, ASN) carry a surcharge on standard residential traffic. AIMultiple reports those filters billed at 2× the standard rate on residential and recommends confirming current billing treatment with support before you plan a budget around it, while other reviews describe city-level targeting as bundled. If your workload depends on city or ZIP precision, ask before you buy.

### The same workload, priced two ways (Tier 1 residential)

| Monthly volume | SOAX (published rates) | DataImpulse |
| --- | --- | --- |
| 10 GB | $50 on Sandbox ($5.00/GB); $200 minimum on any paid plan | $10 |
| 100 GB | $300 on Builder ($3.00/GB) | $100 |
| 500 GB | ~$1,100 on Team ($2.20/GB) | $500 |
| 1 TB | Lower rate, requires Scale or Enterprise commitment | $800 ($0.80/GB) |

Those SOAX figures use published per-GB rates and the plan floors above; your actual bill shifts with your country mix. That's the whole point — at DataImpulse the country mix doesn't move the residential price.

## Every DataImpulse plan, side by side

DataImpulse prices by traffic amount rather than by feature gate, so the table below reflects its published tiers across all four proxy types. Traffic never expires on any of them, there's no subscription, and the minimum entry purchase is $5.

| Proxy type | Plan | Traffic | Price | Effective rate | Billing | Purchase |
| --- | --- | --- | --- | --- | --- | --- |
| Residential | Intro | 5 GB | $5 | $1.00/GB | One-time, no expiry | [Start with 5 GB of residential traffic](https://bit.ly/dataimPulse) |
| Residential | Basic | 50 GB | $50 | $1.00/GB | One-time, no expiry | [Buy 50 GB residential](https://bit.ly/dataimPulse) |
| Residential | Advanced | 1 TB | $800 | $0.80/GB | One-time, no expiry | [Get the 1 TB residential tier](https://bit.ly/dataimPulse) |
| Residential | Custom+ | 5 TB+ | from $4,000 | Custom | Contact sales | [Request volume pricing](https://bit.ly/dataimPulse) |
| Mobile | Intro | 2.5 GB | $5 | $2.00/GB | One-time, no expiry | [Test mobile proxies from $5](https://bit.ly/dataimPulse) |
| Mobile | Basic | 25 GB | $50 | $2.00/GB | One-time, no expiry | [Buy 25 GB mobile traffic](https://bit.ly/dataimPulse) |
| Mobile | Advanced | 1 TB | $1,600 | $1.60/GB | One-time, no expiry | [Get 1 TB of mobile traffic](https://bit.ly/dataimPulse) |
| Mobile | Custom+ | 5 TB+ | from $8,000 | Custom | Contact sales | [Request mobile volume pricing](https://bit.ly/dataimPulse) |
| Datacenter | Intro | 10 GB | $5 | $0.50/GB | One-time, no expiry | [Start with 10 GB datacenter](https://bit.ly/dataimPulse) |
| Datacenter | Basic | 100 GB | $50 | $0.50/GB | One-time, no expiry | [Buy 100 GB datacenter traffic](https://bit.ly/dataimPulse) |
| Datacenter | Advanced | 1 TB | $450 | $0.45/GB | One-time, no expiry | [Get the 1 TB datacenter tier](https://bit.ly/dataimPulse) |
| Datacenter | Custom+ | 5 TB+ | from $2,250 | Custom | Contact sales | [Request datacenter volume pricing](https://bit.ly/dataimPulse) |
| Premium residential | Intro | 1 GB | $5 | $5.00/GB | One-time, no expiry | [Try premium residential from $5](https://bit.ly/dataimPulse) |
| Premium residential | Basic | 10 GB | $50 | $5.00/GB | One-time, no expiry | [Buy 10 GB premium residential](https://bit.ly/dataimPulse) |
| Premium residential | Custom+ | 5 TB+ | from $20,000 | Custom | Contact sales | [Request premium volume pricing](https://bit.ly/dataimPulse) |

A few notes on that table, because flat tables hide things. Mobile volume discounts don't kick in until the 1 TB tier, so mid-size mobile buyers pay $2/GB all the way up. Premium residential carries a dedicated account manager and includes city, state, ZIP and ASN targeting without surcharge, which is where its $5/GB starts to make sense. And DataImpulse lets you enter any GB quantity rather than forcing you into fixed buckets, so the tier names are really reference points for the rate you land on.

## What DataImpulse is not good at

Worth stating plainly, because a review that only lists advantages isn't a review.

- **No managed scraping service.** If you want someone else to handle browser rendering, retries and CAPTCHA solving, DataImpulse is the wrong layer of the stack. It sells IP access.
- **No static ISP proxies.** Persistent-identity workloads that need a fixed address belong on SOAX's ISP line or a dedicated ISP provider.
- **Thinner coverage in hard-to-source regions.** Independent reviews consistently place DataImpulse's Tier 3 depth behind Bright Data and Oxylabs. If your targets are concentrated in sub-Saharan Africa or Central Asia, sample it first.
- **Support is leaner than a named account manager.** DataImpulse advertises 24/7 human support on live chat and HostAdvice's test got a reply in about seven minutes, but enterprise escalations route differently than they do at a vendor charging $3,000 a month.
- **Not for regulated or gated targets.** DataImpulse's own documentation says it isn't the right fit for banking and government sites.

## How to decide without overthinking it

Run your own volume first, then match it.

- **Under 50 GB a month, mostly US or EU residential:** DataImpulse at $1/GB with non-expiring traffic. The SOAX plan floor is the deciding factor here, not performance.
- **50 to 500 GB a month on standard residential, mixed geographies:** DataImpulse again, unless you specifically need SOAX's ISP or mobile lines.
- **Heavy mobile-proxy workloads with US or India focus:** compare carefully. SOAX's mobile network and DataImpulse's $2/GB mobile tier are priced differently, and DataImpulse's mobile discounts only arrive at 1 TB.
- **Enterprise procurement, KYC paperwork, ISP proxies, support contracts:** SOAX or a comparable enterprise vendor. Paying $200 to $3,000 a month for infrastructure with compliance documentation behind it is a legitimate purchase.
- **You need managed scraping output rather than IPs:** neither. Look at a scraping API instead.

One last practical note for buyers doing the SOAX evaluation: ask about country tier before anything else. Get a list of the regions your traffic will route through and ask which tier each falls into. On SOAX that answer can move your effective cost per GB by up to 8×. On DataImpulse, standard residential stays at $1/GB with country targeting included — which is a simpler number to plan around, even if you end up choosing otherwise.
