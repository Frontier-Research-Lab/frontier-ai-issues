# ux-ui-design — AI Issues Radar

_Last updated: 2026-03-29_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 0mar29 | 🟠 Major | **Figma AI credits now purchasable — confirms monetisation squeeze is permanent** — Figma release notes (week of March 29): "Rolling out this week, admins can now purchase additional AI credits to use in Figma"; this move confirms Figma's AI feature gating is not a temporary limit but a permanent pay-to-use model; following backlash over the credit enforcement going live March 18, Figma's response is to sell more credits rather than fix the underlying access problem; Reddit r/FigmaDesign: "Figma Make isn't keeping my design system components. Anyone else?" — LLM ignores component libraries entirely, "no point in having the feature if it does not read the components" | Figma AI / Figma Make | Active (rolling out March 29, 2026) |
| 0mar28 | 🟠 Major | **Figma Canvas now "open to agents" — but Figma Make still ignores your design system** — Figma blog (March 26): Figma Canvas opened to third-party AI agents (Cursor, Warp, Factory, etc.); however core Figma Make product still fails to read design system library components; forum thread "Figma Make not using my library components" still unresolved since June 2025; LLM "rips styles from the library and tries to interpret them the best it can" but ignores component structure entirely; opening canvas to agents while the native AI product is broken alienates the core professional user base | Figma Make / Figma Canvas | Active (March 26–29, 2026) |
| 0NEW | 🟠 Major | **Figma Dev Mode paywall backlash** — Dev Mode (once free) now requires paid seats; replaced the free Inspect panel; forum threads running hundreds of replies; comparisons to Adobe's predatory pricing "circulating widely"; UX Collective: "40% of small agencies now review their software budgets" (March 2026) | Figma | Active (March 2026) |
| 0x | 🟠 Major | Canva global outage March 22 — thousands affected worldwide; photo and video editing blocked; Downdetector spike at 5:40PM ET; global media coverage; residual issues March 23 (now resolved) | Canva | Resolved (March 22–23, 2026) |
| 0 | 🔴 Critical | Google Stitch "vibe design" update wipes 12% off Figma stock in two days — March 18 platform overhaul adds Voice Canvas + natural-language UI generation; Figma now down 35% YTD and ~85% from IPO peak; CNBC confirms "Google launched an AI-design platform, pushing Figma shares down 12% in two days" | Figma / Google Stitch | Active (March 18–20, 2026) |
| 1 | 🔴 Critical | Figma AI credits enforcement NOW LIVE (March 18) — users hitting walls mid-project today; surprise charges for additional credits; pay-as-you-go only available to Org/Enterprise | Figma AI / Figma Make | Active (March 18, 2026) |
| 2 | 🔴 Critical | Grammarly "Expert Review" class action — AI impersonated real writers/journalists without consent; feature pulled after lawsuit filed | Grammarly (Superhuman) | Active (filed Mar 11, 2026) |
| 3 | 🔴 Critical | Adobe CEO exits; stock down 7% today, -38% over past year — AI disruption trade accelerating | Adobe | Active |
| 4 | 🔴 Critical | Adobe down 12% earlier this week on Q1 guidance — "show-me" story as AI revenue transition slower than promised | Adobe | Active |
| 5 | 🟠 Major | Figma subscription price complaints escalating — users report "significantly higher" charges vs last year with no feature parity justification | Figma | Active (March 2026) |
| 6 | 🟠 Major | Figma's role narrowing as vibe coding shifts deliverable from mockups to working software — designers "outgrowing" the tool | Figma | Developing |
| 7 | 🟠 Major | Figma down 81% from peak valuation (Jan 2026) — AI-native tools attacking the design tool market from below | Figma | Ongoing |
| 8 | 🟡 Notable | Adobe's failed $20B Figma acquisition left a $1B termination fee and a wasted strategic window | Adobe | Historical |

---

## Details

### 🟠 Figma Dev Mode Paywall Backlash — Free Inspect Removed, Paid Seat Required — March 2026

**What happened:** Figma has moved its **Dev Mode** — formerly accessible to developers and stakeholders at no extra cost — behind a paid seat requirement. The change replaced the free **Inspect panel** that had been available to everyone (viewers and guests), which was the primary way non-designer collaborators could inspect design specs, extract CSS values, and copy assets.

