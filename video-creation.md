# video-creation — AI Issues Radar

_Last updated: 2026-03-31_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 0mar31 | 🟠 Major | **TechCrunch: "Sora'''s shutdown could be a reality check moment for AI video"** — TechCrunch (March 29): analysis argues Sora'''s sudden discontinuation signals broader questions about whether AI video tools can achieve sustainable business models; Mashable (March 31) confirms Disney CEO Bob Iger was still publicly touting the OpenAI partnership as recently as Feb 2026 — making the March exit even more shocking; the 3-year, $1B deal lasted only ~3 months of active deployment; question now: will Runway, Kling, and Hailuo face the same fundamental problem of high compute costs vs. insufficient commercial demand? | Sora (OpenAI) / AI video industry | Active analysis (March 29–31, 2026) |
| 0SHUTDOWN | 🔴 Critical | **SORA OFFICIALLY SHUT DOWN — DISNEY EXITS $1B DEAL** — OpenAI discontinues Sora app and API (March 24–25, 2026), just 15 months after launch; Disney exits the $1B partnership signed only 3 months ago; OpenAI pivoting to coding AI and robotics; no timeline given for preserving user content; creators who built businesses on Sora blindsided; Interesting Engineering: "OpenAI will discontinue Sora, as Disney exits a $1B deal and industry backlash over copyright intensifies" | Sora (OpenAI) | **DISCONTINUED** (March 24–25, 2026) |
| 0a | 🔴 Critical | Runway + NVIDIA demo real-time AI video generation (100ms time-to-first-frame) — experts warn this makes deepfake scam calls indistinguishable from reality; real-time AI avatar can react live to a victim on a video call (PetaPixel, March 23, 2026) | Runway AI / NVIDIA | Active — misuse risk (March 23, 2026) |
| 0b | 🟠 Major | Chinese AI video quality leap — Kuaishou's monetizable AI video raises global deepfake + copyright risks; Japan Times: "Chinese AI videos used to look fake. Now they look like money." (March 20, 2026) | Kuaishou / Chinese AI video tools | Active (March 20, 2026) |
| 1 | 🔴 Critical | US Senators Blackburn + Welch demand ByteDance "immediately shut down" Seedance 2.0 — "most glaring copyright infringement from ByteDance to date"; MPA CEO also demands immediate shutdown (March 17); ByteDance had already suspended global launch (March 14) after Disney, Paramount, Netflix & Warner Bros C&D letters | Seedance 2.0 (ByteDance) | **Senators demanding shutdown** (March 17, 2026) |
| 1b | 🔴 Critical | Warner Bros Discovery sues MiniMax/Hailuo AI — copyright infringement of "copyrighted characters and related works"; raises concerns about using Hailuo commercially; Kling now advised as "safer commercial choice" for client work | Hailuo AI / MiniMax | Active (February 2026) |
| 2 | 🔴 Critical | Runway AI class action — YouTuber David Gardner sues for scraping YouTube videos via DMCA circumvention | Runway AI | Active |
| 3 | 🔴 Critical | Sora 1 forcibly retired March 13 — all historical content deleted; Sora 2 plagued by "stuck at 99%" bugs, "under heavy load" errors, new accounts having generation disabled; free access killed — now fully shut down (see #0SHUTDOWN) | Sora (OpenAI) | **DISCONTINUED** |
| 4 | 🟠 Major | EU Parliament votes 460–71 to mandate training data disclosure + remuneration — directly targets video model training on YouTube/streaming | Industry-wide | Developing (March 10, 2026) |
| 5 | 🟠 Major | OpenAI "Cameo" feature on Sora blocked by court — trademark injunction issued amid Hollywood consent backlash | Sora (OpenAI) | Active |
| 6 | 🟠 Major | Runway: high costs, slow "relaxed" queues, weak prompt adherence, opaque moderation and account bans | Runway AI | Ongoing |
| 7 | 🟡 Notable | Pricing chaos across the space — tools range wildly and many creators still can't produce audio-native video | Multiple | Ongoing |
| 8 | 🟠 Major | Sora 2 API duration extension bug — API returns 400 errors for advertised 15/20-second durations; developers blocked after building integrations on announced specs | Sora 2 (OpenAI) | Active (March 2026) |

---

## Details

### 🔴 SORA OFFICIALLY SHUT DOWN — OpenAI Discontinues App and API — March 24–25, 2026

**What happened:** In a sudden announcement on March 24–25, 2026, OpenAI confirmed it is **permanently discontinuing the Sora app and its API** — just 15 months after Sora first launched publicly (December 2024). The announcement was made via a social media post after the Wall Street Journal broke the news.

**OpenAI's statement:** "To everyone who created with Sora, shared it, and built community around it: thank you. What you made with Sora mattered, and we know this news is disappointing. We're saying goodbye to the Sora app." The company said it would share "more soon on timelines for the app and API and details on preserving your work" — but no timeline was given.

**The strategic pivot:** According to BBC reporting, OpenAI told them it discontinued Sora "so that it can focus on other developments, such as robotics 'that will help people solve real-world, physical tasks.'" This represents a complete reversal of OpenAI's consumer AI creative tools strategy announced less than 18 months ago.

**Disney actively exits the $1 billion deal:** Just three months ago (December 2025), Disney invested $1 billion in OpenAI and signed a three-year deal to bring 200+ licensed Disney, Marvel, Pixar, and Star Wars characters to the Sora platform. Per Firstpost and Interesting Engineering (March 25, 2026), Disney is **actively exiting** the $1 billion partnership alongside the Sora shutdown — the deal was explicitly tied to the Sora product, which no longer exists. The financial implications of the exit (whether Disney's investment is refunded or redirected) have not been disclosed.

**Why Sora failed:**
- **High compute costs** — Sora's diffusion model required immense GPU resources; even at $20–200/month tiers, margins were unsustainable
- **Falling usage** — Runway, Kling 3.0, Veo 3, and Seedance offered comparable or superior output at lower prices
- **Deepfake backlash** — Sora was widely used for non-consensual deepfakes, putting OpenAI in an uncomfortable position
- **"AI slop" association** — Sora became associated with low-effort AI video content that saturated social media
- **Lack of focus** — As Ars Technica noted, OpenAI all-hands meetings revealed executives said they were "distracted by side quests"; Sora was named as one of them
- **No free tier** — Killed organic growth; competitors offered free credits to build communities

**Who's affected:**
- Creators who built workflows around the Sora API face immediate disruption
- Businesses that integrated Sora (including Adobe Firefly, which offered Sora-powered video) must find replacements
- The Sora community (~6+ months old) is migrating to Kling, Runway, and Veo

**The MiniMax/Hailuo warning:** The Sora shutdown validates advice from video production professionals that "platform risk is real" — and highlights that Runway (where AI video is the entire business) and Veo (central to Google's AI strategy) are safer commercial bets than AI video features from general-purpose AI labs.

**Community reaction:** Widespread shock, with many noting the irony of the Disney deal just months prior. "OpenAI proved you can't trust them with creative tooling" was a common sentiment across Reddit and X.

**Sources:** Ars Technica, BBC, The Guardian, NYT, Euronews, Axios, 9to5Google — March 24–25, 2026

---

### 🟠 Sora App Was Already Failing Before Shutdown — March 19, 2026 (Historical)

**What happened:** OpenAI is planning to absorb its standalone **Sora** video generation app into **ChatGPT**, according to code evidence found in ChatGPT's Android app (version 1.2026.076) by Android Authority. The integration would expose Sora's capabilities to ChatGPT's 400+ million active users — and effectively marks the failure of Sora as a standalone consumer product.

**Why Sora failed as a standalone:**
- **No free tier** (as of January 2026) — while competitors like Runway offer free credits, Sora required a paid subscription from day one
- **Sora 1 forcibly retired on March 13** — all historical content deleted with minimal warning; existing subscribers lost access to their generated content
- **Sora 2 bugs plagued from launch** — "stuck at 99%" generation failures, "under heavy load" queuing errors, API errors for advertised 15/20-second durations
- **ChatGPT "Cameo" trademark blocked by court injunction** — a planned Sora-within-ChatGPT feature was legally challenged by Hollywood studios
- **Quality ceiling** — Kling 3.0 and Google Veo 3 overtook Sora 2 on cinematic realism benchmarks despite Sora's "flagship" positioning

**The absorption strategy:** Rather than compete as a standalone video product, OpenAI is pivoting to bundle Sora's generation into ChatGPT's multimodal interface — similar to how DALL-E image generation became an implicit ChatGPT feature rather than a product in its own right. The move follows OpenAI's stated strategy of centralising all its capabilities within the ChatGPT umbrella to justify the subscription price.

**What this means for video creators:** Sora-as-a-product is effectively dead. The professional video generation market (Runway, Kling, Veo 3) remains competitive — but Sora won't be a serious contender as a standalone tool. Creators who built workflows around the Sora API will face disruption.

**Source:** Android Authority code discovery, The Information, AI.cc — March 19, 2026

---

### 🔴 Runway + NVIDIA Real-Time AI Video: A Breakthrough That Could Supercharge Deepfake Scams — March 23, 2026

**What happened:** Runway demonstrated a new unnamed AI video model at NVIDIA's GTC conference (March 18, revealed publicly March 23) capable of generating HD video in **real time — with a time-to-first-frame under 100 milliseconds**. The model was trained on NVIDIA's new Vera Rubin hardware and can react, respond, and generate continuously as a live AI avatar.

**The capability:** A human operator can control an AI-generated avatar in real time. The avatar looks realistic, reacts immediately, and speaks. This is not a pre-rendered deepfake — it is a **live, interactive AI persona** that can be directed in real time by a human behind a screen.

**Why this is alarming:**
- Currently, deepfake video scams require pre-rendered clips or near-real-time generation with noticeable lag. This removes both of those tells.
- Fraudsters already use deepfake video calls to impersonate bank officials, family members, and executives in scam operations (see voice-creation.md re: WIRED "face model" story)
- With 100ms generation, an AI avatar can respond naturally to a live conversation — nodding, reacting, answering questions — **becoming indistinguishable from a real video call**
- WIRED noted in the same week that human workers are already being recruited to sit in front of cameras operating deepfake personas to scam victims; this technology eliminates even the need for a human operator

**The misuse scenario:** A scammer in a pig-butchering or romance fraud operation could conduct an entire live video call as a cloned version of a known contact, bank employee, or romantic interest — with no lag, no pre-recorded clips, and no tells.

**PetaPixel (March 23):** "AI, along with misinformation and bad actors, is already undermining what people see online. But AI video in real time is an even bigger step as the technology could be used to scam people in the real world as someone controlling an AI avatar reacts and responds to a real person."

**Official position:** Runway has not published safety frameworks for this technology. No mention of watermarking or detection tools in the announcement.

**Sources:** PetaPixel, Runway Twitter/X, NVIDIA GTC, Reuters — March 18–23, 2026

---

### 🟠 Chinese AI Video Goes Monetizable — Deepfake + Copyright Risks Scale Globally — March 20, 2026

**What happened:** Japan Times analysis (March 20, 2026) documented how Chinese AI video tools — particularly Kuaishou's platform — have crossed a quality threshold that makes them "monetizable." The piece examines how Chinese AI video previously looked obviously artificial; it now looks convincingly real.

**The dual risk:**
1. **Copyright:** Kuaishou and similar tools are generating content that incorporates copyrighted characters, styles, and IP without licensing — creating a copyright enforcement crisis that mirrors Seedance 2.0 but at lower profile
2. **Deepfakes:** Higher quality = harder to detect. The same quality improvement that makes these tools useful for legitimate creators makes them more dangerous as fraud and disinformation weapons

**Sources:** Japan Times — March 20, 2026

---

### 🔴 Seedance 2.0 — US Senators Demand Immediate Shutdown + Hollywood Pressure — UPDATED March 17, 2026

**What happened:** ByteDance's Seedance 2.0 has become the AI video industry's most significant legal confrontation. Launched February 10–12, 2026, the model's ability to generate hyper-realistic content featuring copyrighted characters sparked an unprecedented coordinated Hollywood response — and has now forced ByteDance to **suspend its planned global rollout** entirely.

**Timeline:**
- **Feb 10–12, 2026:** Seedance 2.0 launches; viral videos featuring Disney characters (including a Tom and Jerry clip), Star Trek, South Park, Dora the Explorer spread across Chinese social media
- **Feb 13, 2026:** Disney sends formal cease-and-desist letter, accusing ByteDance of training Seedance 2.0 on Disney works without permission and distributing copyrighted IP **as if it were public domain**
- **Feb 2026:** Paramount Skydance cites "blatant infringement" of its IP including Star Trek, South Park, and Dora the Explorer; demands immediate cessation
- **Feb 16, 2026:** ByteDance issues vague statement saying it "respects intellectual property rights" and "heard the concerns" — widely seen as non-committal
- **Multiple studios follow:** Warner Bros Discovery, Netflix also send C&D letters demanding Seedance "immediately cease its infringing activity"
- **March 14, 2026:** Reuters confirms ByteDance has **put on hold the global launch** of Seedance 2.0 after a series of copyright disputes with major Hollywood studios and streaming platforms
- **March 15, 2026:** Multiple outlets confirm the suspension; PCMag, SCMP, Cybernews, India Today, Times of India all report the global rollout is paused
- **March 17, 2026 (NEW):** US Senators **Marsha Blackburn (R-TN) and Peter Welch (D-VT)** write to ByteDance CEO demanding the "**immediate shutdown**" of Seedance 2.0. The senators call it "the most glaring example of copyright infringement from a ByteDance product to date" and demand "meaningful safeguards to prevent further infringing output." On the same day, **Motion Picture Association (MPA) CEO Charles Rivka** released a statement calling upon ByteDance to "immediately cease all infringing activities through the video generation platform." This represents the first formal bipartisan congressional demand to shut down a specific AI video tool.

**Why this matters:** Seedance 2.0 was being positioned as the most capable AI video model of 2026 — capable of generating cinematic-quality video featuring recognisable brand IP at scale. Disney's accusation that ByteDance was essentially treating Disney's entire catalogue as "free public domain" summarises the core grievance: the model was trained on copyrighted material and enables anyone to generate infringing content on demand.

**Scale:** The four simultaneous C&D letters from Disney, Paramount/Skydance, Netflix, and Warner Bros represent the broadest coordinated Hollywood action against a single AI model yet — now escalated to formal congressional pressure. This directly affects ByteDance's global expansion plans and creates legal/political risk that could effectively kill Seedance 2.0 as a global product.

**Community reaction:** The creative community — animation studios, game developers, filmmakers — has been "justifiably denounced" the platform per the senators' own letter. The MPA (representing the major studios) and Congress acting in lockstep is unprecedented for an AI tool.

**Source:** CNBC, Engadget, Washington Times, IPWatchdog, Reuters, PCMag — February–March 14–17, 2026

---

### 🔴 Runway AI Class Action — YouTuber Sues Over YouTube Video Scraping

**What happened:** On **February 24, 2026**, YouTube creator **David Gardner** filed a proposed class action lawsuit against Runway AI in California federal court. The lawsuit alleges Runway:
1. Used data-scraping tools to **download YouTube videos unlawfully**
2. **Circumvented YouTube's technological protection measures** (violating DMCA Section 1201)
3. Used the scraped content without permission to train its video generation models

**Scale:** This is copyright case #84 in the AI space per tracking by "Chat GPT Is Eating the World" — the cumulative legal pressure is building. Runway's valuation of $5.3 billion makes it a high-profile target.

**Significance:** Unlike training data cases arguing copyright infringement of the training set, this case specifically targets **DMCA anti-circumvention** (1201(a)) — a potentially more powerful legal avenue. YouTubers and content creators across the platform are watching closely.

**Community reaction:** Strong support from creator communities. The case feeds into broader anger at AI companies consuming creator content without compensation.

**Source:** Reuters, The Hindu, Economic Times — February 24, 2026

---

### 🟠 OpenAI Sora "Cameo" Feature — Trademark Injunction

**What happened:** OpenAI launched a feature for Sora called "Cameo" allowing users to create and share virtual likenesses of real people. Celebrity-facing company **Cameo** (the personalised shout-out platform) immediately sued for trademark infringement. On **February 17, 2026**, U.S. District Judge Eumi Lee ruled that OpenAI's Cameo feature was **"likely to confuse consumers"** and issued an injunction blocking OpenAI from using the "Cameo" name.

**Background:** OpenAI's Sora has faced Hollywood backlash since its October 2025 launch for allowing real people to appear in AI-generated videos. The "Cameo" branding choice was seen as deliberately invoking the personalised video industry — where consent and authenticity are central to the value proposition.

**Source:** Reuters — February 17, 2026

---

### 🟡 Pricing Chaos & Audio-Native Video Gap

**What happened:** The AI video tool landscape in 2026 is chaotic for buyers. Average cost per minute of AI video dropped 65% from 2024 to 2025 due to competitive pressure, but pricing models remain wildly inconsistent across platforms. A critical divide has also emerged: tools with **native audio** (Seedance 2.0, Veo 3.1, Kling 2.6, Sora 2) vs tools requiring separate post-production audio (Runway, Pika, Luma, all open-source). Creators on Runway face significant additional workflow cost and friction.

**Community reaction:** Reddit's r/Freepik_AI captures the mood: "the pricing models are all over the place and it feels like everything is still in flux." Many creators are using 2–3 tools in combination to get usable output, multiplying subscription costs.

**Source:** Reddit r/Freepik_AI, vidau.ai, pxz.ai — February–March 2026

---

### 🔴 Sora 1 Forcibly Retired — Historical Content Deleted — Sora 2 Broken — March 13–16, 2026

**What happened:** On March 13, 2026, OpenAI **forcibly retired Sora 1** — not a deprecation notice or a gradual wind-down, but a hard shutdown. Simultaneously, its replacement Sora 2 has been plagued by widespread generation failures.

**What was lost:**
- All Sora 1 generation history permanently deleted (no migration path offered, only a limited export window)
- Sora 1's built-in image generation feature also taken offline (redirected to ChatGPT)
- Work saved inside the Sora platform — including mashups, favorites, and iterative creative sessions — gone

**Sora 2's broken state (March 13–16, 2026):**
1. **"Stuck at 99%"** — The most widely reported bug: videos reach 99% completion and hang indefinitely, with no output and no error. Heavily documented on the OpenAI community forum.
2. **"We're under heavy load" errors** — Appear to be a load message but actually disguise the fact that free-tier generation has been completely disabled.
3. **New accounts locked out** — Even after upgrading to ChatGPT Plus ($20/month), new accounts face a 1–3 day review hold before Sora functionality is activated.
4. **Content moderation overreach** — Sentinel moderation system blocking large numbers of normal, non-violative prompts.
5. **Daily rolling credit caps** — Even with sufficient monthly credits, generation is throttled after approximately 30 credits/day.

**Access cliff:**
- Free users: Completely locked out since January 2026 (not just degraded — zero access)
- Plus ($20/month): Limited credits, 480p unlimited, 720p limited
- Pro ($200/month): Full access with 10,000 credits/month

**Community reaction:** Vocal backlash on Reddit (r/OpenAI, r/SoraAI):
- "When they turned it into a TikTok recreation I was done. What garbage. I want a system I can prompt video clips and composite them in my own way. Sora is flaming garbage until they revert back to the OG model."
- Multiple users noting they paid Plus specifically for Sora 2 and still cannot generate videos due to the account review period
- Users migrating to Kling, Runway, Hailuo, Pika as alternatives

**Why this is a rug-pull pattern:** The Sora 1 retirement followed the classic "launch free → grow dependency → kill free tier → force paid upgrade" playbook. Users who built workflows around Sora 1 were given no migration path. The move also coincides with OpenAI integrating Sora directly into ChatGPT — making the standalone Sora product purely a premium ChatGPT feature rather than an independent tool.

**Source:** Apiyi.com, Reuters (March 11), Reddit r/OpenAI, OpenAI community forum — March 10–16, 2026

---

### 🟠 Runway AI: High Costs, Slow Queues, Opaque Moderation — Ongoing 2026

**What happened:** Product Hunt reviews (published within the past week as of March 16, 2026) show a consistent split opinion on Runway: praised for quality output and advanced control features, criticised heavily for:
- **High costs** relative to competitors (Kling, Pika, Hailuo now offer comparable output at lower prices)
- **Slow "relaxed" queues** — lower-tier subscribers wait significantly longer for generation
- **Weak prompt adherence** — described as inconsistent; prompts often partially ignored
- **Opaque moderation and account actions** — users report banned accounts and moderated content without explanation or appeal path

**Source:** Product Hunt reviews, r/runwayml — March 2026

---

### 🟠 AI Video Weaponised for War Propaganda — Journalism "Can't Keep Up" — March 2026

**What happened:** Mediaite published an op-ed (March 12, 2026) documenting the collapse of the traditional propaganda gatekeeping system in the context of ongoing conflicts, driven specifically by AI video generation:

**Key finding:** "That entire system has collapsed under the weight of cheap editing software, AI animation tools, and frictionless global distribution."

**The specific tools cited:** OpenAI's Sora 2, Runway's Gen-4, and Kuaishou's Kling 3.0 can now "generate up to two minutes of continuous, high-definition video from a single text prompt" — making fabricated war footage nearly indistinguishable from real footage.

**The journalism capacity gap:** Traditional journalism relied on editing gatekeepers who could delay and verify. AI-generated war content bypasses this entirely — fake footage goes viral before verification infrastructure can catch up.

**Grok as a force multiplier:** Compounding the problem, Grok (xAI) was simultaneously documented generating fake Iran war images AND wrongly verifying AI-generated fakes as real when users submitted them for fact-checking. This combination — AI generating propaganda + AI "verifying" it as real — is unprecedented.

**The deepfake targeting of Olympians:** Separately (KSLTV.com), con artists are using AI deepfakes targeting Olympic athletes and their fans — creating convincing fake endorsement videos, fake charity appeals, and impersonation scams using Olympic athlete likenesses.

**Source:** Mediaite (March 12, 2026), TechCabal (March 12), KSLTV.com — 2026

---

### 🟠 Sora 2 API: Duration Extension Bug Returning 400 Errors — March 2026

**What happened:** OpenAI's Sora 2 API is shipping documented bugs that are breaking developer integrations. The OpenAI Developer Community forum thread "Sora-2 API not allowing video durations of 15 or 20 seconds" documents a concrete regression: OpenAI announced support for 15-second and 20-second video durations and video extension workflows — but the API is returning **400 errors** when developers request these durations, only accepting the old 4, 8, and 12 second values.

**The specific bug:**
- Sora 2 API documentation says 15 and 20 second durations are supported
- API returns `400: invalid integer` when 15 or 20 second values are passed
- Video extension workflow also broken — passing 16 seconds for extension rejected
- Developers who built integrations based on announced capabilities are blocked

**Context — Sora 2's ongoing reliability crisis:**
This API bug is the latest in a series of issues affecting Sora since it relaunched as Sora 2:
- Videos frequently stuck at 99% completion with no error and no recovery
- Constant "under heavy load" errors blocking generation
- New accounts having video generation features disabled immediately
- Free access removed entirely (January 2026)
- Sora 1 historical content deleted when Sora 2 launched
- API duration extension bug (March 2026) — documented and unresolved

**Developer reaction (OpenAI forum):** "I'm attempting to create videos longer than 12 seconds since OpenAI has recently released the ability to create input '15' and '20' for duration... Unfortunately, I'm receiving a 400 error stating that my input of 16 seconds is an invalid integer when extending a video."

**Why it matters:** Sora 2 is positioned as OpenAI's flagship creative AI product and is integrated into Adobe Firefly's video editor. API instability at this level undermines every downstream integration that depends on reliable video generation.

**Source:** OpenAI Developer Community forum; apiyi.com Sora March 2026 analysis — March 2026
