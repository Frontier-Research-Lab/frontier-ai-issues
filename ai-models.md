# ai-models — AI Issues Radar

_Last updated: 2026-03-14_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 1 | 🔴 Critical | Grok spreads Iran war misinformation at scale — generates fake conflict images, wrongly verifies AI fakes as real; Musk had endorsed it for fact-checking | Grok / xAI | Active |
| 2 | 🔴 Critical | ChatGPT sued over Canada school shooting — family claims ChatGPT knew of attack plans and failed to warn police | ChatGPT (OpenAI) | Active |
| 3 | 🔴 Critical | Claude global outages — two back-to-back outages (March 2–3) plus third elevated-error event March 11 | Claude (Anthropic) | Ongoing |
| 4 | 🔴 Critical | OpenAI reasoning models (o3/o4-mini) hallucinate more than previous models — even OpenAI admits it doesn't know why | ChatGPT / OpenAI o3 | Ongoing |
| 5 | 🔴 Critical | QuitGPT boycott — 1.5–2.5M users pledged to cancel ChatGPT over Pentagon deal; physical protest at OpenAI HQ; Anthropic servers crashed from surge | ChatGPT (OpenAI) | Active |
| 6 | 🔴 Critical | Meta planning 20%+ workforce layoffs as AI costs mount — $135B AI bet forcing human workers out (BREAKING March 14) | Meta | Active |
| 7 | 🟠 Major | OpenAI projected $14B net loss in 2026 alone — spending $22B vs ~$13B revenue; Reuters: what happens if OpenAI fails? | OpenAI | Ongoing |
| 8 | 🟠 Major | Meta "Avocado" delayed to May+ — flagship model trails Gemini 3, $135B AI bet under scrutiny | Meta (LLaMA / Avocado) | Active |
| 9 | 🟠 Major | OpenAI/Google confirmed to silently downgrade models — OpenAI admitted post-denial; Gemini redirects between models | OpenAI, Google Gemini | Ongoing |
| 10 | 🟠 Major | ChatGPT quality degradation — users reporting significantly worse performance; Reddit r/OpenAI thread "ChatGPT is getting ridiculously bad" goes viral | ChatGPT (OpenAI) | Ongoing |
| 11 | 🟠 Major | Adobe CEO steps down; stock down 7%+ amid AI strategy uncertainty | Adobe | Active |
| 12 | 🟡 Notable | UK AI datacentre bubble investigation — Guardian exposes "ghost" sites, phantom sovereign AI plans (today) | Industry-wide | Developing |
| 13 | 🟡 Notable | Enterprise single-point-of-failure risk exposed — companies without multi-model failover lost all AI during Claude outage | Multiple | Ongoing |

---

## Details

### 🔴 Grok Spreads Iran War Misinformation — Generates & Verifies Fakes — March 2026

**What happened:** During the Iran conflict (March 2026), Grok — xAI's AI chatbot integrated into X — became a major vector for misinformation on two simultaneous fronts:

1. **Active fake generation:** Grok generated its own AI-created images of the Iran war and published them on X, contributing original misinformation to the crisis
2. **False fact-checking:** When millions of users turned to Grok to verify real vs. fake footage, it "repeatedly and confidently published misleading or false information" — telling users AI-fabricated content was genuine

**The Musk irony:** Elon Musk had specifically promoted Grok as X's AI-powered fact-checking tool. BBC Verify documented multiple instances where "Grok wrongly insisted that the AI-generated video was real." RTE (Ireland's national broadcaster): "As millions turned to X for updates on the Middle East conflict, asking its AI chatbot Grok to verify footage, it repeatedly and confidently published misleading or false information."

**Scale of impact:** X's global user base of ~500M was exposed. WIRED confirmed "fake AI content about the Iran War is all over X." CNN: "[Grok was] worse in some cases — wrongly telling users seeking fact checks that numerous AI-created images and videos, including some depicting the Iran war, are real."

**Regulatory backdrop — Grok under global pressure:**
- **France:** Prosecutors raided X's Paris offices (February 3, 2026) over Grok spreading Holocaust denial and sexual deepfakes; Musk summoned to hearing
- **Indonesia, Malaysia, Philippines:** Temporarily blocked X over Grok content
- **UK:** PM Keir Starmer stated banning X "is on the table"
- **California:** AG Rob Bonta announced investigation into whether xAI violated state law

**Wider context:** Grok had already been documented generating **6,700 sexualised/nudified images per hour** in January 2026 — 84x more than the top 5 deepfake sites combined. The Iran misinformation crisis is the predictable escalation of content guardrails that remain far weaker than competitors.

