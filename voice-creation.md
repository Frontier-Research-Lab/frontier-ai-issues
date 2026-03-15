# voice-creation — AI Issues Radar

_Last updated: 2026-03-15_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 1 | 🔴 Critical | 1 in 4 Americans received deepfake voice call in past 12 months — AI voice weaponisation has gone mainstream | AI voice tools (misused) | Active |
| 2 | 🔴 Critical | P1bot AI vishing platform discovered — automated fraud calls using ElevenLabs TTS; scammers never have to speak to victims | ElevenLabs (misused) / AI voice tools | Active |
| 3 | 🔴 Critical | Creator voice scraping epidemic — any creator's voice, cadence, and phrasing can be modelled and reproduced without consent | Industry-wide | Ongoing |
| 4 | 🔴 Critical | ElevenLabs sued for misappropriating voice actors' likenesses without consent (Vacker & Boyett) — multiple ongoing lawsuits | ElevenLabs | Active |
| 5 | 🔴 Critical | Unauthorised celebrity voice clone epidemic — several lawsuits ongoing; "iconic" deceased voices on platforms that cannot consent | Multiple platforms | Ongoing |
| 6 | 🟠 Major | Celebrity voice licensing ≠ consent for all voices: Michael Caine, McConaughey licensed their voices — but many "iconic" platform voices are deceased or non-consenting | ElevenLabs / AI voice platforms | Active (March 15, 2026) |
| 7 | 🟠 Major | Legal grey areas around derivative voices, group recordings, and future use of synthetic audio remain unresolved | Industry-wide | Ongoing |
| 8 | 🟡 Notable | State laws (CA/NY/TN) creating patchwork compliance requirements for voice cloning platforms | Industry-wide | Developing |

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

### 🔴 P1Bot AI Vishing Platform — Automated AI Voice Fraud at Scale — March 11, 2026

**What happened:** Security researchers (Help Net Security, March 11, 2026) uncovered **P1bot** (p1bot.io) — a fully automated AI-powered vishing (voice phishing) platform for sale to cybercriminals. Key capabilities:
- **Scammers never have to speak to victims** — P1bot plays pre-recorded messages using natural-sounding AI-generated voices
- The platform automates the entire fraud flow: lure, escalate, extract
- Targeted at impersonating banks, tech support, government agencies
- Uses voice synthesis similar to commercial tools (ElevenLabs, Play.ht-style APIs) in weaponised automation

**Why this is a step-change:** Previous voice fraud required either a live human scammer or crude text-to-speech. P1bot is a polished SaaS product specifically designed to automate voice fraud at scale. Microsoft's threat intelligence team (March 6, 2026) confirmed threat actors are "using AI-generated voice cloning to impersonate executives or trusted individuals in vishing and business email compromise (BEC) scams."

**Real-world impact:** Ericsson disclosed a breach traced to a vendor vishing attack (The Register, March 10, 2026) — social engineering via phone. AI voice tools lower the barrier to this type of attack dramatically.

**Source:** Help Net Security, Microsoft Security Blog, The Register — March 6–11, 2026

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