**Community reaction:** Per UX Collective analysis (March 2026):
- Forum threads on the Figma community forum ran to hundreds of replies
- Comparisons to Adobe's pricing practices — "unflattering ones" — circulated widely across design Twitter/X and LinkedIn
- UX Collective documented that "40% of small agencies now review their software budgets" as a direct consequence of Figma's compounding pricing changes
- The move was characterised as "enshittification" by designers — a pattern of eliminating free features to force paid upgrades

**Compounding pricing pressure:** This paywall is the latest in a series of Figma monetisation moves that have eroded goodwill:
- Dev Mode → paid seat
- Figma AI → credits (enforcement March 18, 2026)
- Subscription cost inflation year-over-year
- Meanwhile, Google Stitch (free, backed by Gemini 2.5 Pro) is a direct free competitor

**Who's affected:** Development teams and agencies who relied on the free Inspect workflow. "Engineering-first" teams especially impacted — many of whom are now evaluating whether Figma's per-seat costs for developers are justified when Google Stitch and open-source alternatives offer inspection capabilities.

**Sources:** UX Collective ("Who can actually afford AI tools now?", Dora Czerna, March 2026), Byter.com Design Tool Transition Guide — March 2026

---

### 🟠 Canva Global Outage — Thousands Blocked from Photo and Video Editing — March 22–23, 2026

**What happened:** Canva experienced a significant global outage on March 22, 2026, blocking users worldwide from accessing photo and video editing features. The platform is used by hundreds of millions of users — students, small businesses, marketers, educators — many of whom have come to depend on it as their primary creative tool.

**Timeline:**
- **March 22:** Downdetector showed a visible spike in reports starting at approximately **5:40PM Eastern Time**; multiple social media reports confirmed editing, project access, and platform loading failures
- **March 23 morning:** Brief residual loading issues reported by some users; third-party monitors (Downforeveryoneorjustme.com, IsItDownRightNow.com) confirmed Canva was reachable by mid-day with low response times
- The most recent detected full outage lasted approximately one hour per Downforeveryoneorjustme.com

**Affected functionality:** Users reported being unable to edit photos, videos, and projects. Website and app both showed problems. Multiple international outlets covered the outage (Koha.net in Albania, DeUltimoMinuto in Mexico/Spanish-language media).

**Context:** This is part of a broader reliability pattern for creative AI tools this week — Canva's outage, Claude Outage #11, and ChatGPT downtime all occurred within a 24-hour window (March 22–23). Canva has also been reported as a secondary front in the AI design competition following Google Stitch's expansion (r/UXDesign: "companies like Canva with AI tools eat Figma's place in creating marketing materials").

**Official response:** No public statement from Canva on root cause.

**Sources:** DesignTAXI Community, Downdetector, IBTimes Australia, Koha.net, DeUltimoMinuto.net — March 22–23, 2026

---

### 🔴 Google Stitch "Vibe Design" Update Triggers Figma Stock Crash — March 18–19, 2026 (BREAKING)

**What happened:** On March 18, 2026, Google Labs released a major platform-level update to **Stitch**, its AI-native UI design tool, that sent shockwaves through the design industry. Figma shares (NYSE: FIG) fell **8.8% on March 18** — their steepest single-day decline in over a month — and continued falling, trading down a further **5% on March 19**. Figma stock is now down approximately **85% from its IPO peak**.

**What changed in the Stitch update:**
- **"Vibe Design"** — Google's term for prompt-based UI generation: describe the experience in natural language, Stitch generates full UI compositions. "No wireframes, no artboards, no manual layout. Just intent in, design out."
- **Voice Canvas** — users can now **speak directly to the Stitch canvas** to create and modify designs in real time; the AI agent listens and acts
- The tool generates "high-fidelity" UI design **and** front-end code simultaneously
- Stitch is **completely free**, backed by Google's Gemini 2.5 Pro models

**Why the market is scared:** Figma's core value proposition — being the place where UI design happens — is under siege from a tool backed by Google's unlimited resources and given away for free. The parallel to "vibe coding" (writing software via natural language) is explicit: Google is betting "vibe designing" becomes the dominant paradigm for UI creation in 2026.

