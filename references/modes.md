# Analysis Modes

This file expands each analysis mode. Read the section for the mode you're using.

## Universal Business Analysis

The default fallback when nothing fits cleanly. Treat it as "generic but with the business lens applied."

Focus:
- What in this source would change a decision for this business?
- Signal or noise?
- If signal — what kind (market, customer, product, operational, strategic)?
- Function mapping and action classification.

Emphasis: balanced. Don't let the source dictate the structure; let the business context dictate what to surface.

---

## Competitive / Market Signal Mode

Use for: external articles, news, competitor product pages, competitor releases, industry reports, foreign market cases.

Focus:
- **Signal strength** — is this a real move or marketing gloss? Is there operational substance behind it?
- **Threat / opportunity / noise classification** — be explicit
- **Strategic positioning** — how does this change the user's competitive posture?
- **Transferability** — foreign cases especially need skeptical transfer analysis
- **Response options** — if it's a threat, what are the plausible responses and what do they cost?

Hype check is mandatory here. If the source is a press release or a partner-sponsored article, assume substance is below the surface and say so unless you find evidence otherwise.

Don't over-index on novelty. "Nobody is doing this" can mean "there's a reason nobody is doing this."

---

## Internal Memo Review Mode

Use for: the user's or colleagues' internal writing — strategy memos, six-pagers, one-pagers, MBR text, product cases, org notes.

Focus:
- **Strongest ideas** — what's actually good, sharp, novel, decision-grade
- **Argument quality** — where does the logic hold, where does it leak?
- **Missing pieces** — evidence that should be there but isn't; stakeholders / constraints not considered
- **Contradictions** — internal inconsistencies, tensions with strategy, hidden trade-offs
- **Execution risk** — where the plan looks like it will break in practice
- **Decision readiness** — if a reader has to make a call on this, can they? What's still missing?

Tone shift: the user is often the author or colleague. Be direct and critical, not cushioning — but not brutal. Aim for "best reviewer you've worked with" — specific, constructive, high-signal.

The output is less about function-mapping and more about **what the author should strengthen, drop, or reconsider before this is decision-grade.**

---

## Customer Insight Mode

Use for: transcripts of customer-facing conversations — buyer calls, customer interviews, call-center recordings, partner calls, negotiations with developers.

Focus:
- **Repeated pains** — things said multiple times or across speakers
- **Objections** — especially during money/commitment moments
- **Unmet needs** — jobs that customers are trying to do that the current product or process doesn't support
- **Demand patterns** — where buyers/developers show intent, where they drop out
- **Trust and decision barriers** — what makes them hesitate, what they want to verify
- **Hidden product opportunities** — things the customer didn't ask for but clearly would use
- **JTBD framing** — what job was the customer hiring the interaction to do?

Output emphasis:
- Cite specific evidence (short quotes or paraphrases tied to speakers) — this is what makes insights from transcripts credible
- Rank findings by relevance to product, sales, marketing, and operations (including call-center process)
- Distinguish what one customer said vs. what looks like a pattern

---

## Applicability Stress Test Mode

Use for: when the user has an idea (theirs, from a source, or floating around) and wants to pressure-test whether it transfers to the business. Often triggered by phrases like "can we do this", "is this applicable", "would this work for us".

Focus:
- **What would need to be true** for this to work in this business?
- **Dependencies** — what prerequisites exist (capability, tech, data, process, org)?
- **Blockers** — constraints that could kill or limit the idea (regulation, unit economics, buyer behavior, seller dynamics)
- **Honest translation** — what's the version of this idea that would actually work here, even if diminished?
- **Minimum viable test** — if the user wanted to validate cheaply, what's the smallest experiment?

Bias toward "here's where it breaks" over "here's how it could work". That's the value of the mode. If everything looks great, you probably missed something.

Output shape:
- Summary verdict: transferable / partially transferable / not transferable / only under conditions X, Y, Z
- List of required conditions
- List of blockers, with severity
- Minimum test design
- What similar bets in this business have taught us (if user has mentioned any)

---

## Depth configuration

Across all modes:

- **Default (compact)** — TL;DR + 3 tight insight cards + actions + risks. ~400–600 words. This is what the user wants by default; do not pad. See the compact template in SKILL.md.
- **Deep** — full insight cards (5–7), cross-functional implications, transferability analysis, contradiction checks, hypotheses to validate. Trigger on explicit user request or when reviewing a high-stakes memo going to leadership.

The old "standard" middle tier is gone on purpose. Either tight or deep — no middle sprawl.

## Horizon configuration

If the user specifies or it's clear from context:

- **Immediate** — quick wins, fast experiments, decisions in 1–4 weeks. Favor Applicability, Feasibility, Speed to value.
- **Quarterly** — roadmap / GTM / operational improvements. Balanced weighting.
- **Strategic** — structural trends, capability gaps, long-term moves. Favor Strategic relevance and Defensibility.

If the user doesn't specify, infer from the source: news articles are often Immediate-or-Quarterly; strategy memos are Quarterly-or-Strategic; customer transcripts are Immediate-or-Quarterly.
