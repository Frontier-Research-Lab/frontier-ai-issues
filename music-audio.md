# music-audio — AI Issues Radar

_Last updated: 2026-03-13_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 1 | 🔴 Critical | Google sued by indie musicians over Lyria 3 — "vertically-integrated syndicate" that illegally copies music, launders ownership, unfairly competes | Google Lyria 3 | Active (filed March 6, 2026) |
| 2 | 🔴 Critical | GEMA v. Suno — German court hears landmark copyright case, ruling expected June 2026 | Suno | Active |
| 3 | 🔴 Critical | Suno enforces paid-only downloads + monthly download caps as part of Warner Music deal — community furious at monetisation pivot | Suno | Active |
| 4 | 🟠 Major | Udio copyright lawsuit (RIAA) still active — unlike Suno, Udio has not yet settled with major labels | Udio | Active |
| 5 | 🟠 Major | AI musicians flooding Spotify — major labels pushing back as synthetic content devalues platform | Multiple | Developing |
| 6 | 🟠 Major | Suno "2026 model" will replace existing version with licensed-only training data — old-style open generation ending | Suno | Developing |
| 7 | 🟡 Notable | Industry backlash grows even as Suno hits 2M paid subscribers — human musicians deeply hostile | Suno, Udio | Ongoing |

---

## Details

### 🔴 Google Sued Over Lyria 3 — "Vertically-Integrated Syndicate" — March 6, 2026

**What happened:** A group of independent musicians and songwriters filed a class action lawsuit against Google on March 6, 2026, accusing the company of:
- **Training its Lyria 3 AI music model** on copyrighted recordings pulled from YouTube without permission or payment
- **"Laundering" music ownership** — stripping metadata and rights information from scraped content
- **Running a "vertically-integrated syndicate"** — Google owns YouTube (where the music lives), controls the AI tool (Lyria 3), and then competes directly with the musicians whose work it stole
- **Unfairly competing** in the marketplace against the very artists whose work it used to build its tools

**Legal claims:** Copyright infringement, unfair competition, unjust enrichment. The lawsuit — filed by law firm Loevy + Loevy on behalf of Chicago-area and other indie artists — is seeking damages for the use of copyrighted recordings without consent or compensation.

**Why this case is different:** Previous AI music suits (RIAA vs. Suno/Udio) were filed by the major labels. This is an **indie artist class action** — representing musicians who don't have label resources to fight tech giants. The "vertically integrated syndicate" framing directly attacks the systemic advantage Google has: own the platform, mine the content, train the AI, then compete with the original creators.

**Scale:** Google's YouTube hosts hundreds of millions of songs. If the court accepts that training on this content constitutes infringement, the remedies could be staggering.

**Industry reaction:** Music Business Worldwide, Billboard, Crain's Chicago Business all covered the filing prominently. The lawsuit has reignited debate about tech platforms that "own the library" using it to train competitors to the original artists.

**Source:** Music Business Worldwide, Billboard, Crain's Chicago Business, Loevy + Loevy press release, OK Magazine — March 6–13, 2026

---

### 🔴 GEMA v. Suno — German Court Hearing, Ruling Expected June 2026 — March 9, 2026

**What happened:** Munich's Hamburg District Court held oral proceedings in the **GEMA v. Suno** copyright case on March 9, 2026 — described as a "packed courtroom" landmark hearing. GEMA (Germany's music rights collective) is suing Suno for copyright infringement, arguing that Suno's AI model was trained on copyrighted music without authorization.

**What makes this pivotal:** Unlike the US RIAA suit (where Suno partially settled), this is a European rights case where the legal framework for AI training data is less settled. The Munich court is expected to rule on whether AI training on copyrighted music constitutes infringement — with a ruling expected **June 2026**.

