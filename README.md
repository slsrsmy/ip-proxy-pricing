# buy ip proxy: what a gigabyte really costs, how to test a pool for $5, and which plan fits your job

Nobody ships you a proxy in a box. When you buy IP proxies you are buying metered access to addresses that belong to someone else's hardware, and almost every pricing argument in this market comes down to three questions: what kind of IP is it, how much traffic do you push through it, and how precisely do you want to point it at a specific place.

Get those three straight and the shopping part takes ten minutes. Skip them and you end up paying $7 per GB for a job that a $0.50 datacenter IP would have handled, or buying a monthly plan that resets before you've used half the quota.

## The type of IP sets the floor price

Proxies are sold in four flavours, and the supply of each one explains the price gap better than any feature list.

| Type | Where the IP comes from | What it is good at | Typical market rate |
| --- | --- | --- | --- |
| Datacenter | Servers in commercial data centers | Cheap, fast, high-volume work on sites that don't scrutinise IP reputation | $0.50–$3/GB or a few dollars per IP per month |
| Residential | Real home broadband connections | Protected targets: e-commerce, SERPs, social platforms | $1–$8/GB |
| Mobile (4G/5G) | Cellular devices on carrier networks | The hardest targets, app and mobile-web data | $2–$15/GB |
| ISP / static residential | Datacenter-hosted IPs registered to an ISP | Long sessions where the same address must stay stable | ~$1.50–$5 per IP per month |

The logic behind the ladder is scarcity. Datacenter IPs are abundant, so they're cheap and easy to detect. Residential IPs have to be sourced from real people who consent and get paid, which costs money. Mobile IPs sit behind carrier-grade NAT, where thousands of subscribers share one address, so blocking them breaks legitimate users too. That resistance is why they cost five to ten times a datacenter IP.

