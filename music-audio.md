# music-audio — AI Issues Radar

_Last updated: 2026-03-19_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 1 | 🔴 Critical | Google sued by indie musicians over Lyria 3 — "vertically-integrated syndicate" that illegally copies music, launders ownership, unfairly competes | Google Lyria 3 | Active (filed March 6, 2026) |
| 2 | 🔴 Critical | GEMA v. Suno — German court heard landmark copyright case March 9; ruling scheduled June 12, 2026; Hamburg court reached opposite conclusion same paragraph | Suno | Active (ruling due June 12) |
| 2a | 🔴 Critical | Suno indie artist class action oral arguments TOMORROW (March 20) — could set precedent for independent artists' standing to sue; Suno still has no API and credits expire monthly post-Warner deal | Suno | IMMINENT — oral args March 20, 2026 |
| 3 | 🔴 Critical | Suno enforces paid-only downloads + monthly download caps as part of Warner Music deal — community furious at monetisation pivot | Suno | Active |
| 4 | 🟠 Major | Udio settles with Warner, Universal, Merlin — "walled garden" model imposed; indie artists excluded from restitution | Udio | Resolved for majors / Active for indie artists |
| 5 | 🟠 Major | EU Parliament votes 460–71 for mandatory AI copyright disclosure + fair remuneration for all training data — industry-wide threat | Industry-wide | Developing (March 10, 2026) |
| 6 | 🟠 Major | AI musicians flooding Spotify — major labels pushing back as synthetic content devalues platform | Multiple | Developing |
| 7 | 🟠 Major | Suno "2026 model" will replace existing version with licensed-only training data — old-style open generation ending | Suno | Developing |
| 8 | 🟡 Notable | "Starting fresh" playbook exposed — labels and AI companies doing deals that leave independent artists without recourse | Suno, Udio | Ongoing |
| 9 | 🟡 Notable | Industry backlash grows even as Suno hits 2M paid subscribers — human musicians deeply hostile | Suno, Udio | Ongoing |

---

## Details

### 🟠 Udio Settles With Warner, Universal & Merlin — "Walled Garden" Controversy — March 2026

**What happened:** Udio — the RIAA's other major defendant alongside Suno in the landmark 2024 copyright suits — has reached settlements with **Warner Music Group, Universal Music Group, and Merlin** (the global digital rights agency for independent labels). The deals mirror the Suno/WMG framework: labels withdraw their specific suit, Udio agrees to operate a "walled garden" model going forward.

**The "walled garden" model explained:** Users can create music inside the Udio platform, experiment with AI generation, and share tracks within the ecosystem — but **cannot export AI-generated music off the platform** for commercial use outside its controlled environment. The structure was designed by the major labels to prevent AI music from freely entering streaming platforms and competing with signed artists.

**The fundamental problem — who isn't in the room:**

Music Business Worldwide op-ed attorney Krystle Delgado (leading class action lawsuits against Suno and Udio for indie artists) published a withering critique titled "The Problem with AI Companies 'Starting Fresh'" (MBW, March 12, 2026). Key argument:
- The conversation has shifted from "they stole music illegally" to "let's all make money together"
- **But "a large portion of these songs belong to independent artists, who were never asked for permission, offered compensation, or are even being included in the 'let's start fresh' AI campaigns today"**
- Major labels cut deals for their catalogues at the expense of the millions of independent artists whose work was also in the training data
- Whether indie artists can get justice through pending class action lawsuits (indieailawsuit.com) "remains to be seen"

**Why this is a bigger issue than it looks:** The settlement structure allows Warner, Universal, and Merlin to claim moral authority ("we protected rights") while:
1. Effectively granting Udio a licence to have already used the music
2. Receiving a share of future AI music revenue
3. Leaving independent artists — who have fewer legal resources — to fight separately

**RIAA position:** The RIAA's original suit (June 2024, seeking $150,000 per infringed work) is now effectively resolved for the major label plaintiffs. The indie artist class action is an entirely separate legal track.