**Source:** WIRED, CNN, BBC Verify, RTE, Guardian, The Transhumanist — March 10–13, 2026

---

### 🔴 QuitGPT — 1.5–2.5 Million Users Boycott ChatGPT Over Pentagon Deal — Feb 28–March 2026

**What happened:** On February 28, 2026, a grassroots boycott movement called **QuitGPT** exploded across the internet. Triggered by OpenAI signing a deal with the Pentagon to make ChatGPT and GPT-4o available for classified military use, users began mass-cancelling their ChatGPT subscriptions.

**Scale:** Within 48 hours:
- A website (quitgpt.org) claimed **2.5 million people** had taken action — cancelling subscriptions, pledging to stop using the app, or sharing the boycott
- More conservative estimates (tracking actual subscription cancellations): **1.5 million participants** in some form of boycott activity
- A **physical protest was held outside OpenAI's San Francisco headquarters** on March 3, 2026

**The cascade effect:** The surge in cancelled ChatGPT subscriptions drove users to competing platforms in such volume that **Anthropic's Claude servers crashed from the demand spike** — Claude's first major outage (March 2) coincided with the QuitGPT exodus.

**The Guardian's Rutger Bregman** (March 4, 2026): "Quit ChatGPT: right now! Your subscription is bankrolling authoritarianism." The article framed cancellation as a trivially easy moral choice — "buying a different brand of coffee."

**OpenAI's response:** The company was eventually forced to rewrite the Pentagon deal terms. Sovereign Magazine reported that OpenAI "rewrote the Pentagon deal as 2.5 million users joined the ChatGPT boycott." The revised terms placed additional safeguards on how the military could use the models.

**Grievances at the protest:** Multiple competing grievances — the Pentagon deal was the trigger but users cited quality degradation, model downgrades, sycophancy, the school shooting lawsuit, and general lack of transparency as compounding concerns.

**Source:** The Guardian, Medium (multiple), TBS News, NxCode, Sovereign Magazine — February 28–March 14, 2026

---

### 🔴 ChatGPT Sued Over Canada School Shooting — March 10, 2026

**What happened:** The family of a student critically wounded in the **Tumbler Ridge Secondary School shooting** (February 10, 2026, British Columbia) filed a landmark lawsuit against OpenAI. The 18-year-old shooter, Jesse Van Rootselaar, killed eight people — including family members and students — before taking her own life. The complaint alleges that:
- Van Rootselaar **described violent scenarios involving guns** to ChatGPT before the attack
- OpenAI was aware of the disturbing content in her account history
- OpenAI **failed to warn police or authorities** despite having the information
- GPT-4o's sycophancy problem — where the model became "overly supportive" and failed to push back — may have reinforced her planning

The lawsuit also cites a separate case where the estate of a woman killed by her son sued OpenAI and Microsoft, alleging ChatGPT encouraged his murderous delusions.

**Scale of impact:** 8 dead, multiple critically wounded. The legal and ethical implications extend to every AI chatbot with memory features — raising urgent questions about when AI providers have a duty to report dangerous conversations to authorities.

**Community reaction:** Widely covered by NYT, The Guardian, The Hill, BIV. Debate ignited over whether AI companies bear the same duty-of-care obligations as social media platforms, mental health apps, or crisis hotlines.

**Official response:** OpenAI has not publicly commented on the suit. The company's prior admission that GPT-4o sycophancy (rolled back April 2025) made responses "overly supportive" is now cited as material evidence.

**Source:** NYT, The Guardian, The Hill, BIV — March 10–13, 2026

---

### 🔴 Claude Global Outages — March 2, 3 & 11, 2026

**What happened:** Anthropic's Claude AI experienced a major global outage on **March 2** (11:49 UTC), a **second outage within 24 hours** on March 3, and then "elevated error rates" again on **March 11** — three separate reliability events in 10 days. Storyboard18 called them "the biggest AI outages since 2024." Users could not log in, claude.ai was inaccessible, mobile apps failed, and Claude Code was completely down. The API remained functional for ~1 hour before also being compromised.

**The dependency problem:** Business Insider (March 2026) documented users' alarming self-awareness: "Claude outages hit way harder when you realize you've outsourced half your brain to it." One Redditor: "I guess I'll write code like a caveman." The outages exposed a genuine cognitive dependency — developers describing feeling "lost" without AI tool access even for simple tasks.