DataImpulse, the provider used as the worked example below, prices at the bottom of each band: $1/GB residential, $0.50/GB datacenter, $2/GB mobile, and $5/GB for a premium residential pool. You can [👉 check the current per-GB rates and top-up tiers here](https://bit.ly/dataimPulse) before reading further, though it's worth understanding what those numbers do and don't include first.

## The four factors that actually decide your bill

Bandwidth and pool quality come first. Traffic is usually billed per gigabyte, and the cleanliness of the pool matters more than the sticker price. A $1 pool with a 55% success rate can end up costing more per usable result than a $2 pool at 90%, because every failed request still burns traffic and forces you to send more requests to hit the same target. That arithmetic is worth running on your own target before you scale anything.

IP type is second, and it's the one most buyers get wrong in the expensive direction. If a job runs fine on datacenter IPs, moving it to mobile isn't an upgrade; it's simply a bigger invoice.

Targeting granularity is third. Country-level targeting is almost always included. City, state, ZIP, and ASN filters are usually a paid add-on, and that surcharge can quietly double your effective cost per GB. DataImpulse's own FAQ says country targeting is free while city, state, ASN, and ZIP carry "a small extra fee"; a third-party teardown reports the advanced filters billed at twice the standard per-GB rate on residential plans. Its datacenter product page lists state, city, ZIP, and ASN as included, which is a different treatment for the same filters. If precise geo-targeting is central to your project rather than a nice-to-have, price the whole job with the surcharge applied, not just the headline rate.

Commitment is the fourth. Bigger monthly commitments and higher concurrency limits lower the unit price and raise the amount you pay whether you use it or not.

Most of the confusion in this market comes from comparing those four factors across providers that quote them differently. Pick the two that matter for your workload and compare on those.

## The part that costs you nothing on paper and a lot in practice

Expiring traffic is the quietest line item in proxy pricing. Plenty of plans zero out unused gigabytes at the end of each billing cycle, which means the month your scraping job slips, you've paid for bandwidth you'll never send. If your usage is irregular, a cheap per-GB rate on a subscription is a worse deal than a slightly higher per-GB rate on a pay-as-you-go balance.

DataImpulse built its pitch around that gap. Traffic is bought as balance, the balance doesn't expire, there's no subscription, and the minimum top-up is $5. Somebody testing whether residential proxies fix their problem at all can find out for the price of a lunch rather than committing to a monthly plan. The trade-off is the unit rate: you don't get the volume discounts a monthly commitment unlocks, and you pay $1/GB until 1 TB, where it drops to $0.80.

Three listings of what the plans include, in plain terms:

- Residential proxes: 90M+ IPs across 195 countries, rotating and sticky sessions, HTTP(S) and SOCKS5, free country targeting, and a published 99.51% success rate.
- Mobile proxies: real 4G/5G/LTE carrier IPs on the same pay-as-you-go model, at $2/GB.
- Datacenter proxies: randomized datacenter subnets with 99.9% uptime advertised, at $0.50/GB.

Support is 24/7 and human, via chat or email, and the company publishes a 4.8/5 G2 rating on its own site. Third-party listings also describe a 7-day refund window for first purchases, but that's a term to read on the checkout page rather than take from a review, since refunds are exactly where policies differ from how they're described.

## Every plan DataImpulse publishes

The four product lines, with each publicly listed tier. Rates are per the provider's own published pricing.

| Product | Tier | Price | Effective rate | Buy link |
| --- | --- | --- | --- | --- |
| Residential | Starter top-up | $5 for 5 GB | $1.00/GB | [ Take the $5 / 5 GB residential top-up](https://dataimpulse.com/residential-proxies/?aff=86938) |
| Residential | Standard | Any volume below 1 TB | $1.00/GB | [ Add residential balance in the dashboard](https://dataimpulse.com/residential-proxies/?aff=86938) |
| Residential | Advanced (volume) | 1 TB | $800 | $0.80/GB — [ See the residential volume tier](https://dataimpulse.com/residential-proxies/?aff=86938) |
| Datacenter | Starter | $5 for 10 GB | $0.50/GB | [ Start the datacenter pool at $0.50/GB](https://dataimpulse.com/datacenter-proxies/?aff=86938) |
| Datacenter | Mid | 100 GB | $50 | $0.50/GB — [ Top up 100 GB of datacenter traffic](https://dataimpulse.com/datacenter-proxies/?aff=86938) |
| Datacenter | Volume | 1 TB | $450 | $0.45/GB — [ Check the 1 TB datacenter tier](https://dataimpulse.com/datacenter-proxies/?aff=86938) |
| Datacenter | Custom | 5 TB+ | from $2,250 | Custom — [ Request a custom datacenter plan](https://dataimpulse.com/datacenter-proxies/?aff=86938) |
| Mobile | Starter | $5 for 2.5 GB | $2.00/GB | [ Try mobile IPs for $2/GB](https://dataimpulse.com/mobile-proxies/?aff=86938) |
| Mobile | Mid | 25 GB | $50 | $2.00/GB — [ Buy 25 GB of mobile traffic](https://dataimpulse.com/mobile-proxies/?aff=86938) |
| Mobile | Volume | 1 TB | $1,600 | $1.60/GB — [ See mobile volume pricing](https://dataimpulse.com/mobile-proxies/?aff=86938) |
| Mobile | Custom | 5 TB+ | from $8,000 | Custom — [ Ask about custom mobile volume](https://dataimpulse.com/mobile-proxies/?aff=86938) |
| Premium residential | Starter | $5 for 1 GB | $5.00/GB | [ Test the premium residential pool](https://dataimpulse.com/premium-residential-proxies/?aff=86938) |
| Premium residential | Mid | 10 GB | $50 | $5.00/GB — [ Buy 10 GB of premium residential traffic](https://dataimpulse.com/premium-residential-proxies/?aff=86938) |
| Premium residential | Custom | 5 TB+ | from $20,000 | Custom — [ Talk to support about premium volume](https://dataimpulse.com/premium-residential-proxies/?aff=86938) |

Two things stand out from that table. The first is the datacenter ladder, where the gap between $0.50 and $0.45 per GB is small enough that committing to 1 TB mainly makes sense if you're certain you'll burn it. The second is that volume discounts on mobile and premium residential only start at the 1 TB tier, so smaller buyers stay at the list rate.

## What you can't buy here

DataImpulse is a rotating network, and that shapes what it's the wrong tool for.

There are no static ISP proxies, so if your job needs the same address to persist for weeks — account management being the obvious case — this isn't the product. There's no managed scraping or SERP API either; you get proxies and documentation, and the parsing is yours. DataImpulse's own materials make the same point: it's for collecting public data and reaching content, not for static endpoints or fully managed extraction.

There's also a gating layer that surprises people. Bank and payment sites are restricted, and .gov domains require identity verification. All .gov websites open at once once you've verified your identity and spent over $100; banking and payment sites are considered after verification plus $1,000 in spend, and only for business use cases. Individual .gov domains can be requested earlier, also with KYC completed. If your project depends on those targets, factor the verification step and the spend threshold into your timeline, because no amount of topping up skips it.

## How to test a pool without gambling $200

Testing is cheaper and more decisive than reading reviews, including reviews that compare providers where the reviewer is a competing network. Concretely:

1. Create an account and top up the minimum. On this provider that's $5, which buys 5 GB of residential traffic that won't expire while you decide.
2. Build the endpoint in the dashboard. Rotating connections run on port 823 for HTTP/HTTPS and 824 for SOCKS5; sticky sessions live in the 10000–20000 range, where an IP stays fixed for one to 120 minutes, defaulting to 30 if you don't specify an interval. Authentication is username/password or an IP whitelist.
3. Point it at the target you actually care about, not a homepage. Run maybe a few thousand requests with your real concurrency and headers, then count successes rather than bytes.
4. Calculate cost per successful request. That figure, not the per-GB rate, is what your budget will feel, and it's the only comparison that survives contact with a defended website.

For a reference point from outside the vendor: a proxy network that tests rivals published measurements showing DataImpulse returning 172,893 live IPs across five countries, with median response times between 430 and 501 ms, and a pool depth around 60% of the deepest network it measured. That review carries a disclosed commercial interest — the publisher sells a competing network — which makes the numbers worth knowing and the framing worth discounting. The direction of the finding is the honest summary: fast responses, mid-sized pool, likely fine for steady work on ordinary targets, and more likely to show address repetition under heavy defensive loads.

## Sessions, concurrency, and the boring integration bits

Rotating and sticky sessions both exist, and the choice is driven by your target, not by preference. Rotating suits crawling, where you want a fresh IP per request and no request pattern to cluster on a single address. Sticky helps when a site behaves better with short-term continuity, like a multi-step form or a login flow.

DataImpulse supports up to 2,000 simultaneous connection threads, scalable on request, which is the number that matters once your throughput stops being limited by the network. Protocols are HTTP(S) and SOCKS5, integrations are documented for Python, Selenium, Playwright, Puppeteer and Scrapy, and there are guides for the usual anti-detect browsers. Nothing here is exotic, and the documentation is public if you want to sanity-check the setup before paying.

## A short buying checklist

Before you enter card details anywhere in this market, five questions are worth answering:

- What's the minimum top-up, and does unused traffic expire? A cheap rate with a $50 minimum and monthly resets is an expensive way to test an idea.
- Are the targeting filters you need included or surcharged? City and ASN filters commonly double the per-GB rate on residential plans.
- How are failures billed? They almost always are. Success rate, not list price, decides your real cost.
- Is there a refund window, and what conditions attach to it?
- Which targets are gated behind identity verification or refused outright?

Answer those and the remaining decision is mostly about matching the plan to the job.

## Which plan fits which job

For a first purchase, the 5 GB residential top-up at $5 is the sensible default. It's enough traffic to run real requests against your own targets, it covers country-level targeting, and it never expires, so there's no clock racing you. Residential IPs are the ones that get past IP-reputation checks on e-commerce, search, and social platforms, which is where most buyers of IP proxies actually lose requests.

Datacenter is the right answer when your targets don't inspect IP type and you care about throughput per dollar. At $0.50/GB with 99.9% uptime advertised, it's four times cheaper than mobile and twice as cheap as residential, and $5 buys 10 GB instead of 5.

Mobile is for the specific case where datacenter and residential both fail and you need carrier IPs — mobile-first platforms, app-level data, and sites that treat non-cellular traffic as suspicious. Paying $2/GB for a job that works at $1/GB is a waste; paying $1/GB for a job that only mobile IPs will complete is a waste with extra retries attached.

Premium residential sits between residential and mobile in positioning, at $5/GB, with a dedicated account manager and every targeting option without surcharge. It only makes financial sense on targets where standard residential traffic is getting blocked, and then only if the extra success rate outweighs the five-times price difference. Run the numbers on the standard pool first.

## Quick answers

**Is a per-gigabyte plan cheaper than a monthly subscription?** Only sometimes. A large monthly commitment usually has a lower unit rate, but if you use half of it, the effective cost per usable gigabyte can be worse than pay-as-you-go. The regularity of your workload decides this, not the sticker price.

**Can you buy a single static IP here?** No. The network is rotating, with sticky sessions capped at two hours. Static ISP proxies are a different product from a different kind of vendor.

**What does a $5 test actually get you?** Five gigabytes of residential traffic, or 10 GB of datacenter, or 2.5 GB of mobile. Enough for a few thousand real requests on your own targets, which is more useful than any benchmark you can read.

**Why is mobile ten times the price of datacenter?** Carrier-grade NAT means many subscribers share one address, so websites can't block mobile IPs aggressively without breaking real users. Scarce supply, high resistance, high price.

The short version: decide what kind of IP your target actually requires, keep the entry purchase small enough that testing is cheap, and ignore every advertised per-GB rate until you've measured cost per successful request on your own workload. Start with the smallest tier that answers that question — [👉 the $5 residential top-up is the cleanest way to get an answer](https://bit.ly/dataimPulse).