**The Hamburg contradiction:** A separate Hamburg court had already arrived at the *opposite conclusion* on the same legal paragraph — ruling that AI training may not constitute infringement under German law. The divergence means GEMA v. Suno could set a decisive precedent (or escalate to Germany's Federal Court of Justice).

**Context:** Suno did settle with Warner Music Group in November 2025, ending WMG's US case — but that deal explicitly did not resolve the broader European and indie-artist claims. The "launch, train, settle" playbook that Suno apparently used is now under direct legal attack in Munich.

**Source:** Digital Music News, Music Business Worldwide, Billboard, Medium — March 9–12, 2026

---

### 🟠 AI Musicians Flooding Spotify — Major Labels Pushing Back — March 2026

**What happened:** AI-generated music is flooding Spotify at a scale that is visibly impacting the platform. Substream Magazine (March 2026): "AI musicians are flooding Spotify — is the music industry in trouble?" Key dynamics:
- Spotify's royalty pool is being diluted by high volumes of synthetic content
- Major record labels are beginning to formally push back against AI-generated music they believe infringes on artist rights
- The Google Lyria 3 lawsuit directly connects to this: if AI tools can cheaply generate infinite synthetic tracks, streaming revenue for human artists collapses
- Spotify's "minimum streams for royalties" threshold policy (introduced 2024) was explicitly designed to combat low-effort AI filler — but hasn't stopped the flood

**Community reaction:** Human musicians describe the situation as "the controversy sparked renewed debate about whether AI systems are learning from artists or exploiting them."

**Source:** Substream Magazine, Forbes — March 2026

---

### 🔴 Suno Download Paywall + Monthly Caps — Community Backlash

**What happened:** Following Suno's November 2025 settlement with Warner Music Group, the platform underwent a fundamental shift: **audio downloads now require payment** (previously free), and **monthly download caps** were introduced for all tiers. The December 2024 Reddit post "Suno puts a price on EVERY download. FREE AI music is DYING" went viral with strong upvote response. 

Key changes from the Warner deal:
- Free tier: music generation still possible, but downloads are restricted/paywalled
- Paid tiers: commercial use license included but subject to monthly download limits
- 2026 roadmap: existing models deprecated in favour of new models trained exclusively on **licensed music**
- Free downloads of rejected/experimental generations are being removed

**Community reaction:** The r/SunoAI thread "How many people are actually canceling their subscription?" accumulated significant engagement. Long-time power users who relied on downloading rejected takes and iterating in DAWs (like Ableton) are the most affected. The general mood: Suno is transitioning from "open lab" to "licensed content platform" — acceptable to some, a betrayal to others.

**Suno's position:** CEO Mikey Shulman framed the changes positively — rolling out "more robust features" and "opportunities to collaborate with talented musicians." The platform hit **2 million paid subscribers** as of February 26, 2026, suggesting the changes haven't killed adoption. But user sentiment in communities is clearly negative.

**Source:** Reddit r/SunoAI (multiple threads), Digital Music News, Forbes — November 2025–February 2026

---

### 🟠 Udio Copyright Lawsuit — Still Active, No Settlement

**What happened:** The RIAA filed copyright suits against both Suno and Udio in June 2024, alleging mass infringement of copyrighted sound recordings. While Suno settled with Warner (November 2025) and began licensing negotiations with other labels, **Udio has not publicly announced any settlement**. The lawsuit documents Udio producing outputs that "strongly resemble copyrighted recordings" when prompted with artist/era/genre combinations — including songs similar to ABBA and Jason Derulo tracks.

**Stakes:** The RIAA sought up to **$150,000 per infringed work** — representing potentially billions of dollars in liability given the scale of training data used.

**Where things stand:** Udio continues operating; the lawsuit is ongoing through the courts. The unresolved status puts Udio in a legally precarious position compared to Suno, which secured at least a partial settlement and licensing framework.

**Source:** RIAA, The Guardian, Reuters, Music Business Worldwide — June 2024–ongoing

---

### 🟠 Suno 2026 Model — Transition to Licensed-Only Training

**What happened:** Suno's updated Rights & Ownership documentation (December 2025) outlined a fundamental pivot: the 2026 model will be **trained exclusively on licensed music**, moving away from the pre-licensing approach that caused the RIAA lawsuits. Current users are warned that existing models "may be deprecated."

**Why this matters:** The new model will be fundamentally different in character. Music trained only on licensed catalogs will reflect those catalogs' biases and gaps. The organic diversity of styles that made Suno's original model interesting came partly from training on the full breadth of human music production — including copyrighted work.

**Community reaction:** Mixed. Some welcome the ethical clarity; others see it as a dilution of capability. The download caps are universally unpopular.

**Source:** Digital Music News, lilys.ai — December 2025–February 2026

---

### 🟡 Industry Backlash vs. Growing User Base

**What happened:** The contradiction at the heart of AI music in 2026: Suno hit 2 million paid subscribers (100 million total users) by February 2026 — clear product-market fit with consumers. Simultaneously, the music industry's hostility is intensifying, not decreasing.

**The tension:** Human musicians see AI music tools as existential threats that devalue their work and flood streaming platforms with synthetic content. The Warner deal was widely criticised by artists as label executives cutting their own deal at musicians' expense.

**Source:** Forbes — February 26, 2026