**Figma's already-weakened position:**
- Stock was already down ~85% from peak before this drop
- Post-IPO enterprise ramp has been slower than expected
- Adobe's failed $20B acquisition attempt left Figma competing alone against both legacy (Adobe) and AI-native (Google, Anthropic-backed tools) threats
- The Figma AI credit enforcement (rolled out March 18) added user friction at the exact moment Google launched its free alternative

**Design community reaction:** Mixed — many designers note that Stitch still lacks the collaborative features, design system depth, and handoff precision of Figma. The NxCode analysis concluded: "The market's reaction reveals a misunderstanding of what these tools actually do and who they serve." But the direction of travel is unmistakeable.

**Long-term view:** Figma has ~13x trailing revenue multiple (still a premium vs Adobe's 5.8x) despite the stock decline — the market is still pricing in some future growth. But a free Google competitor entering the "AI-native UI design" space makes that premium increasingly hard to justify for investors.

**Source:** Business Insider, NxCode, Stocktwits, Investing.com, Indian Express — March 18–19, 2026

---

### 🔴 Grammarly "Expert Review" Class Action — AI Impersonated Real Writers — March 11, 2026

**What happened:** Grammarly's parent company Superhuman launched an "Expert Review" feature that offered users writing feedback framed as coming from established journalists, authors, and academics — including The Markup's editor-in-chief **Julia Angwin** and other real, named experts. The experts had **not consented to having their identities used**.

On March 11, 2026, Angwin filed a **class action lawsuit** (Angwin v. Superhuman) alleging:
- Grammarly misappropriated the names and identities of prominent journalists and writers
- The "Expert Review" feature presented AI-generated feedback as if it came from real, named humans
- No consent was obtained from the people whose names and reputations were used
- Users paid for a premium feature believing they were getting genuine expert input

**Grammarly's response:** The company **disabled the Expert Review feature** on March 11, immediately after the lawsuit was filed (or simultaneously with its announcement). The Guardian (March 13, 2026) confirmed the feature was pulled "after expert rebellion and class action suit."

**Why this matters beyond Grammarly:** The Expert Review concept — AI giving feedback "in the voice of" a real expert — is a pattern spreading across AI writing tools. This is the first major class action specifically targeting AI identity appropriation. The multimillion-dollar lawsuit (if successful) sets precedent that any AI tool that names real humans as the source of AI output could face similar liability.

**Scale:** Grammarly has 30+ million active users. The Expert Review feature was positioned as a premium value-add for paid subscribers.

**Community reaction:** The backlash was immediate and from multiple directions: the named experts were furious, writers' advocacy groups called it "straightforward identity theft," and users who paid for the feature felt misled about what they were actually receiving.

**Source:** WIRED, The Guardian, NYC Today, AV Club, PRF Law — March 11–13, 2026

---

### 🔴 Adobe CEO Exit + Stock Collapse — March 13, 2026 (Today)

**What happened:** Adobe's long-time CEO announced today (March 13, 2026) they would step down. Shares immediately dropped **6–7.34%** in the session — the company's worst single-day percentage fall since September 2022. The departure arrives at the worst possible time: Adobe is already down **37.7% over the past year** and **18.9% YTD 2026**, trading at a 52-week range low of approximately $270 (vs high of $443).

**The core problem:** Adobe is not a bad business — it beat earnings 13 consecutive quarters. The issue is **AI disruption anxiety**. Canva, Figma, and AI-native design tools are growing fast. Adobe's Firefly AI tools exist but analysts at Morgan Stanley and UBS describe a "show-me story" — AI features are live, but the **transition from experimentation to meaningful revenue is taking longer than the market expected**.

**Quote from analyst consensus:** "The current guidance suggests challenges ahead including heightened competition in the AI software space and potential margin pressures."

**Source:** Reuters, Benzinga, TradingKey — March 13, 2026 (today)

---

### 🔴 Adobe 12% Single-Day Plunge on Q1 Guidance — March 12, 2026

**What happened:** Just one day before the CEO exit news, Adobe posted Q1 guidance that disappointed the market. Stock dropped 12% in a single session — its worst drop in years. Despite strong current performance, the forward guidance implied the AI revenue ramp is slower than anticipated.

**The $25 billion share buyback distraction:** Adobe announced a massive $25B repurchase program alongside earnings — widely seen as a financial engineering move to offset stock decline rather than a sign of strategic confidence.

**Background — failed Figma deal:** Adobe attempted to acquire Figma for ~$20 billion. The deal was blocked on antitrust grounds, costing Adobe **$1 billion in termination fees** and leaving it without the design community's most beloved tool. Figma went on to IPO independently.

**Source:** FinancialContent, markets.chroniclejournal.com — March 12, 2026

---

### 🟠 Figma's Role Narrowing as Vibe Coding Changes the Deliverable — March 2026

**What happened:** A widely-shared analysis by Roger Wong (rogerwong.me, March 9, 2026), titled "Why Are Designers Leaving Figma? The Great Transition," captures a structural shift in how design tools are used in 2026:

> "Designers aren't leaving Figma so much as outgrowing it. As vibe coding shifts the deliverable from mockups to working software, Figma's role is narrowing rather than disappearing."

**The structural shift:** In 2024, designers handed developers a Figma file. In 2026, AI coding tools (Claude Code, v0, Bolt, Lovable) let teams jump from rough sketch to deployed application without traditional Figma mockup handoffs. The deliverable has changed:
- Previously: **Figma prototype → developer build**
- Now: **Rough sketch/prompt → AI-generated working app**

This doesn't make Figma disappear — it's still the best tool for visual design refinement and design systems — but it removes Figma from a step that used to be central to every product build.

**Who's affected:** Product teams at startups and agencies building web/app products. Figma's value proposition was "the complete tool from wireframe to developer handoff" — that positioning is being challenged as the developer handoff step is automated.

**Community reaction:** Reddit r/ClaudeAI thread (March 2026): "Claude is making me question whether web designers will exist in 5 years?" — hundreds of comments from designers grappling with the shift. The dominant view: UX and design are not disappearing, but the workflow is fundamentally changing.

**Figma's response:** New AI-powered features (Buzz, Draw, Make, Sites) launched at Config 2025 attempt to position Figma as an AI-native design tool. The market remains skeptical that these features meaningfully close the gap with AI-first competitors.

**Source:** rogerwong.me, Reddit r/ClaudeAI, fourweekmba.com — March 2026

---

### 🟠 Figma — 81% Decline From Peak Valuation

**What happened:** By January 2026, Figma had lost **81% of its peak valuation**. The IPO was initially valued at a massive premium to revenue; AI-native tools entering the design space have compressed growth expectations dramatically. Figma now trades at ~13x trailing revenue — still a premium to Adobe's 5.8x, but no longer pricing in hypergrowth.

**The AI pressure:** Figma launched four new AI-powered products at Config 2025 (Buzz, Draw, Make, Sites) to defend against AI-first website builders and design tools. But the market is skeptical. AI coding tools like v0 (by Vercel) can generate functional UI from a text prompt, bypassing Figma's design-to-code workflow entirely for many use cases.

**Source:** davefriedman.substack.com — January 2026

---

### 🟡 Adobe's Wasted Figma Window

**What happened:** Adobe's 2022 attempt to acquire Figma for $20 billion would have secured the dominant design tool for the next decade. Antitrust regulators in the EU and UK blocked the deal in 2023. Adobe paid a $1 billion break fee. Three years later, Figma is an independent public company, Adobe stock is down 38%, and every AI startup that builds a design tool adds further competitive pressure.

**The counterfactual:** Had the deal closed, Adobe would own Figma's design community lock-in, browser-native collaboration, and prototyping toolset — defensive moats that would be far more valuable against AI disruption than Adobe's current position.

**Source:** stocktwits.com, thetechtrep.com — ongoing context

---

### 🔴 Figma AI Credit Enforcement — NOW LIVE — March 18, 2026 (TODAY)

**What happened:** Figma announced in December 2025 that **AI credits would be enforced starting March 18, 2026** — and that day is today. The announcement (Figma Forum, "AI credits update: new purchasing options and enforcement on March 18") details:

**What's changing:**
- AI credits are included with every Figma seat and reset monthly
- Starting March 11, new purchasing options rolled out (rolling across accounts through March 12)
- **Starting March 18: credit limits will be enforced** — users who exhaust their monthly credits will be blocked from AI features mid-project

**The pricing problem:**
- Additional credits are available via subscription or pay-as-you-go — but **only for Organisation and Enterprise plans**; Professional plans must wait until May 2026
- Users on Professional plans hit their limit have no ability to purchase additional credits until May
- Users who weren't tracking their credit usage will hit walls without warning

**Subscription price complaints:** Separately, Figma Forum users (March 2026) are complaining that subscription prices have increased significantly vs. last year with the same charges appearing "significantly higher" — suggesting Figma is quietly raising prices while simultaneously metering AI features.

**State of UX 2026 context:** Nielsen Norman Group's annual State of UX 2026 report described the design field as still recovering from "instability from layoffs, hiring freezes, and AI hype." Adding surprise AI credit walls to a field already under financial stress is particularly poorly timed.

**Community reaction:** As enforcement goes live today, designers are now hitting credit limits mid-sprint. The predicted disruptions are materialising — users on Professional plans have no ability to purchase additional credits until May, and the surprise walls are landing mid-project as expected. The limited availability of credit top-ups for non-Enterprise plans is confirmed as a "Professional plan tax."

**Source:** Figma Forum ("AI credits update" thread), releasebot.io, Nielsen Norman Group State of UX 2026 — March 2026

---

### 🟠 Figma Make Ignores Design System Components — Core AI Feature Still Broken — March 2026

**What happened:** Reddit r/FigmaDesign thread "Figma Make isn't keeping my design system components. Anyone else?" confirms a persistent issue: **Figma Make's LLM ignores component libraries entirely**. When users connect their Figma design system (components, variants, tokens), Figma Make's AI disregards the component structure and instead "rips the styles from the library and tries to interpret them the best it can." The result is AI-generated designs that don't use your components, creating design debt rather than respecting established systems.

**Figma Forum evidence:** Forum thread "Figma Make not using my library components" (originally filed June 2025) remains unresolved as of March 2026. A forum commenter summarised the core issue: "same issues as above — got a better overall result without using my library so there is no point in having the feature if it does not read the components either in the design linked or in the library linked."

**Why this matters:** Figma Make was sold as an AI design tool that works within your design system. Professional designers who have invested hundreds of hours building component libraries find that Figma's AI feature provides zero benefit from their investment — it generates fresh layouts ignoring established components, creating inconsistency and rework. Figma opened its Canvas to third-party agents (Cursor, Warp, Factory) on March 26, 2026 — but the core native AI tool that most users interact with daily still has this fundamental flaw.

**Who's affected:** Any Figma user on Org/Enterprise plan who has built a component library and expects Figma Make to use it. Estimated many thousands of professional users.

**Source:** Reddit r/FigmaDesign, Figma Forum, Figma blog (March 26, 2026)

---

### 🟠 Figma AI Credit Top-Up Now Purchasable — Confirms AI Paywall Is Permanent — March 29, 2026

**What happened:** Figma release notes (week of March 29, 2026) confirm: "Rolling out this week, admins can now purchase additional AI credits to use in Figma." This move, rather than resolving user complaints about the credit enforcement that went live March 18, **institutionalises the paywall** — AI features are confirmed as a permanent metered resource, not a subscription perk.

**The pattern:** Since March 18, designers hitting their monthly AI credit limit are blocked from Figma AI and Figma Make features mid-project. Figma's response to the backlash was not to increase limits or reconsider the model — it was to add a purchase flow for more credits.

**Community reception:** The "Figma Make isn't keeping my design system components" thread (Reddit) and the ongoing Figma Dev Mode paywall backlash are layering: users are being asked to pay more for a tool that doesn't work correctly. The combination of mandatory paid Dev Mode + AI credit enforcement + component library incompatibility is driving small agencies and freelancers to evaluate alternatives.

**Source:** Figma release notes (March 29, 2026), Reddit r/FigmaDesign