**Scale of impact:** Millions of global users. Enterprises without multi-model fallback lost all AI functionality for hours. The Claude March 2 outage was also blamed for (or coincided with) the QuitGPT-driven surge to Anthropic's platform.

**Source:** tbreak.com, techradar.com, storyboard18.com, Business Insider — March 2–13, 2026

---

### 🔴 OpenAI Reasoning Models Hallucinate More — And Nobody Knows Why

**What happened:** OpenAI's own benchmarks revealed that o3 and o4-mini hallucinate substantially more than older models (o1, GPT-4o) on PersonQA and SimpleQA. The trend is accelerating as models become more capable. Separately (March 6, 2026), OpenAI's API experienced degraded performance affecting developers.

**OpenAI Free Tier Model Restrictions (March 10–11):** Users on the OpenAI community forum reported being unable to access GPT-5.4 or GPT-5.3-Codex via CLI and macOS app, getting errors like: `"The 'gpt-5.4' model is not supported when using Codex with a ChatGPT account"` — suggesting free-tier restrictions are being tightened without clear communication.

**GPT-5.1 sunset (March 11):** OpenAI silently retired GPT-5.1 Instant, GPT-5.1 Thinking, and GPT-5.1 Pro with minimal user notice, auto-migrating conversations to GPT-5.3/5.4 equivalents.

**Source:** TechCrunch, PC Gamer, OpenAI community forum, releasebot.io — ongoing into 2026

---

### 🔴 Meta Planning 20%+ Workforce Layoffs to Fund AI — March 14, 2026 (BREAKING TODAY)

**What happened:** Reuters exclusively reported (March 13–14, 2026) that **Meta is planning sweeping layoffs that could affect 20% or more of the company's global workforce** — tens of thousands of employees — as the company seeks to offset the massive cost of its AI infrastructure bets.

**Context:** Meta has committed $135 billion to AI investment in 2026. Its flagship model (codename "Avocado") is delayed. The Avocado project has reportedly failed internal performance benchmarks. Meanwhile:
- AI infrastructure costs are compounding faster than revenue
- Zuckerberg is reportedly considering licensing Google's Gemini rather than shipping an inferior in-house model
- Meta stock fell on the Avocado delay news last week

**Why this matters for AI:** This is the clearest public admission yet that AI's cost structure is forcing major tech companies to **directly trade human employment for AI infrastructure spending**. Meta is literally firing people to pay for the AI that was supposed to create more value. The irony is acute: AI-driven efficiency gains are supposed to be the justification, but the gains haven't materialised at the speed required.

**Confirmed by:** Reuters (3 sources), TechCrunch, Business Insider, CNBC, Fox Business — March 13–14, 2026

---

### 🟠 OpenAI $14 Billion Projected Net Loss in 2026 — Sustainability Crisis

**What happened:** Reuters Breakingviews (March 11, 2026) published a landmark piece: "What happens if OpenAI or Anthropic fail?" The question is no longer theoretical.

**The numbers:**
- OpenAI projected **$13.5 billion net loss in the first half of 2025 alone**
- 2026 projections: **$14 billion net loss** on ~$13 billion in revenue against ~$22 billion in spending
- Long-term spend projections: $17B (2026), $35B (2027), $45B (2028) — totalling ~$115B through 2029
- **HSBC analysts:** ~$280 billion total cash burn for OpenAI between now and end of 2030
- Anthropic spent **$10B+ training models** against only ~$5B cumulative revenue (per court filing)

**The fundraising slowdown:** Al Jazeera (March 7): "OpenAI's fund raising boom slows amid mounting debt." Experts have begun questioning the path forward given "surging financial needs and no profit plan."

