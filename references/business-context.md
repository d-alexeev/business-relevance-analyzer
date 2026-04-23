# Business Context

This file describes the user's business. The Business Relevance Analyzer grounds every judgment of relevance, applicability, and action in this context. Edit this file as the business evolves — do not edit the skill logic.

## Business model

The user leads a business unit in **real estate, focused on new developments (новостройки)**. The operating model is close to a **marketplace / classifieds / lead generation platform**:

- Two-sided: buyers (end consumers looking for apartments) and sellers (property developers / застройщики)
- Revenue is earned by connecting buyers to sellers and proving value to sellers
- The business operates in a matrix organization with shared resources across business units

## Monetization

Revenue streams include (and lean on in roughly this order):

- **Media products** — paid placements, promotion, visibility to buyers
- **CPA / qualified leads** — developers pay for buyers that meet a quality bar; this is the priority growth vector
- **Call-center-assisted conversion** — inbound buyer calls are qualified by an internal call center before being handed off to developers
- **Data / insights products** — analytics, market data

Unit economics are a first-class concern. Contribution margin per lead, per call, per developer matters more than raw GMV or traffic.

**CPA model detail:** A "qualified lead" is a buyer who has passed through the call center and confirmed real interest and budget. Potential expansion of the model: differentiated CPA tiers ("hot" — ready for a meeting now vs. "warm" — real buyer with a 1–3 month horizon) and premium CPA events (e.g., online booking).

## Market conditions (~2026)

- **Buyer's market:** buyers expect discounts, personalized terms, flexible payment options
- **Deal cycle has elongated significantly:** 60+ days on average (was 23–26 days in H1 2024); sales managers average 12 touchpoints to close a deal
- **Mortgage dominates:** 70–75% of deals go through mortgage programs; installment (рассрочка) remains relevant for a segment of buyers
- **Льготная ипотека** has been significantly restricted; key rate (ключевая ставка) is high with expected gradual decrease
- **Market volume is declining** — developers are under pressure; every lead matters more than before
- **~70% of buyers** begin their search on classifieds, then move to the developer's site

## Strategic priorities

What the user cares about, roughly in order:

1. **Revenue growth** — topline expansion, especially seller-side
2. **Contribution margin improvement** — margin per unit of work / lead / call
3. **Buyer funnel expansion** — more buyers at the top, better qualification through the funnel
4. **Seller monetization** — proving value to developers, unlocking higher-tier products, increasing per-developer revenue
5. **Lead quality over lead volume** — raw leads without buyer intent are worse than nothing; qualified leads are the product
6. **Call center efficiency and automation** — the call center works on an inbound model: buyer leaves a request on the platform → call center calls back, qualifies, hands off to developer. Speed of first response is critical (conversion loss is significant with delays >5 min for hot leads). Qualification criteria: real budget + purchase horizon + interest in a specific development. Current gap: leads with a 60+ day horizon are often discarded as "non-target," even though the market closes such deals routinely.
7. **AI-enabled operating leverage** — AI matters when it changes economics, not as a narrative
8. **Market leadership** — category position in new developments
9. **Stronger value proof for sellers** — developer-facing attribution, ROI, transparency

## Buyer profile

- Russian-speaking audience, primary age range 28–50
- Conservative decision-making: high key rate → long consideration cycle
- 70% start their search on classifieds, then explore the developer's site
- Primary purchase mechanism: mortgage (70–75%); installment is an alternative for some
- Low tolerance for automated messaging interactions (especially 35+): AI-first contact is perceived worse than in APAC cases
- Requires pricing transparency: discounts and payment terms should be visible before the first call

## Ecosystem map

Key players to know when analyzing any external source:

**Competitors (classifieds / lead gen):**
- Яндекс.Недвижимость — major competitor, classifieds + lead gen
- Домклик (Sberbank) — classifieds + mortgage ecosystem
- ЦИАН — classifieds, stronger in secondary market

**Technology partners / developer ecosystem:**
- **Profitbase** — dominant CRM for new-development sales teams (650+ developer clients in Russia); mediates developer presence on classifieds via API/data export; key integration partner and potential strategic intermediary
- **Сделка.РФ** — mortgage aggregator (30+ banks, real-time rate updates)
- **Trendagent, CMKet** — agent channel aggregators (growing channel)

**Structural threats:**
- Self-qualification tools for developers (AI agents like Gene AI) — reduce developer dependency on our lead gen
- Growth of the agent channel — agent-mediated deals partially bypass our classifieds

## Functional structure

The user works across these functions and expects insights to be mapped to them correctly:

- **Product** — features, UX, funnel mechanics, data capture, intent signaling, trust/transparency tools, lead qualification aids, content tools
- **Marketing** — messaging, segmentation, campaigns, pre-demand education, content formats, acquisition narrative
- **Sales** — seller-facing (developer sales), value story, packaging, objections handling, ICP differentiation, enablement, offer design
- **BizDev** — partnerships, ecosystem plays, route-to-market, new business models, integrations, strategic channel moves
- **Revenue Ops** — unit economics, routing logic, qualification rules, margin impact, prioritization by economics, operational measurement
- **Operations** — call center scripts, QA, process efficiency, handoff quality, staffing, AI automation candidates
- **Strategy** — category bets, investment cases, market posture, capability gaps, strategic risks
- **Analytics** — measurement frameworks, attribution, data products, insight generation

Common confusions to avoid:
- **Sales** here means developer-facing revenue motion, not consumer-facing. Don't conflate with Marketing.
- **BizDev** is for partnership and new-channel moves, not tactical sales enablement.
- **Revenue Ops** owns unit economics and routing; **Operations** owns call-center execution. They're adjacent but distinct.

## Organizational reality

- Matrix environment — decisions live at the intersection of business, product, and shared functions
- Headcount and ROI constraints are real; "hire a team to do this" is rarely a cheap recommendation
- Cross-functional execution is the default, which means dependency burden is always a non-trivial cost
- The user often works on memos, six-pagers, MBR content, and needs output that's close to decision-grade

## What "applicable" means here

An idea is applicable if:
- It fits the marketplace / lead-gen / two-sided logic (not pure e-commerce, not pure SaaS)
- It respects the call-center-in-the-loop reality
- It plays with unit economics that depend on lead quality, not just volume
- It can work in a matrix org without requiring a brand-new team
- It lands in one of the functions above, clearly

An idea is **not directly applicable** if:
- It assumes direct-to-consumer transactions (the buyer doesn't buy an apartment from the platform)
- It assumes a subscription SaaS motion
- It requires capabilities the business doesn't have and can't easily build
- It's a US or foreign case with very different buyer behavior, financing, or regulation
- It assumes "qualified" means "ready to buy this week" — our market's normal horizon is 60+ days and 12 touchpoints
- It assumes high buyer tolerance for AI/bot interactions in financial decisions (Russian audience 35+ is significantly more skeptical than APAC cases)
- It relies on an agent commission structure of 5%+ (our market is structured differently)
- It is premised on a growing market — our market is contracting; only conversion-improvement solutions are relevant, not demand-capture plays

When something isn't applicable, say so — don't stretch it.
