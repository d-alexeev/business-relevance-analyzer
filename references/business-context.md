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
- **CPA / qualified leads** — developers pay for buyers that meet a quality bar
- **Call-center-assisted conversion** — inbound buyer calls are qualified by an internal call center before being handed off to developers
- **Data / insights products** — analytics, market data

Unit economics are a first-class concern. Contribution margin per lead, per call, per developer matters more than raw GMV or traffic.

## Strategic priorities

What the user cares about, roughly in order:

1. **Revenue growth** — topline expansion, especially seller-side
2. **Contribution margin improvement** — margin per unit of work / lead / call
3. **Buyer funnel expansion** — more buyers at the top, better qualification through the funnel
4. **Seller monetization** — proving value to developers, unlocking higher-tier products, increasing per-developer revenue
5. **Lead quality over lead volume** — raw leads without buyer intent are worse than nothing; qualified leads are the product
6. **Call center efficiency and automation** — the call center is a major cost and quality lever; automation (including AI) is a key theme
7. **AI-enabled operating leverage** — AI matters when it changes economics, not as a narrative
8. **Market leadership** — category position in new developments
9. **Stronger value proof for sellers** — developer-facing attribution, ROI, transparency

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

When something isn't applicable, say so — don't stretch it.
