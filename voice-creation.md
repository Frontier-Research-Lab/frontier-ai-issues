# voice-creation — AI Issues Radar

_Last updated: 2026-03-21_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 1 | 🔴 Critical | UN Global Wake-Up Call — deepfakes and voice cloning "weaponised" by organised crime networks in Southeast Asia for fraud, money laundering, malware | AI voice/deepfake tools (misused) | Active (March 17, 2026) |
| 2 | 🔴 Critical | Deepfake attacks rise 900% — women most targeted; India cybercrime involving women up 60% in two years (50K→80K complaints) | AI voice/image tools (misused) | Active |
| 3 | 🔴 Critical | 1 in 4 Americans received deepfake voice call in past 12 months — AI voice weaponisation has gone mainstream | AI voice tools (misused) | Active |
| 4 | 🔴 Critical | P1bot AI vishing platform discovered — automated fraud calls using ElevenLabs TTS; scammers never have to speak to victims | ElevenLabs (misused) / AI voice tools | Active |
| 5 | 🔴 Critical | Deepfake audio is an evidence crisis — courts not equipped for synthetic audio challenges; voice familiarity standard inadequate | Industry-wide | Active (March 15, 2026) |
| 6 | 🔴 Critical | Creator voice scraping epidemic — any creator's voice, cadence, and phrasing can be modelled and reproduced without consent | Industry-wide | Ongoing |
| 7 | 🔴 Critical | ElevenLabs sued for misappropriating voice actors' likenesses without consent (Vacker & Boyett) — multiple ongoing lawsuits | ElevenLabs | Active |
| 8 | 🔴 Critical | Unauthorised celebrity voice clone epidemic — several lawsuits ongoing; "iconic" deceased voices on platforms that cannot consent | Multiple platforms | Ongoing |
| 9 | 🟠 Major | Celebrity voice licensing ≠ consent for all voices: Michael Caine, McConaughey licensed their voices — but many "iconic" platform voices are deceased or non-consenting | ElevenLabs / AI voice platforms | Active (March 15, 2026) |
| 10 | 🟠 Major | Legal grey areas around derivative voices, group recordings, and future use of synthetic audio remain unresolved | Industry-wide | Ongoing |
| 11 | 🟡 Notable | State laws (CA/NY/TN) creating patchwork compliance requirements for voice cloning platforms | Industry-wide | Developing |

---

## Details

### 🔴 1 in 4 Americans Received Deepfake Voice Call in Past 12 Months — March 14, 2026 (TODAY)

**What happened:** TechRadar published new research today (March 14, 2026) revealing the scale at which AI-generated voice fraud has entered mainstream American life: **one in four Americans report receiving a deepfake voice call in the past 12 months**. Security researchers quoted in the article state: "In 2026, cybercrime has reached a point of total convergence."

**The three key shifts per Keepnet research (March 2026):**
1. **Voice cloning for phone-based vishing** — real-time impersonation of trusted contacts, executives, family members
2. **Deepfake videos in video calls and messaging apps** — faces and voices simultaneously cloned in real-time
3. **AI-generated background noise** — calls now include synthetic office ambience, crowds, traffic to make fraud calls sound authentic and contextually plausible

**Why this matters beyond scam statistics:** This signals that voice AI has crossed from niche misuse to mass-scale weaponisation. At 1-in-4 saturation, it is no longer possible to treat AI voice fraud as an edge case. Every voice generation platform now contributes to an ecosystem where:
- Grandparent scams clone grandchildren's voices in distress
- CEO fraud impersonates executives for wire transfers
- Government impersonation (IRS, Social Security, police) exploits AI voices
- Political deepfakes disrupt elections and public discourse

**Regulatory gap:** The P1bot discovery (see below) confirms this is industrialised. Despite ElevenLabs' stated acceptable use policies, its TTS capabilities are being directly misused in fraud platforms with minimal apparent enforcement.

**Source:** TechRadar, Keepnet — March 14, 2026

---

### 🔴 P1Bot AI Vishing Platform — ElevenLabs Embedded as First-Class Feature — March 11, 2026

