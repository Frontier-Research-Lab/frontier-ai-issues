# automation — AI Issues Radar

_Last updated: 2026-03-15_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 1 | 🔴 Critical | Zapier pricing rage — what started at $10/month has ballooned to $750+/month for basic automations; mass migration underway | Zapier | Ongoing |
| 2 | 🟠 Major | "Zapier Tax" — per-task pricing model penalises growth, destroying SaaS margins as automation volume scales | Zapier | Ongoing |
| 3 | 🟠 Major | Make (formerly Integromat) — steep learning curve and performance slowdowns with heavy data volumes | Make | Ongoing |
| 4 | 🟡 Notable | n8n self-hosted maintenance burden; requires engineering resources most target users don't have | n8n | Ongoing |

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

**Overall picture for 2026 automation market:**

The space is deeply dysfunctional for mid-market users. Large enterprises use custom solutions. Technical founders self-host n8n. Everyone in between is trapped in Zapier/Make pricing escalation. The emergence of AI agent workflows (LLM-powered steps, not just trigger-action) is adding new complexity without solving the underlying pricing problem — and AI steps are among the most expensive per-task items in Zapier's catalogue.
