# Examples: good vs. bad output

Read this when uncertain about the right level of specificity, or when tempted to write generic-sounding analysis.

## Example 1 — insight cards

### ❌ Bad

> **Insight:** AI is becoming important in real estate.
> **Why it matters:** Competitors are using it, so we should consider it.
> **Score:** 7/10
> **Impacted functions:** Product, Operations, Strategy
> **Suggested application:** Explore AI opportunities in our funnel.
> **Recommended next step:** Form a working group to discuss AI strategy.

Why this is bad:
- The "insight" is a truism, not a signal.
- "Why it matters" is circular ("because competitors are doing it").
- Score has no basis.
- Functions are dumped in without differentiating.
- Next step is a meeting, not a move.

### ✅ Good

> **Insight:** The competitor is using a voice-AI agent for first-line lead qualification, reporting 40% reduction in human-agent handle time without measurable drop in developer-facing lead quality (per their product blog — self-reported, single cohort).
> **Why it matters for our business:** Our call center is a P&L lever: first-line qualification costs about [X] per call and currently takes [Y] minutes. If a voice agent can halve handle time on ~50% of calls that are pure info-gathering, contribution margin per lead improves materially. This is also an asymmetric move — if they reach scale first, our cost base becomes harder to defend to sellers.
> **Business relevance score:** 8.4 / 10
> **Confidence:** Medium — one source, self-reported, no independent validation.
> **Signal type:** Competitive threat + monetization opportunity
> **Impacted functions:** Operations, Product, Revenue Ops
> **Suggested application:** (1) Scope a 4-week pilot on inbound calls tagged as "info-seeking" by current routing rules. (2) Build an internal cost model to size the margin impact before committing engineering.
> **Recommended next step:** Pull last quarter's call tags + AHT by category from RevOps, size the addressable cost pool, and assign an Ops + Product owner pair for a 2-week discovery sprint.
> **Caveat:** Buyer expectations around developer interactions differ from US patterns — Russian buyers show lower tolerance for non-human first contact in our past surveys. A pilot must measure qualified-lead conversion, not just AHT.

Why this is good:
- Concrete (numbers, cohort, tagging logic).
- "Why it matters" is tied to specific P&L mechanics of this business.
- Score earns its weight — one source, self-reported → Medium confidence.
- Functions selected because they each have a real role.
- Next step is a specific, ownable move.
- Caveat names the transferability risk without hand-waving.

---

## Example 2 — executive summary

### ❌ Bad

> The article discusses several trends in proptech including AI, personalization, and data-driven marketing. These are all relevant to our business. We should consider which ones to pursue.

Why this is bad: zero prioritization, no business framing, no decision. It's a restatement of the article's table of contents.

### ✅ Good

> **Mode:** Competitive / Market Signal. **Source strength:** Moderate — one opinion piece by a VC, no primary data.
>
> Two of the three trends the author flags have real relevance for us, one doesn't:
>
> 1. **AI-first lead qualification** is the headline signal — it intersects directly with our call-center economics. Worth a pilot.
> 2. **Transparent developer ratings** maps to our "proof of value for sellers" priority. Worth validating on a cohort.
> 3. **VR walkthroughs** is hype-adjacent for our market — high cost, weak evidence of conversion lift, and Russian buyer behavior doesn't match the US cases cited. Ignore for now.

Why this is good: names the mode and source strength up front, takes a position on each item, dismisses one with a reason.

---

## Example 3 — handling weak sources

### ❌ Bad (manufacturing insights from a weak source)

> The press release announces a partnership between X and Y. Key implications:
> 1. Partnerships are becoming important in proptech.
> 2. Integration is a trend.
> 3. We should consider similar partnerships.

### ✅ Good

> This is a promotional partnership announcement with no operational detail. The only potentially interesting observation is that X has chosen to integrate with Y rather than build in-house capability — which is a weak signal that they see the build cost as high or the time-to-market pressure as real. But that's one data point from a self-interested source. Confidence: Low. Not actionable. **Monitor** the pair for future indicators of actual traction (usage numbers, repeat announcements, category expansion).

Why this is good: refuses to manufacture. States what's weak. Gives one honest observation and flags it as Low confidence. Chooses the right bucket (Monitor, not Act).

---

## Example 4 — function mapping discipline

Source: a customer interview transcript where the buyer complained about unclear apartment pricing on developer websites and about being passed between multiple call-center agents.

### ❌ Bad function mapping

> **Impacted functions:** Product, Marketing, Sales, BizDev, Operations, Strategy, Analytics

(Lists all functions because the template has them.)

### ✅ Good

> **Impacted functions:** Product, Operations.
>
> - **Product** — the pricing transparency gap on listing cards is a feature opportunity; we already capture the data, we're just not surfacing it.
> - **Operations** — call-center handoff quality issue (buyer was transferred 3 times). Worth pulling the call log to see if this is systemic in the developer-specific queues.

Marketing, Sales, BizDev, Strategy, Analytics are omitted because the transcript doesn't meaningfully implicate them.
