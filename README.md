# Business Relevance Analyzer

An AI skill for **Claude** that turns any business source — news articles, competitor pages, strategy memos, call transcripts, partner emails — into a prioritized, actionable analysis for **your** business.

It's not a summarizer. It's a senior analyst that:

- tells you what's actually a signal vs. what's noise,
- ranks the findings by business relevance,
- maps them to the right functions (product, sales, ops, strategy, etc.),
- proposes concrete next steps,
- and is honest about what's weak evidence or doesn't transfer to your market.

Built for executives who want a **half-page, decision-ready** breakdown — not a wall of text.

---

## What it looks like in practice

**You:** *drop in a news article about a competitor raising a funding round*

**Claude:** produces a structured analysis — mode used, signal strength, top 3 insights (each with a score, one-line rationale, a concrete next step, and a caveat), an Act/Validate/Monitor/Ignore action list, and the main risks.

All of it grounded in **your business context** — not generic advice. If you run a real-estate lead-gen platform, the skill won't recommend you "explore B2B SaaS opportunities" because it knows that's not what you are.

---

## Who this is for

Business leaders, product/strategy leads, chiefs of staff, bizdev — anyone who regularly gets hit with documents, articles, and transcripts and has to figure out *"what does this mean for us, and what should we do?"*

The skill is pre-configured with a real-estate classifieds / lead-generation context (see `references/business-context.md`). **You'll want to edit that file to match your business** once installed — it's a single, plain-English markdown file; no coding required.

---

## Installation

You can use this skill with **Claude Code** (the terminal version of Claude) or with **Claude.ai** (the web version). Pick whichever you use.

### Option A — Claude Code (terminal)

1. **If you don't have Claude Code yet**, install it: [https://claude.com/claude-code](https://claude.com/claude-code)

2. **Clone or download this repo** somewhere on your computer:
   ```
   git clone https://github.com/YOUR_USERNAME/business-relevance-analyzer.git
   ```
   (Or click the green "Code" button on GitHub → "Download ZIP" and unzip it.)

3. **Put it where Claude Code looks for skills:**
   ```
   ~/.claude/skills/business-relevance-analyzer/
   ```
   So the full move is: take the `business-relevance-analyzer` folder you just cloned, and copy it into `~/.claude/skills/`. If the `skills` folder doesn't exist, create it.

4. **Edit the business context** to match your business. Open:
   ```
   ~/.claude/skills/business-relevance-analyzer/references/business-context.md
   ```
   Replace the real-estate context with a description of your business, priorities, and the functions you work across. This file is the single biggest driver of how relevant the analysis is — **don't skip it.**

5. **Start a new Claude Code session and try it.** Just paste in an article or a memo and ask something like *"Разбери это с точки зрения моего бизнеса"* or *"What matters in this for us, and what should I do?"* Claude will pick up the skill automatically.

### Option B — Claude.ai (web)

1. Go to [Claude.ai](https://claude.ai) and sign in.

2. Create a new **Project** (left sidebar → Projects → New project).

3. Upload the skill files to the project:
   - `SKILL.md`
   - Everything inside the `references/` folder (`business-context.md`, `modes.md`, `examples.md`)

4. In the project's **Custom instructions** field, paste this:
   > You have access to a skill called Business Relevance Analyzer. Whenever I share a document, article, transcript, memo, or any other source and ask you to analyze it, follow the instructions in SKILL.md. Always load references/business-context.md first.

5. **Edit `business-context.md`** (in the project files) to match your business — same as step 4 of the Claude Code instructions above.

6. Done. Upload or paste sources into the chat and ask for an analysis.

---

## How to use it

Once installed, just send Claude a source and ask what it means. A few examples:

- *"Проанализируй эту статью про конкурента."*
- *"Review this internal memo — I'm taking it to leadership next week, tell me where it's weak."*
- *"Вот транскрипт звонка с клиентом, вытащи сигналы для продукта и операций."*
- *"Can we actually apply this in our business, or is this US-only? Stress-test it."*

The skill supports a few **modes** — it picks one automatically based on what you gave it. You can also steer it explicitly:

- **Competitive / Market Signal** — for news, competitor pages, industry moves
- **Internal Memo Review** — for reviewing your own or colleagues' strategy docs
- **Customer Insight** — for call transcripts, customer interviews
- **Applicability Stress Test** — for pressure-testing whether an idea transfers to your business

Default output is **compact** (~half a page). If you want the full treatment — function-by-function implications, hypotheses to validate, transferability analysis — ask for "**deep**" analysis or "**полный разбор**".

---

## What's in this repo

- `SKILL.md` — the core skill file (what Claude reads to know how to behave)
- `references/business-context.md` — the business context (edit this!)
- `references/modes.md` — detailed per-mode guidance
- `references/examples.md` — good/bad output examples
- `evals/` — test cases and synthesized source materials used during development (optional, for reference)

---

## FAQ

**I'm not technical. Do I need to write code?** No. You edit one plain-English markdown file (`business-context.md`) and the skill does the rest.

**Will it work in English / Russian / other languages?** Yes. The skill responds in whatever language you write in. It's been tested in Russian and English.

**Is my data sent anywhere?** The skill itself is just a set of markdown instructions. Whatever Claude normally does with your data (per Anthropic's terms) is what happens here too.

**Can I fork it and adapt it for my team?** Yes — that's the intended use. Fork, edit `business-context.md` for your company, and share with your team.

---

## License

MIT. Use it, fork it, share it.