**What happened:** Mirage Security researchers (Help Net Security, March 11, 2026) uncovered **P1bot** (p1bot.io) — a fully commercial, subscription-based AI-powered vishing (voice phishing) platform. Critically: P1bot **integrates ElevenLabs as a first-class, native feature** — not just bolted on by individual operators. The integration is polished, the voice catalog is curated, and the workflow is designed to lower the barrier for anyone willing to pay.

**Business model:** Scammers register via a Telegram bot, pay **$399/month** via OxaPay crypto payment gateway, and access a web dashboard to run automated voice fraud campaigns.

**Core capabilities:**
- **Scammers never have to speak to victims** — P1bot plays messages pre-recorded with natural AI-generated ElevenLabs voices
- The platform is a browser-based softphone: operators can spoof phone numbers, generate AI voice prompts, and place calls via WebRTC
- Targeted at impersonating banks ("your account has been compromised — press 1"), tech support, government agencies
- Full "press 1" scam automation — the entire fraud flow from lure to credential extraction

**ElevenLabs' exposure:** Mirage Security CEO Ross Lazerowitz: "P1bot represents something different: a commercial, subscription-based platform where ElevenLabs is embedded as a first-class feature, not bolted on by individual operators. The integration is polished, the voice catalog is curated." This means ElevenLabs' specific voice capabilities are what make P1bot work — raising direct questions about ElevenLabs' ability to detect and prevent misuse of its API.

**Why this is a step-change:** Previous voice fraud required either a live human scammer or crude TTS. P1bot is a polished SaaS product — $399/month for industrial-scale AI voice fraud. Microsoft's threat intelligence team (March 6, 2026) confirmed threat actors are "using AI-generated voice cloning to impersonate executives or trusted individuals in vishing and business email compromise (BEC) scams."

**Real-world impact:** Ericsson disclosed a breach traced to a vendor vishing attack (The Register, March 10, 2026) — social engineering via phone. AI voice tools lower the barrier to this type of attack dramatically.

**Source:** Help Net Security, Mirage Security Blog (miragesecurity.ai), Microsoft Security Blog, The Register — March 6–11, 2026

---

### 🔴 Creator Voice Scraping Epidemic — March 2026

**What happened:** Junia AI (March 2026) documented what it called "the most obvious example of a wider 2026 creator problem that is now painfully normal: your voice, your cadence, your 'signature' phrasing, your whole vibe can be scraped, modelled, and reproduced." Key findings:
- Any public audio content (podcasts, YouTube, TikTok) is potentially harvesting material
- The few seconds of audio needed for voice cloning is trivially obtainable for any public figure
- No consent mechanism exists for retroactive audio that predates AI voice cloning tools
- Current protections (DMCA takedown, platform policies) are reactive and too slow for real-time misuse

**Grok's Nicki Minaj hallucination case (adjacent issue):** A Gothamist story (March 10, 2026) documented a court case where lawyers used Grok to research Nicki Minaj — and Grok hallucinated case citations. When the judge discovered this, he dismissed the entire lawsuit. This illustrates how AI tools in legal contexts are creating new failure modes adjacent to voice/identity abuse.

**Source:** Junia AI, Gothamist, First Reliance Bank — March 2026

---

### 🔴 ElevenLabs Sued for Voice Misappropriation — Vacker & Boyett

**What happened:** Voice actors **Karissa Vacker and Mark Boyett** filed a federal lawsuit against ElevenLabs alleging the company misappropriated their voices to build its text-to-speech software. The plaintiffs argue ElevenLabs trained its AI by **circumventing technological protections** they had placed on their copyrighted material — essentially scraping protected audio to train the "Bella" and "Adam" voice personas without consent or compensation.

**Legal claims:** The lawsuit specifically requires ElevenLabs to instruct users not to create "Bella," "Adam," or similar voice clones. Bloomberg Law reported the suit in August 2024; it was still active heading into 2026 with no publicly announced settlement.

**Who's affected:** Professional voice actors whose livelihoods depend on uniqueness of voice. The precedent has enormous implications: if platforms can train on scraped audio, the entire voice-acting profession faces existential threat from technology that replicates the workers it displaced.