**Source:** Music Business Worldwide, Medium, YouTube (Top Music Attorney), indieailawsuit.com — March 12, 2026

---

### 🟠 EU Parliament Votes 460–71 for AI Copyright Legislation — March 10, 2026

**What happened:** The European Parliament adopted a landmark resolution on "Copyright and Generative Artificial Intelligence – Opportunities and Challenges" with an overwhelming majority: **460 votes in favour, 71 against, 88 abstentions**.

**What the resolution demands:**
- Full mandatory **disclosure of all copyrighted works used to train AI models** — with automatic copyright infringement proceedings against parties that fail to be completely transparent
- **Fair remuneration** for rights holders whose works were used in training
- Extension of EU copyright directive to all generative AI systems on the EU market, **regardless of where they were trained** (directly targeting US-trained models like Suno, Udio, Google Lyria)
- Protection of Europe's creative sector, which generates ~7% of EU GDP

**Why this threatens every major AI music tool:** The "regardless of where trained" clause means US-based AI music tools that were trained on European-copyrighted music without disclosure would face EU infringement proceedings when operating in EU markets — a de facto global disclosure requirement for any tool with European users.

**Industry reaction:** EU creative sector groups (FIM, GESAC, IMRO) celebrated. European tech associations pushed back, arguing the regulation could harm innovation. Billboard and Deadline covered it prominently as a major development in the global AI copyright war.

**Next steps:** The resolution is non-binding but calls on the European Commission to initiate a formal legislative proposal — which would become binding EU law.

**Source:** Billboard, Euronews, EU News, GESAC, FIM, IMRO, Deadline — March 10, 2026

---

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

### 🔴 Suno Indie Artist Class Action — Oral Hearing MARCH 20, 2026 (2 DAYS AWAY)

**What happened:** The independent artist class action lawsuit against Suno (tracked at indieailawsuit.com) has its **oral arguments hearing scheduled for March 20, 2026** — in just two days. This is a critical procedural moment: the court will hear arguments on Suno's motion to dismiss.

**What's at stake:** Suno has argued that the indie artist plaintiffs lack standing and that the claims should be dismissed. The plaintiffs — represented by attorney Krystle Delgado and the Loevy + Loevy law firm — argue that:
- Suno trained on copyrighted music by independent artists without consent or compensation
- The WMG/Suno settlement explicitly excluded independent artists from any remedy
- Independent artists have a direct legal claim separate from the major labels

**Why this matters for the broader AI music industry:**
- If the court dismisses: Suno effectively walks away from obligations to independent artists entirely, even after the WMG deal
- If the court allows the case to proceed: Every AI music tool that trained on non-licensed music faces potential class action liability to millions of independent artists whose music was scraped

**Krystle Delgado's central argument (MBW op-ed, March 12):** The AI companies are running a "launch, train, settle" playbook — training on stolen music, then cutting deals with the majors while leaving independent artists without recourse. "Whether indie artists can get justice through pending class action lawsuits remains to be seen" — the March 20 hearing is the first major test.

**Source:** indieailawsuit.com, Music Business Worldwide, Medium (GEMA v. AI Titans) — March 2026

---

### 🟠 AI Musicians Flooding Spotify — Bot Crackdown, Papaoutai Controversy — March 2026

**What happened:** AI-generated music is flooding Spotify at a scale that is visibly impacting the platform and triggering multiple crackdowns. Key developments this week:

**Spotify bot stream crackdown (March 2026):** Several artists recently saw **millions of their streams disappear** after Spotify launched a major crackdown on artificial streaming. Spotify defines "artificial streams" as plays that do not reflect real listener intent — a category that includes bot-driven streaming of AI-generated filler tracks. The mass deletion caught some legitimate artists in the net alongside bad actors.

