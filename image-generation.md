# image-generation — AI Issues Radar

_Last updated: 2026-03-31_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 0mar31a | 🟠 Major | **Midjourney V8 hidden restrictions silently distort user prompts** — HalfJourney Lab / Medium (March 29): V8 Alpha introduces improved prompt adherence but enforces **hidden guardrails that silently alter image outputs without informing the user** — prompts accepted but quietly modified by undisclosed content filters; artists cannot tell if poor output is their fault or invisible censorship; Geeky Gadgets (March 25): some creators switching back to V7 due to V8 aesthetic regressions; Midjourney's zero adult content policy remains absolute — insta-blocked, no loopholes; V8.1 planned to address quality complaints | Midjourney V8 Alpha | Active (March 2026) |
| 0mar31b | 🔴 Critical | **Senator formally demands MidJourney, ElevenLabs, Synthesia crack down on political deepfakes before midterms** — biometricupdate.com (March 26): Virginia senator sent formal letters to MidJourney, OpenAI, Anthropic, xAI, Meta, Adobe, ElevenLabs, Cohere, Microsoft, Synthesia, Canva, Google, Snap, TikTok US, Bluesky, Pinterest, Reddit demanding deepfake crackdown; Reuters (March 28): AI deepfake political ads already live in 2026 midterm campaigns — Democratic Texas Rep. James Talarico'''s likeness cloned without consent; no federal law restricts AI political messaging; image platforms have zero legal obligation to prevent political deepfake misuse | MidJourney / AI image tools (misused) | **Active** (March 26–28, 2026) |
| 0mar29 | 🔴 Critical | **Iran war deepfake images flood social media — 110+ unique AI-generated fakes identified, "feel true" even when audiences know they're fake** — NYT (March 28): identified 110+ unique deepfakes conveying pro-Iran messages (battlefield images, missile strikes, fake soldiers); Guardian (March 28): deepfakes "shape emotional responses and beliefs even when audience is explicitly told they're fake"; FDD (March 19): both US/Israel and Iran sides weaponising AI-generated images; no AI image platform has restricted warzone propaganda use; Grok already documented generating fake Iran war images and wrongly verifying them as real | Grok / xAI + generative AI tools (misused) | **Active** (March 28–29, 2026) |
| 0mar28 | 🟠 Major | **Grok mass login failure — thousands abruptly logged out (March 26)** — thousands of X users lost Grok access when authentication errors hit the platform March 26; users experienced "repeated authentication errors" after being logged out without warning; no official explanation from xAI; incident comes as Grok faces CSAM lawsuits, Baltimore municipal suit, and 6,700 deepfakes/hour findings — the platform's image generation safety crisis continues to compound | Grok / xAI | Resolved (March 26, 2026) |
| 0mar27 | 🔴 Critical | **Gemini image generation API down TODAY** — gemini-3-pro-image-preview ("Nano Banana Pro") and Nano Banana 2 image APIs experiencing major outage; massive request failure rates; developers report persistent 429 errors on Gemini CLI for 2+ days; apiyi.com confirms active failure (March 27, 2026) | Google Gemini image generation | **Active TODAY** (March 27, 2026) |
| 0NEW | 🔴 Critical | **Baltimore becomes first US city to sue xAI** over Grok deepfake porn (March 24, 2026) — municipal lawsuit alleges Grok AI enabled widespread creation of harmful deepfakes including images of minors; this follows the Tennessee CSAM class action (March 16) and women/girls lawsuit (March 17); legal pressure mounting from all sides | Grok / xAI | Active (filed March 24, 2026) |
| 1 | 🔴 Critical | xAI/Grok CSAM class action — three Tennessee teenagers sue xAI alleging Grok used their real photos to generate + distribute child sexual abuse material; deepfake images uploaded to Discord (filed March 16, 2026) | Grok / xAI | Active (filed March 16, 2026) |
| 1a | 🔴 Critical | Women and girls lawsuit vs Grok — separate lawsuits by adult women AND underage girls over sexualised AI deepfakes; on Jan 14 Musk promised a fix; two of three lawsuits allege CSAM was generated before that fix date (19th News, March 20, 2026) | Grok / xAI | Active (filed March 17–20, 2026) |
| 2 | 🔴 Critical | Grok generates + wrongly verifies fake Iran war images as real — spreading misinformation at scale during active conflict | Grok / xAI | Active |
| 3 | 🔴 Critical | Grok users generating 6,700 sexualised/nudified images per hour — 84x more than top 5 deepfake sites combined; Australian regulator says CSAM "systemic" on X | Grok / xAI | Active |
| 3a | 🔴 Critical | EU Parliament backs outright ban on AI nudify/deepfake apps (460–71) — triggered by Grok backlash; EC previously admitted AI Act had gaps on CSAM and nonconsensual deepfakes; new Ars Technica analysis: Musk's "blame users" tactic may be foiled by incoming EU law | Grok / xAI (trigger), Industry-wide (scope) | Developing (March 13–19, 2026) |
| 4 | 🟠 Major | Disney/Lucasfilm/Marvel sues Midjourney for copyright infringement — "unlawfully copied" Star Wars, Marvel assets to train model | Midjourney | Active |
| 5 | 🟠 Major | EU Parliament votes 460–71 to mandate disclosure of all training images + fair remuneration — affects every image model deployed in EU | Industry-wide | Developing (March 10, 2026) |
| 6 | 🟠 Major | US Supreme Court declines Thaler case — AI-generated art cannot receive copyright; human authorship required | Industry-wide | Resolved (Mar 2026) |
| 7 | 🟠 Major | Midjourney v7 consumes 2x GPU credits vs v6 — CEO admits team "profoundly unsatisfied" with the release | Midjourney | Ongoing |
| 8 | 🟠 Major | Andersen v. Stability AI — landmark copyright case still progressing; artists secured key win, unjust enrichment claims dismissed but copyright claims survive | Stability AI | Active |
| 9 | 🟡 Notable | DALL-E most expensive per-image at scale, least customisable; losing ground to open-source alternatives | DALL-E (OpenAI) | Ongoing |
| 10 | 🟡 Notable | Stable Diffusion base models require significant fine-tuning to match Midjourney/DALL-E quality out of the box | Stable Diffusion | Ongoing |
| 11 | 🟠 Major | US Copyright Court signals legal shifts for Midjourney — 2026 rulings emphasising fair use only for lawfully-obtained training data; pirated datasets explicitly rejected; The Atlantic: 19 AI copyright lawsuits active | Midjourney, Stability AI | Active (March 2026) |
| 12 | 🟡 Notable | UK government partially backtracks on AI copyright TDM exception — hasn't fully ruled out unlicensed training data access; creative industry on high alert (BBC, March 2026) | Industry-wide (UK) | Developing |

---

## Details

### 🔴 Baltimore Sues xAI — First US City to Sue Over Grok Deepfake Porn — March 24, 2026

**What happened:** On March 24, 2026, the **Mayor and City Council of Baltimore** filed a groundbreaking municipal lawsuit against xAI and X, making Baltimore the **first US city to sue over AI-generated deepfake pornography**. The lawsuit alleges Grok enabled widespread creation of harmful deepfake content, including images involving minors.

**The accumulating legal front against Grok:**
This suit is the latest in an accelerating wave of Grok-related deepfake litigation:
1. **March 16, 2026:** Three Tennessee teenagers file class-action — allege Grok generated CSAM (child sexual abuse material) from their real photos; images found on Discord
2. **March 17–20, 2026:** Women and girls file separate lawsuits over sexualised deepfakes; two of three cases allege CSAM was generated *before* Musk's January 14 "fix" announcement
3. **March 24, 2026:** Baltimore (first municipality) files suit
4. **Wikipedia now has a dedicated article:** "Grok sexual deepfake scandal" — documenting the scale of the crisis

**The background:**
- By late December 2025, users were using Grok to edit photos of real women into sexualised poses — with the chatbot posting the graphic images publicly on X
- Grok was generating an estimated 6,700 sexualised/nudified images per hour at peak — 84x more than the top 5 dedicated deepfake sites combined
- Australian regulator found CSAM was "systemic" on X
- When Musk claimed to have fixed the issue on January 14, lawsuits allege the CSAM generation had already occurred and victims had already been harmed

**Why the municipal lawsuit matters:** City governments suing AI companies over deepfakes introduces a new legal enforcement vector. Baltimore's suit provides city prosecutors direct standing to seek injunctions and damages. This model could be replicated by other cities.

**Sources:** CNBC (March 24), 19th News (March 20), DicelloLevitt, Wikipedia, Breitbart — March 2026

---

### 🔴 Grok Generates & Wrongly Verifies Fake Iran War Images — March 2026

**What happened:** During the Iran conflict coverage (March 2026), X's Grok AI chatbot became a misinformation amplifier on two fronts:

1. **Generating fakes:** Grok was producing its own AI-generated images about the Iran war and publishing them on X
2. **Falsely verifying fakes:** When users submitted AI-generated images or videos asking Grok to verify whether they were real, Grok "repeatedly and confidently published misleading or false information" — telling users that AI-fabricated content was authentic footage

**The Musk irony:** This occurred after Elon Musk had explicitly positioned Grok as X's fact-checking AI tool. The BBC's verification team (BBC Verify) documented multiple cases where "Grok wrongly insisted that the AI-generated video was real."

**Scale of impact:** Millions of X users relying on Grok for fact-checking during an active military conflict received confidently wrong information. The Guardian (March 13, 2026) described the spread of AI-generated Iran war images as reaching critical mass, with Grok actively contributing to rather than solving the problem.

**Regulatory context:** France has already raided X's Paris offices (February 2026) over Holocaust denial and sexual deepfakes generated by Grok. Multiple governments (Indonesia, Malaysia, Philippines) have temporarily blocked X over Grok content. California's AG is investigating xAI for state law violations.

**Source:** WIRED, CNN, BBC, Guardian, RTE, The Transhumanist — March 10–13, 2026

---

### 🔴 Grok Generating 6,700 Sexualised/Nudified Images Per Hour — January 2026

**What happened:** A 24-hour analysis (January 5–6, 2026) found that Grok users were generating **6,700 sexually suggestive or nudified images per hour** — **84x more than the top 5 deepfake websites combined**. WIRED reported that even more graphic content was being generated beyond what was captured in that analysis.

**Why this matters for image generation:** Grok's image generation (powered by Aurora) operates with significantly weaker content filters than competitors. This isn't just an ethical issue — it demonstrates that image generation guardrails are inconsistently applied across the industry, and that when they're absent, harm scales instantly and massively.

**Source:** Wikipedia (AI Controversies), WIRED — January 2026

---

### 🟠 EU Parliament Votes 460–71 for AI Image Training Disclosure — March 10, 2026

**What happened:** The European Parliament voted overwhelmingly (460–71, 88 abstentions) on March 10, 2026 to adopt the "Voss Report" — a resolution calling on the European Commission to legislate mandatory:
- **Full disclosure of all copyrighted images used to train AI models** (with automatic infringement proceedings for non-compliance)
- **Fair remuneration** for rights holders whose images were used in training
- Extension to ALL generative AI systems on the EU market **regardless of where they were trained**

**Impact on image generation tools:** Every major image generation model (Midjourney, Stable Diffusion, DALL-E, Adobe Firefly, Flux, Grok's Aurora) trained on scraped web images would face EU compliance requirements. Midjourney's notorious refusal to disclose training data would become illegal in EU markets. The "regardless of where trained" clause is designed specifically to close the "trained in the US, deployed in Europe" loophole.

**Industry split:** EU creative organisations (GESAC, IMRO) celebrated. European tech associations (representing AI startups) warned it could harm innovation. The resolution is non-binding but constitutes strong political direction — binding legislation expected to follow.

**Source:** Billboard, Euronews, GESAC, IMRO, Deadline — March 10, 2026

---

### 🟠 US Supreme Court Declines Thaler AI Copyright Case — March 2026

**What happened:** The US Supreme Court declined to hear Dr. Stephen Thaler's appeal seeking copyright protection for his AI-generated artwork "A Recent Entrance to Paradise." The refusal means lower court decisions stand: **AI-generated art cannot receive copyright protection in the US** because it lacks human authorship.

**Why this matters:** The ruling definitively closes the door on AI tools receiving copyright for their outputs — which affects every commercial image generation tool that promises users exclusive ownership of generated content. Key implications:
- AI-generated images are effectively in the public domain (anyone can copy them)
- Commercial tools marketing "copyright ownership" of AI outputs to users are in a grey area
- Human artists' rights advocates claim a victory — AI cannot displace them as copyright holders

**Parallel development:** State laws requiring AI content disclosure (e.g. labelling AI-edited real-estate photos) are multiplying, suggesting a legislative trend toward disclosure requirements even absent copyright protection.

**Source:** Wikipedia (AI Visual Art), LAT, gadgetsgigabytesandgoodwill.com — March 2026

---

### 🟠 Midjourney v7 — High Cost, Quality Concerns, CEO Dissatisfaction

**What happened:** Midjourney v7 consumes **2x the GPU time** compared to v6. Video generation costs even more — users report it costs **8x a standard fast generation**. The credit drain is so aggressive that multiple users report burning through an entire month's allocation within days of using video features. Internally, Midjourney CEO David Holz reportedly admitted the team was "profoundly unsatisfied" with v7's quality — suggesting it was released before the team was happy with it.

**Community reaction:** Reddit posts like "I already regret subscribing to Midjourney for a year" reflect broader disappointment. Long-term users describe v7 images as lacking the "soul" that made earlier versions beloved — "beautiful and breathtaking" has given way to images that feel "generic and ugly" to loyal users. The dominant workflow workaround is now to generate with v7, then pass images into Photoshop, Fal Kontext, or Kling for further refinement — defeating the "one tool" promise.

**Context:** The 2026 competitive landscape is brutal. Flux 2, Imagen 4, and others have closed the quality gap significantly, removing Midjourney's historical quality moat. The shift to Discord-only access remains a persistent friction point compared to web-native competitors.

**Source:** r/midjourney (multiple threads), gradually.ai — 2025–2026

---

### 🟠 Andersen v. Stability AI — Copyright Battle Continues

**What happened:** The landmark copyright case brought by artist Sarah Andersen and others against Stability AI is progressing through the Northern District of California. While claims of **unjust enrichment and breach of contract were dismissed**, U.S. District Judge William Orrick **denied Stability AI's motion to dismiss the core copyright infringement claims** in an August 2024 ruling. The case continues into 2026, with artists surviving the most important legal hurdle.

**Who's affected:** The case has industry-wide implications. If artists win, every major image generation model trained on scraped data faces liability. Stability AI's ability to fund a prolonged legal battle against well-resourced plaintiff attorneys is also under pressure.

**Scale:** This is the test case for the entire AI image generation industry's legal foundation. Dozens of similar cases cite Andersen as a precedent.

**Community reaction:** Artists' communities remain deeply mobilised. The "Fairly Trained" certification movement (founded by former AI exec Ed Newton-Rex) is gaining traction as an alternative to models trained on scraped data.

**Source:** NYU JIPEL (jipel.law.nyu.edu), blankrome.com — ongoing

---

### 🟡 DALL-E — Most Expensive, Least Flexible at Scale

**What happened:** DALL-E (via OpenAI API or ChatGPT) is consistently rated the most expensive per-image option at production scale. It lacks the stylistic range of Midjourney and cannot be self-hosted, making it unsuitable for cost-sensitive or privacy-sensitive workloads. Despite deep integration with ChatGPT, its customisation limitations are widely criticised.

**Source:** dev.to, starryai.com, aiwiner.com — 2025–2026

---

### 🟡 Stable Diffusion — Quality Gap Without Fine-tuning

**What happened:** Stable Diffusion 3.5, while open-source, requires significant fine-tuning or careful prompt engineering to match Midjourney or DALL-E quality out of the box. The open-source advantage (self-hosting, privacy, cost) comes with a steep expertise requirement that excludes casual users and increases production complexity for teams without ML engineers.

**Source:** lovart.ai, dev.to — 2025–2026

---

### 🔴 xAI / Grok CSAM Class Action — Tennessee Teenagers — March 16, 2026 (NEW)

**What happened:** Three teenage girls from Tennessee filed a class action lawsuit in California federal court on **March 16, 2026**, against xAI — Elon Musk's AI company and maker of the Grok chatbot. The case is now being reported by NPR, Washington Post, The Guardian, Engadget, and Digital Watch Observatory.

**Core allegations:**
- xAI's Grok AI model powered a third-party app that generated **nonconsensual, sexually explicit images and videos** of the plaintiffs, taken when they were minors
- Incidents occurred between **mid-2025 and early 2026**
- Real photographs of the plaintiffs were altered into CSAM and circulated online without their knowledge
- The lawsuit explicitly accuses xAI of "distributing, possessing and producing with intent to distribute child pornography"
- Filed as a class action, potentially representing hundreds or thousands of additional victims

**Legal specifics:** The complaint was filed in US federal court in California. Three plaintiffs are named, two of whom are still minors at the time of filing.

**Australian dimension:** Australia's eSafety Commissioner was separately warned on March 17, 2026, that CSAM is "systemic" on Musk's X platform — adding international regulatory pressure on top of the US civil lawsuit.

**Context — pre-existing Grok CSAM problem:** This lawsuit follows months of documented evidence that Grok was generating sexualised/nudified images at a rate of **6,700 per hour** — 84x more than the top 5 dedicated deepfake sites combined. Multiple prior studies identified Grok as the most prolific generator of nonconsensual nude images of any AI platform. The teenagers' lawsuit represents the first time victims have directly sued xAI.

**Why it matters:** This case could establish whether AI companies are liable for downstream harms when their models are used via third-party apps to generate illegal content. The class action scope means damages could be enormous if certified.

**Source:** NPR, Washington Post, The Guardian, Engadget, Digital Watch Observatory, The Guardian (Australia) — March 16–17, 2026

---

### 🔴 EU Parliament Backs Ban on AI Nudify Apps — Triggered by Grok Backlash — March 13–19, 2026

**What happened:** The European Parliament voted **460 to 71** to back a new law banning AI tools that generate sexualised deepfakes — including "nudification apps" — as a direct response to the Grok controversy. The vote came after the European Commission had previously acknowledged that **the existing EU AI Act does not prohibit AI systems that generate CSAM or sexually explicit deepfake nudes** — a gap that Elon Musk's platform had exploited (or at minimum enabled at scale).

**Key details:**
- Irish MEP **Michael McNamara** (leading the AI file) said the ban aimed to stamp out "nudification apps without consent, which have caused much pain for the profit of some" — explicitly naming the type of tool Grok had made mainstream
- The vote comes after Grok is estimated to have generated ~**3 million sexualised images** (including ~23,000 of apparent children) during the December–January window when its safety filters were effectively non-functional
- The European Commission's admission that the AI Act had a **gap on CSAM** created urgency — the new rules close that gap
- A fresh Ars Technica analysis (March 19) argues that Musk's defensive strategy of "blaming users" for Grok's outputs may be "foiled" by the incoming EU regulation, which assigns liability to the AI provider, not just the end user

**Regulatory timeline:** This is a Parliament vote (backing, not final enactment). The ban still needs formal Council adoption. However, the 460–71 majority and the political urgency signal it will pass. Companies operating "nudify" products in the EU — or providing AI infrastructure used for such tools — face a hard deadline.

**Broader impact:** This is the first major post-AI-Act legislative action in Europe targeting a specific AI use case. The signal: regulators are moving much faster to patch AI Act gaps than originally anticipated. Any AI image generation tool operating in the EU — or whose API is used in EU-accessible apps — must now actively model the compliance risk.

**Source:** Ars Technica, France 24, Digital Journal — March 13–19, 2026

---

### 🟠 Disney / Lucasfilm / Marvel Sues Midjourney — Copyright Infringement — March 2026

**What happened:** Disney and its subsidiaries — including Lucasfilm and Marvel — filed a lawsuit alleging that **Midjourney unlawfully copied their copyrighted works** to train its AI image-generation service, and continues to infringe those rights in its outputs.

**Specific claims (per Lexology, March 2026):**
- Star Wars characters, Marvel characters, and Disney IP are recognisable in Midjourney outputs
- The training dataset included copyrighted Disney assets without permission
- Ongoing infringement in the model's ability to generate derivative content on demand

**Significance:** Disney is the most powerful IP owner in the entertainment industry. Its entry into AI copyright litigation signals that major studios are no longer waiting to see how artist-filed cases resolve — they're bringing their own suits directly. This will generate substantially higher damages exposure for Midjourney than any individual artist case.

**Source:** Lexology AI in Litigation series, Reuters AI copyright roundup — March 2026

---

### 🟠 US Copyright Courts Signal Shift: Fair Use Only for Lawfully-Obtained Training Data — March 2026

**What happened:** A comprehensive analysis by legal commentator Yuyjo.com (March 2026) documents the emerging trend in 2026 US copyright rulings: courts are beginning to **accept fair use arguments for AI image models only when training data was lawfully obtained** — and are explicitly rejecting fair use protections for pirated or improperly scraped datasets.

**Key development:**
- A US Copyright Court review indicated that fair use standards are "emerging" for AI systems that trained on properly licensed or public domain works
- Courts are treating models that used pirated datasets differently from those that used lawfully-obtained data — creating a legal incentive for proper training data hygiene going forward
- The Atlantic's reporting (March 20, 2026) documents that **19 active copyright lawsuits** against AI companies are pending, many related to image generation

**Who this affects:**
- **Midjourney**: Currently defending against Disney/Lucasfilm/Marvel suit; training data legitimacy is central
- **Stability AI**: Getty Images lawsuit (filed 2023, still active in early 2026) + Andersen class action
- **Runway**: Andersen class action includes Runway among defendants
- Any image model with unclear training data provenance

**The Andersen v. Stability AI update:** Artists Sarah Andersen, Kelly McKernan, and Karla Ortiz secured a significant legal win — their copyright infringement claims survived a motion to dismiss and are progressing to discovery. Unjust enrichment claims were dismissed, but the core IP case continues.

**Source:** Yuyjo.com, Reuters AI Copyright Roundup, The Atlantic — March 16–20, 2026

---

### 🟡 UK AI Copyright Exception: Partial Backtrack — Creative Industry Remains on Alert — March 2026

**What happened:** The UK government has walked back (but not fully abandoned) a proposed text-and-data mining (TDM) exception that would have allowed AI companies to train on any copyrighted work, including images, without a licence or payment.

**What happened:** After sustained pressure from the UK creative industry — photographers, illustrators, designers, visual artists, and major image agencies — the government has signalled it will not proceed with the most controversial form of the exception. However, Minister Chris Bryant made clear the option is "not entirely ruled out."

**The creative industry's concern:**
- Even a partial TDM exception would allow AI image companies to legally ingest stock photography, illustration databases, and commissioned artwork for training without compensation
- Getty Images, Shutterstock, and professional photographers' organisations all lobbied against the exception
- The UK is home to a significant creative economy that generates substantial export revenue

**Current status:** Ongoing consultation. The exception in its most harmful form appears to be off the table for now — but the creative sector is maintaining pressure to ensure permanent exclusion.

**Source:** BBC News, UK Government consultation documents — March 2026

---

### 🔴 Iran War AI Deepfake Propaganda — 110+ Fakes, "Feel True" Even When Audiences Know — March 28–29, 2026

**What happened:** The New York Times and Guardian documented the most extensive AI-generated propaganda campaign observed in active wartime. In the first weeks of the US/Israel-Iran war in 2026:

- NYT (March 28) identified **110+ unique AI-generated deepfake images** spreading pro-Iran messages — including fake battlefield scenes, missile strike depictions, and fake female Iranian soldiers posting "Habibi, come to Iran" recruitment content
- Guardian (March 28, "They feel true"): published new psychological research showing **deepfakes shape emotional responses and belief formation even when the audience is explicitly told the content is AI-generated** — the "feel true" effect persists despite disclaimer exposure
- FDD analysis (March 19): both sides in the conflict are weaponising AI-generated images — not just Iran but also pro-US/Israel accounts generating synthetic propaganda
- Foreign Policy (March 17): "a torrent of fake videos and images generated by artificial intelligence have overrun social networks during the first weeks of the war in Iran"

**Scale context:** 500,000 deepfakes shared online in 2023 → 8,000,000 in 2025 → active wartime tactical deployment in 2026. The Iran conflict represents the moment AI-generated image propaganda became **systematic military/political information warfare**.

**Platform accountability gap:** No AI image generation platform has meaningfully restricted warzone propaganda use. Grok is already documented (see entry #2 above) generating fake Iran war images and incorrectly verifying AI-generated fakes as real — actively amplifying misinformation rather than filtering it. The broader industry has no coordinated response.

**Why this matters:** The "feel true" psychological finding is particularly alarming — it means content moderation labels ("This may be AI-generated") are **insufficient** to neutralise the harm. The 110+ distinct fakes also suggest coordinated production rather than individual actors.

**Source:** NYT (March 28), The Guardian (March 28), FDD (March 19), Foreign Policy (March 17) — 2026

---

### 🟠 Midjourney V8 Hidden Restrictions Silently Distort User Prompts — March 29–31, 2026

**What happened:** A detailed Medium investigation by HalfJourney Lab (March 29) exposed a significant problem with Midjourney V8 Alpha: the model accepts prompts that it then **silently modifies** based on undisclosed content restrictions. Users receive an output that bears little resemblance to what they requested — but are given no indication that their prompt was altered or refused. The result looks like poor prompt engineering when it's actually hidden censorship.

**The specific problems documented:**
- Hidden guardrails distort outputs in unexpected ways without any error or warning
- Midjourney V8 enforces its zero adult content ban "as strictly as ever" — insta-blocked for anything "spicy"
- Artists building commercial workflows report outputs are unpredictable in ways that make professional use difficult
- Some professional users are switching **back to V7** due to aesthetic quality regressions in V8, particularly for stylised/artistic work

**Credit model frustration:** Midjourney remains strictly paywalled (April 2023 onwards) with no free tier. V8 Alpha's 5x faster processing speeds allow rapid credit consumption, and users report burning through monthly credits faster than ever when exploring or iterating.

**The V8.1 plan:** Midjourney developers have signalled a V8.1 update is planned specifically to address the image quality and prompt adherence complaints — confirming the issues are acknowledged internally.

**Sources:** HalfJourney Lab / Medium (March 29), aiexotic.com (March 2026), Geeky Gadgets (March 25), cometapi.com (2026)

---

### 🔴 Senator Demands MidJourney and 17 Other Platforms Block Political Deepfakes Before 2026 Midterms — March 26–28, 2026

**What happened:** A US Virginia senator sent formal letters to 18+ AI companies and social platforms — including MidJourney, OpenAI, Anthropic, xAI, Meta, Adobe, ElevenLabs, Cohere, Microsoft, Synthesia, Canva, Snap, Google, TikTok US, Bluesky, Pinterest, and Reddit — demanding they implement safeguards against AI-generated political deepfakes before the 2026 midterm elections.

**The documented harm:** Reuters (March 28) confirmed that AI deepfake political ads are already active in midterm campaigns. A video depicting Texas State Representative James Talarico was created using AI image and video generation, showing him apparently endorsing policies he opposes. The video circulated for days before Talarico became aware of it.

**The accountability gap for image tools:** No AI image generation platform — including Midjourney — has meaningful policies restricting the creation of realistic images of real politicians or public figures for political messaging. Users can generate photorealistic images of any public figure saying or doing things they never did. These then feed into deepfake video pipelines.

**No legal obligation:** With no federal AI political speech regulation, image platforms face **zero legal enforcement risk** for enabling political deepfake content creation. The senator's letter carries no legal mandate — only reputational pressure.

**Sources:** biometricupdate.com (March 26), Reuters (March 28), Economic Times (March 29)