**Community reaction:** Voice acting communities (Voice Realm, SAG-AFTRA affiliates) are deeply hostile to ElevenLabs. Despite the lawsuits, ElevenLabs continued growing aggressively. The platform's consent policy was updated in 2026 to require explicit consent for all voice clones, but enforcement mechanisms remain weak.

**Source:** Bloomberg Law (Aug 2024), The Voice Realm (Oct 2025), Blank Rome LLP — ongoing

---

### 🔴 Unauthorised Celebrity Voice Clone Epidemic

**What happened:** As of 2026, several lawsuits are ongoing involving **unauthorised celebrity voice clones** created through ElevenLabs and other platforms. Bad actors are using freely available voice samples to clone celebrity and public figure voices for disinformation, fraud, and non-consensual content. The most alarming real-world abuse pattern is financial fraud: cloning a family member's voice and sending audio messages requesting money transfers.

**Scale:** ElevenLabs' own help documentation acknowledges the risk but places legal responsibility on users rather than the platform. The company's "we only partner with clients who adhere to our policies" position is widely seen as insufficient given the ease of abuse on free/cheap tiers.

**Community reaction (2023 Reddit thread that remains highly relevant):** "ElevenLabs is a company of like 5 people and they are fully aware that what people can do with this technology is like, take someone's mom's voice and send messages to that person asking for money to be wired." This critique only grew as the company scaled.

**State law complexity:** California, New York, and Tennessee have enacted voice protection laws. Platforms operating nationally must now navigate a patchwork of state requirements — a compliance burden that disproportionately affects smaller companies.

**Source:** leaveit2ai.com, Blank Rome LLP, Reddit (multiple threads) — 2023–2026

---

### 🟠 Celebrity Voice Licensing Doesn't Solve the Consent Crisis — March 15, 2026

**What happened:** TechRadar (March 15, 2026) reported on AI voice platforms signing high-profile celebrities — including **Michael Caine and Matthew McConaughey** — to licence their voices for commercial AI use. The story highlights a core problem the deals don't solve: **"not every 'iconic' voice on the platform can consent."**

**The consent gap:** AI voice platforms promote their licensed celebrity catalogue as proof of ethical practise. But alongside these consensual deals, the same platforms host:
- Voices of deceased celebrities (who cannot consent retroactively)
- Voices of living people who never agreed to having their voice modelled
- Voices derived from historical recordings without rights clearance
- "Iconic" voice personas that evoke real people without directly using their recordings

**Why licensing deals can obscure the problem:** When ElevenLabs announces a deal with a living celebrity, it generates positive press about ethical AI voice development. But those deals don't address the broader library of voices that weren't acquired through consent-based agreements.

**The dead celebrity problem:** Several AI voice platforms offer voices of deceased celebrities and historical figures — voices that cannot legally "consent" to synthetic reproduction under existing frameworks. Estates may hold IP rights but the ethical question of reproducing a person's voice after death is unresolved by current laws.

**Source:** TechRadar — March 15, 2026

---

### 🟠 Grey Areas: Derivative Voices, Group Recordings, Future Use

**What happened:** Even experts who defend AI voice cloning struggle with edge cases: What happens when a voice is "derived" from another voice via style transfer? Who owns a group recording? Can consent given today be revoked for future AI-generated content? As of 2026, these questions remain legally unanswered, creating ongoing risk for anyone using AI voice tools commercially.

**Source:** terms.law, margabagus.com — February 2026

---

### 🟡 State Law Patchwork: CA/NY/TN Voice Protection Laws

**What happened:** Without comprehensive federal regulation, states are filling the void with inconsistent voice protection laws. California (strongest protections), New York, and Tennessee have all enacted legislation. For a national platform like ElevenLabs, this means maintaining separate compliance stacks for different jurisdictions — and users in protected states face different terms than those in unprotected states.

**Source:** terms.law — November 2025

---

### 🔴 UN Global Wake-Up Call — Voice Cloning Weaponised by Organised Crime — March 17, 2026 (TODAY)