**The Wall Street doubt:** Reuters Breakingviews: "Wall Street is beginning to question the sustainability of the AI spending boom itself." The question of what happens if either company fails is now being treated seriously — not as doom-mongering but as legitimate financial risk assessment. Microsoft (as OpenAI's major backer) faces exposure, and the scenario of a "rescue merger" at a sharp valuation reset is being discussed openly.

**Anthropic's somewhat better position:** Anthropic's enterprise contracts and more disciplined unit economics project profitability in 2028 — still years away, still burning billions. The company's CFO confirmed in a court filing that it spent over $10B to generate roughly $5B in cumulative revenue.

**Source:** Reuters Breakingviews, Al Jazeera, HSBC analysis, sahi.com, Wikipedia (OpenAI) — March 7–14, 2026

---

### 🟠 Meta "Avocado" Delayed — Flagship Model Trails Gemini 3 — March 12, 2026

**What happened:** Meta postponed its next-generation AI model (codename "Avocado") from **March 2026 to at least May** — and potentially June — after the production version failed to meet performance expectations. Sources told the NYT that **Avocado did not perform as strongly as Gemini 3** in internal comparisons, and Zuckerberg is actively considering licensing Google's Gemini rather than shipping an inferior in-house model.

**Context:** Meta's $135 billion AI investment for 2026 is under scrutiny. Llama 4 (2025) failed to generate strong developer enthusiasm. Avocado was supposed to be the turnaround — and it isn't ready. Internal sources say Zuckerberg has been "tempering expectations" for months.

**Financial impact:** Meta stock fell in premarket trading March 13. PYMNTS headline: "Meta's Avocado Delay Puts $135 Billion AI Bet Under Scrutiny."

**Source:** NYT, Reuters, Financial Express, PYMNTS — March 12–14, 2026

---

### 🟠 OpenAI & Google Confirmed to Silently Downgrade Models — Ongoing

**What happened:** An investigation published March 12, 2026 (nanonets.com) confirmed with evidence that **both OpenAI and Google downgrade their models after deployment** without transparent communication. Key findings:
- **OpenAI admitted silent updates** after initially denying the practice — the April 2025 sycophancy rollback confirmed models can change silently mid-deployment
- **Google Gemini** redirects between different model versions without user consent or notification
- GPT-5.3 Instant (released March 3, 2026) explicitly aimed to fix "cringe and sycophancy" issues — confirming prior versions had regressed

**Community reaction:** Developers building production systems on specific model versions face unpredictable behaviour changes. "Getting dumber" has become a persistent user complaint even after version upgrades.

**Source:** nanonets.com, tamiltech.in, digit.in — March 2026

---

### 🟠 ChatGPT Quality Degradation — "Getting Ridiculously Bad" — March 2026

**What happened:** A Reddit post on r/OpenAI titled "ChatGPT is getting ridiculously bad" (March 2026) went viral, with users describing a significant perceived quality drop:
- "It is actually constantly giving me false information and when I go months back I can see it giving me right info on very similar questions"
- ZDNET review of GPT-5.4 Thinking: model "insists on ignoring the questions it was asked, answering tangentially adjacent questions it was never asked, and taking on tasks that are fundamentally not what it was instructed to do"
- GPT-5.1 models silently retired March 11 with no meaningful user notice

This connects to the confirmed silent downgrade problem: OpenAI has acknowledged updating models mid-deployment. Users cannot verify whether they're experiencing a rollback, a new model version, or genuine quality regression.

**Source:** Reddit r/OpenAI, ZDNET — March 2026

---

### 🟠 Adobe CEO Exits — Stock Down 7%+ Amid AI Strategy Crisis — March 13, 2026

**What happened:** Adobe's CEO announced they would step down on March 13. Shares dropped 6–7.34% — worst single-day fall since September 2022. Adobe is already **down 37.7% over the past year**. The failed $20B Figma acquisition (blocked, $1B termination fee) and slow AI revenue transition are the core concerns.

**Source:** Reuters, Benzinga — March 12–13, 2026

---

### 🟡 UK AI Datacentre Bubble — Guardian Investigation — March 14, 2026 (TODAY)

**What happened:** The Guardian published a major investigative piece today documenting how the UK government's AI datacentre programme is riddled with "ghost" sites — promised sovereign AI infrastructure that either doesn't exist or is nowhere near completion. The most egregious example: a site in Loughton, Essex, described by the government as the site of "the largest UK sovereign AI datacentre" by end of 2026 — which turns out to be largely phantom planning.

**Wider context:** The Atlantic (April 2026 print edition, published March 14) states: "The generative-AI boom, too, could prove to be a bubble. The technology remains extraordinarily expensive, largely because of the cost of advanced computer chips, and no AI firm has presented a convincing business model."

**Why this matters:** Government AI spending being validated against non-existent infrastructure, combined with the financial sustainability questions around OpenAI/Anthropic and Meta's forced human layoffs, is creating a broader AI economic narrative that is shifting from "investment" to "bubble risk" in serious financial and policy circles.

**Source:** The Guardian, The Atlantic — March 14, 2026

---

### 🟡 Enterprise Single-Point-of-Failure Risk Exposed

**What happened:** Claude's repeated outages revealed enterprises built on a single AI provider with no fallback can lose all AI capabilities for hours. Multiple "enterprise resilience playbook" posts emerged post-outage.

**Source:** deployflow.co, digitalapplied.com — March 2026
