# automation — AI Issues Radar

_Last updated: 2026-03-18_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 1 | 🔴 Critical | Zapier pricing rage — what started at $10/month has ballooned to $750+/month for basic automations; mass migration underway | Zapier | Ongoing |
| 2 | 🔴 Critical | "$40K/year Zapier lesson" — viral Reddit post documents company that burned $40K/yr on simple automations, now migrating entire stack | Zapier | Active (March 2026) |
| 3 | 🟠 Major | "Zapier Tax" — per-task pricing model penalises growth, destroying SaaS margins as automation volume scales | Zapier | Ongoing |
| 4 | 🟠 Major | AI agent workflow steps are Zapier's most expensive per-task items — AI-powered automations cost 5–10x more than traditional steps | Zapier / Make | Active |
| 5 | 🟠 Major | Make (formerly Integromat) — steep learning curve and performance slowdowns with heavy data volumes | Make | Ongoing |
| 6 | 🟡 Notable | n8n self-hosted maintenance burden; requires engineering resources most target users don't have | n8n | Ongoing |

---

## Details

### 🔴 Zapier Pricing Explosion — $10/month → $750+/month

**What happened:** A October 2025 Reddit post — "TIRED OF ZAPIER" — encapsulated a community boiling point. Long-time Zapier users report their costs have exploded from an accessible entry price to **over $750/month for basic automations** that haven't fundamentally changed. The root cause is Zapier's **per-task pricing model**: every step in every Zap counts as a billable task. As businesses grow and automate more, costs compound rapidly.

**The March 2026 Reddit verdict** (r/automation "Honest Review: Which automation tool is actually worth it in 2026?"):
- **Zapier**: "Still the easiest for simple API-to-API stuff. But the cost per task is insane once you scale."
- **The brutal summary**: "Zapier and Make are the most successful scams in SaaS history. They charge you per 'task' for literally moving data between two APIs — something that costs fractions of a cent in compute."

**Scale of impact:** This is not a niche complaint. Zapier is one of the most widely-used business automation tools globally. The pricing structure actively penalises successful users — the more you automate (and presumably the more value you get), the more you pay.

**The "Zapier Tax" concept** (from r/SaaS, March 2026): By 2026, the term "zapier tax" has entered the SaaS vocabulary. It describes the phenomenon where a growing company's automation costs balloon faster than their revenue, because Zapier's per-task model means you are "literally being penalized for your own growth."

**Community migration:** Users are moving to n8n (self-hosted, no per-task fees) and Make as alternatives, despite both having significant drawbacks (see below).

**Source:** Reddit r/automation, Reddit r/zapier, Reddit r/SaaS — October 2025–March 2026

---

### 🟠 Make (Integromat) — Learning Curve and Slow Performance

**What happened:** Make is the most-recommended Zapier alternative for users who need visual workflow control. However, it has consistent complaints:
- **Steep learning curve** — the visual interface is powerful but non-obvious; new users frequently get stuck
- **Performance slowdowns with heavy data** — workflows processing large volumes of data run slowly
- **Hidden costs** — like Zapier, costs escalate with volume (though generally more slowly)

**Community reaction:** Make is frequently described as "better than Zapier but still frustrating." It captures users fleeing Zapier's pricing but doesn't satisfy users who want simple, fast, cheap automation.

**Source:** Reddit r/automation, Reddit r/SaaS — 2026

---

### 🟡 n8n — Self-Hosted Maintenance Burden

**What happened:** n8n (open-source, self-hosted workflow automation) is the main "escape hatch" from Zapier/Make's pricing. Zero per-task fees. But it comes with a significant trade-off: **it requires infrastructure knowledge to run, maintain, and update**. For the typical SMB owner who just wants their CRM to talk to their email tool, spinning up and managing an n8n instance is a non-starter.

**The paradox:** The users most burned by Zapier's pricing are often small businesses with low technical capacity — exactly the users who can't operationalise n8n without hiring a developer to do it.

**n8n Cloud** (the managed version) addresses the maintenance issue but reintroduces pricing pressure — users on the cloud version are paying again, reducing the cost advantage.

**Source:** Reddit r/SaaS, hatchworks.com — 2026

---

### 🔴 "$40K/Year Zapier Lesson" — Viral Reddit Post — March 2026

**What happened:** A Reddit post in r/SaaS (March 2026) titled "We Burned $40K/Year on Zapier Before We Finally Woke Up" went viral in the automation and SaaS communities. The poster described a company that had gradually scaled Zapier usage over three years, adding integrations as the business grew, until they opened an annual bill and discovered they'd been paying over $40,000 per year — for automations that move data between APIs in tasks that cost fractions of a cent in actual compute.

**The community reaction:** The post resonated strongly because it's not an edge case. The Zapier pricing model is specifically designed to be invisible at small scale (the "gateway drug" of free/cheap entry tiers) and catastrophic at medium scale. The per-task pricing means costs compound quietly month-over-month as businesses grow.

**The specific pain points documented:**
- Zapier AI steps (LLM-powered workflow actions) cost 5–10x more per execution than standard API-to-API steps
- A workflow that was $50/month in 2022 cost $600/month in 2025 after the AI steps migration
- No cap on monthly spending — the bill arrives after the damage is done
- Cancelling means rebuilding every integration from scratch

**Migration horror:** The poster spent 6 months rebuilding their entire automation stack in n8n self-hosted after the discovery. "We gained our sanity back, but lost six months of engineering time. The ROI math doesn't work either way."

**Source:** Reddit r/SaaS — March 2026

---

### 🟠 AI Agent Steps Are Zapier's Most Expensive Items

**What happened:** As Zapier and Make introduced AI-powered steps (LLM calls, AI classification, intelligent routing), they priced them at a significant premium over standard trigger-action steps. In Zapier's task billing model:
- Standard steps (e.g., send Slack message, update Airtable row): 1 task
- AI steps (e.g., classify with ChatGPT, summarise email): 5–10 tasks per execution

A workflow that previously cost 1,000 tasks/month becomes 5,000–10,000 tasks/month when AI steps are added — pushing users from the Professional plan ($30/month) into the Teams tier ($100+/month) immediately.

**Why this matters:** AI automation is the stated future of the category. If the pricing model makes AI steps unaffordable for SMBs, the companies that need AI automation most (lean teams, small businesses) are priced out. The large enterprises that can afford it don't need the cost savings as urgently.

**Community verdict (r/automation, March 2026):** "Zapier's AI steps are a trap. They get you hooked on automating with AI during the free trial, then the bill comes in."

**Source:** Reddit r/automation, Zapier pricing documentation — March 2026

---

**Overall picture for 2026 automation market:**

The space is deeply dysfunctional for mid-market users. Large enterprises use custom solutions. Technical founders self-host n8n. Everyone in between is trapped in Zapier/Make pricing escalation. The emergence of AI agent workflows (LLM-powered steps, not just trigger-action) is adding new complexity without solving the underlying pricing problem — and AI steps are among the most expensive per-task items in Zapier's catalogue.