**What happened:** The United Nations issued a global alert on March 17, 2026, describing how **organised crime networks in Southeast Asia have weaponised AI voice cloning and deepfakes** as core operational tools for fraud, money laundering, and cybercrime-as-a-service operations.

**Key UN findings (news.un.org, March 17):**
- Criminal networks are deploying AI for **voice cloning** and **deepfake video** in coordinated fraud operations
- These tools are now being sold as **cybercrime-as-a-service** — other criminals can purchase deepfake fraud capabilities without technical expertise
- The same networks also **facilitate money laundering and deploy malware**
- The operations are transnational and increasingly industrialised — not individual bad actors

**Scale of the voice fraud epidemic (corroborating data from TechRadar, March 2026):**
- **1 in 4 Americans** report receiving a deepfake voice call in the past 12 months
- Scammers successfully impersonate family members, executives, and government officials in real-time
- Mobile network protections have been consistently outpaced by AI voice generation improvements

**The evidence crisis dimension (Forbes, March 15):** Legal scholar Lars Daniel documented a federal case where a defense challenge to a voice recording on deepfake grounds was rejected because "witness familiarity with the defendant's voice" was deemed sufficient. This standard was designed before any human could clone a voice from a few seconds of audio — the legal framework has completely failed to keep pace.

**Source:** UN News (news.un.org), TechRadar, Forbes (Lars Daniel), Africa Global Village — March 15–17, 2026

---

### 🔴 Deepfake Attacks Rise 900% — Women Most Targeted — March 2026

**What happened:** New research (Business Standard, March 15, 2026) documents a **900% increase in deepfake attacks**, with women disproportionately targeted:

**India-specific data:**
- Cybercrime complaints involving women jumped from **roughly 50,000 in 2024 to nearly 80,000 by 2026** — a 60% increase in two years
- The Keepnet report (March 2026) attributes the rise primarily to "highly convincing voice and video scams" that combine voice cloning with smishing and spear-phishing

**Global pattern:**
- Attackers are "moving beyond simple impersonation tactics" — they now combine voice, video, and environmental audio for multi-layered deception
- The "most women take no action" finding in the report suggests a systemic reporting gap that means real incident counts are significantly higher than official figures

**YouTube's response:** YouTube escalated deepfake policy with detection and removal capabilities in March 2026, citing "the surge in realistic AI voice cloning as the primary driver behind this policy escalation."

**Source:** Business Standard, Keepnet, YouTube policy update — March 2026

---

### 🟠 ElevenLabs Pledges $1B in Free Voice Restoration at SXSW — Consent Questions Persist — March 13, 2026

**What happened:** At SXSW 2026, ElevenLabs announced a landmark initiative: pledging **$1 billion in free AI voice restoration technology** to 1 million people living with permanent voice loss. The company partnered with Rebecca Gayheart Dane (wife of the late actor Eric Dane) to promote the programme.

**The positive case:** The initiative is genuinely significant — AI voice restoration for people with conditions like ALS, laryngeal cancer, or stroke-related aphasia is one of the few unambiguously beneficial applications of voice cloning technology. ElevenLabs is committing real resources ($1 billion in free service credits) to a medically vulnerable population.

**Why this raises questions simultaneously:**
- ElevenLabs is running this PR campaign at the same time it faces lawsuits from voice actors (Vacker & Boyett) for misappropriating likenesses without consent
- The company's "Iconic Voice Marketplace" — launched the same week — allows use of celebrity voices including those of individuals who **cannot consent** (deceased celebrities, those with limited legal recourse)
- TechRadar noted: "We know many unauthorized voice clones already exist. ElevenLabs is positioning the Iconic Marketplace as the legitimate version of something that was going to happen anyway."

**The tension:** ElevenLabs is simultaneously the company that:
1. Is doing genuine good (voice restoration for disabled people)
2. Is being sued for taking voice actors' voices without consent
3. Is building a marketplace of "iconic" voices including those of deceased celebrities

**Community reaction:** The SXSW initiative was largely praised by the disability community. The voice actor community was not impressed — the good PR does not resolve the ongoing consent lawsuits.

**Source:** Mashable, Wikipedia, TechRadar — March 13–15, 2026