**The "Papaoutai" AI cover controversy:** A viral incident this week involved an AI-generated cover of Stromae's "Papaoutai" that spread widely without disclosure. The University of Melbourne's The Conversation (March 10, 2026) explored the crisis of AI music passing as human: "While Bandcamp has taken a clear anti-AI stance and works to keep AI-generated music off the platform entirely, other platforms like Spotify have gestured towards governance changes but largely allowed AI music to rack up streams without clearly disclosing the use of AI."

**AI artists thriving on Spotify's algorithms (Reddit r/Fauxmoi, March 12):** A viral thread documented AI "artists" systematically gaming Spotify's recommendation algorithms — generating music in bulk optimised for algorithm signals rather than human listenability, then harvesting royalty pool share.

**The structural problem:**
- Spotify's royalty pool is being diluted by high volumes of synthetic content
- Major record labels are beginning to formally push back against AI-generated music
- Spotify's "minimum streams for royalties" threshold policy (2024) was designed to combat low-effort AI filler — but it hasn't stopped the flood
- The Google Lyria 3 lawsuit directly connects to this: if AI tools generate infinite synthetic tracks, human artist streaming revenue collapses

**Community reaction:** Music fans are demanding Spotify flag AI-generated music recommendations. TechRadar headline (this week): "Music fans are demanding Spotify flags AI-generated music recommendations." The r/Fauxmoi summary: "AI artists thrive on Spotify's algorithms as the platform gets more expensive and the CEO pours money into military technology."

**Source:** Substream Magazine, Forbes, The Conversation, TechRadar, Reddit r/Fauxmoi, nomusica.com — March 2026

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

### 🟠 Udio Copyright Lawsuit — Settled with Major Labels, Indie Artists Still Pursuing Action

**What happened:** The RIAA filed copyright suits against both Suno and Udio in June 2024, alleging mass infringement of copyrighted sound recordings. The lawsuit documented Udio producing outputs that "strongly resemble copyrighted recordings" when prompted with artist/era/genre combinations — including songs similar to ABBA and Jason Derulo tracks.

**Update (March 2026):** Udio has now settled with Warner Music Group, Universal Music Group, and Merlin through a "walled garden" licensing structure (see section above). The major label cases are effectively resolved. However, a separate **indie artist class action** (indieailawsuit.com, led by attorney Krystle Delgado) continues.

**What independent artists face:** Unlike major labels, indie artists can't negotiate settlement terms directly. Their compensation, if any, will be determined by class action outcomes — which could take years and may result in minimal per-artist payments even if they succeed.

**Source:** RIAA, Music Business Worldwide, indieailawsuit.com — June 2024–March 2026

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

---

### 🔴 Suno Motion to Dismiss — Oral Arguments Scheduled March 20, 2026

**What happened:** In the ongoing major label copyright lawsuit against Suno, oral arguments on Suno's motion to dismiss have been **scheduled for March 20, 2026** — three days from today. This is a pivotal procedural moment in the case:

**What's at stake (per jam.com, March 2026):**
- The hearing will address whether independent artists whose work was used to train Suno's model without permission have **standing to sue** and what damages they can recover
- Labels are seeking **statutory damages of up to $150,000 per infringed work**
- Suno's model is alleged to sometimes produce outputs that "closely replicate existing songs"

**Three-front legal exposure for AI music as of March 17, 2026:**
1. **Labels v. Suno** — Oral arguments March 20, motion to dismiss pending
2. **GEMA v. Suno** — German court hearing; ruling expected June 2026
3. **Labels v. Google (Lyria 3)** — Filed March 6, 2026; indie musicians suing over YouTube training data scraping

**The "starting fresh" pattern:** Legal analysis documents how Suno attempted to restart with "licensed-only training data" for future model versions while arguing old claims are moot. Courts are being asked to determine whether this "clean slate" strategy absolves prior infringement — a question with enormous implications for the entire industry.

**Source:** jam.com, terms.law, Reuters AI copyright roundup — March 16–17, 2026
