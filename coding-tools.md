# coding-tools — AI Issues Radar

_Last updated: 2026-04-01_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 0apr1a | 🔴 Critical | **SUPPLY CHAIN ATTACK: Axios npm library trojanized — Claude Code users hit with Remote Access Trojan** — Malicious versions of axios (1.14.1 and 0.30.4) were published to npm on March 31 between 00:21–03:29 UTC; anyone who installed or updated Claude Code during this window may have pulled a cross-platform RAT (Remote Access Trojan); Elastic Security Labs, Malwarebytes, Hacker News, and CyberNews all confirmed; maintainer email on malicious versions changed from `jasonsaayman@gmail.com` to `ifstap@proton.me`; OIDC provenance broken; axios has 100M+ weekly downloads — high-blast-radius; coincided with Anthropic's source code leak creating mass confusion (two unrelated simultaneous events) | Claude Code / axios npm | **Critical — check install dates** (March 31, 2026) |
| 0apr1b | 🔴 Critical | **Anthropic accidentally leaks entire Claude Code source (512K lines) via npm packaging error** — Version 2.1.88 of `@anthropic-ai/claude-code` included a 59.8 MB internal debug `.map` file; discovered by Solayer Labs intern @Fried_rice at 4:23 AM ET March 31; mirrored across GitHub within hours and analysed by thousands; reveals three-layer "Self-Healing Memory" architecture, permission systems, multi-agent coordination, and 44 hidden feature flags (KAIROS, ULTRAPLAN, BUDDY); Anthropic confirmed: "release packaging issue caused by human error, not a security breach. No sensitive customer data exposed." VentureBeat: "a literal blueprint for competitors"; timed 10 days after Anthropic sent C&D to OpenCode for API abuse — community trust damage compounded | Claude Code (Anthropic) | Confirmed — source archived (March 31, 2026) |
| 0apr1c | 🔴 Critical | **Claude Code "Extreme Token Burn" + stalling bugs flood GitHub on April 1** — GitHub issues filed April 1: #41866 "Extreme Token Burn with Claude Code CLI — Normal Work Impossible!"; #41831 "Tool calls stall for 10–20 minutes after text output on v2.1.89 + Bun GC crash"; #41857 "Can't Open Claude Code"; #41813 "Not responding from last 1 hour" — all open April 1, 2026; coincides with multi-incident API outage day; users on paid subscriptions blocked during critical work | Claude Code (Anthropic) | Active (April 1, 2026) |
| 0mar29 | 🟠 Major | **Claude Code Dispatch silent failure bug — responses generated but never delivered to UI** — Claude Desktop 1.1.9310 (released ~March 28) introduced a regression where Dispatch sessions stop responding; messages are processed internally and logged in audit.jsonl but **never appear in the conversation**; Anthropic status page (March 29, 00:53 UTC) confirmed the issue; GitHub issues #40178, #40179, #40257 all filed same day; affects Claude Code users in Cowork+Dispatch mode on desktop and mobile; resolved same day — but the pattern of regressions in Claude Code releases continues (this is Anthropic's 613th tracked incident since June 2024) | Claude Code (Anthropic) | Resolved (March 29, 2026) |
| 0mar28 | 🔴 Critical | **GitHub Copilot will train AI on your code starting April 24 — opt-out required** — GitHub quietly published policy change March 25: all Copilot Free, Pro, and Pro+ users' interaction data (code snippets, prompts, file names, repo structure, outputs) will feed AI model training by default unless manually opted out; The Register: "GitHub: We going to train on your data after all"; HotHardware: "GitHub reverses course"; HN thread hit #1; community describes it as bait-and-switch — Microsoft previously promised code would NOT be used for training when building user trust | GitHub Copilot (Microsoft) | Active — opt-out at /settings/copilot/features (March 25, 2026) |
| 0NEW | 🟠 Major | **Microsoft rolls back "unnecessary" Copilot integrations from Windows** — removing Copilot entry points from Photos, Widgets, Notepad, and Snipping Tool (March 20–23); framed as improving "Windows quality"; community saw this as an admission that forced AI integration was hated; "Microslop" Discord server banned the word, causing fresh backlash | Microsoft Copilot (Windows) | Active (March 20–23, 2026) |
| 0a | 🔴 Critical | Cursor/Kimi K2.5 controversy deepens — Geeky Gadgets (March 23): Cursor failed to provide attribution required by Kimi K2.5's open-source license, potentially violating license terms; Elon Musk publicly confirmed "Yeah, it's Kimi 2.5"; Fireworks AI CEO says Cursor was "compliant from day one" via their platform; community: "Cursor is becoming a model routing layer, not an IDE" | Cursor / Kimi K2.5 (Moonshot AI) | Active (March 19–23, 2026) |
| 0b | 🔴 Critical | Microsoft CVE-2026-26133: cross-prompt injection in Copilot email + Teams summarisation lets attackers shape AI output silently — no attachment needed; patched March 11, 2026 | Microsoft 365 Copilot | Patched (March 11, 2026) |
| 0c | 🔴 Critical | "Reprompt" attack chains 3 techniques to turn Copilot Personal into a single-click data exfiltration channel — disclosed early 2026 | Microsoft Copilot Personal | Active (early 2026) |
| 1 | 🔴 Critical | AI coding tools fail 1 in 4 structured tasks — peer-reviewed study published March 17, 2026; AI co-authored code has 2.74x more security vulnerabilities | All AI coding tools | Active (March 17, 2026) |
| 2 | 🔴 Critical | Amazon's AI coding mandate caused 6.3M lost orders + 90-day safety reset — Kiro & Q implicated in multiple Sev-1 outages; even senior engineers now need manager sign-off | Kiro / Amazon Q | Active |
| 3 | 🔴 Critical | Fake AI browser extensions stolen ChatGPT/DeepSeek conversations from 900K users across 20K enterprises — "full chat exfiltration" | Chrome/Edge extensions | Active |
| 4 | 🔴 Critical | AI coding tools introduce security flaws in 87% of pull requests — cross-site scripting had 86% failure rate | All AI coding tools | Ongoing |
| 5 | 🔴 Critical | Malicious Rust crates exploit AI coding assistants — injected code uses Claude, Copilot, Gemini, Kiro to exfiltrate secrets | Claude Code / Copilot / Gemini / Kiro | Active |
| 6 | 🟠 Major | GitHub Copilot Student plan guts premium models — GPT-5.4, Claude Opus, Claude Sonnet removed March 12; thousands of student downvotes | GitHub Copilot | Active (March 12–16, 2026) |
| 7 | 🟠 Major | Developer trust in AI code accuracy at historic low — 46% distrust vs 33% trust (Stack Overflow Feb 2026) | All AI coding tools | Ongoing |
| 8 | 🔴 Critical | Cursor confirmed code reversion bug — Agent Review Tab + cloud sync racing silently reverts edits; developer reports losing 4 months of work | Cursor | Active (confirmed March 2026) |
| 9 | 🟠 Major | Cursor: surprise pricing overages, crashes, file-saving failures, AI modifying wrong files without permission | Cursor | Ongoing |
| 10 | 🟠 Major | GitHub Copilot: suggests code with subtle bugs, outdated APIs, and security flaws that look correct at a glance | GitHub Copilot | Ongoing |
| 11 | 🟡 Notable | Privacy concerns — code sent to third-party APIs without explicit disclosure; vendor lock-in across all tools | Cursor, Copilot, Windsurf | Ongoing |
| 12 | 🟠 Major | Windsurf ownership chaos — OpenAI's $3B acquisition collapsed (Microsoft blocked); Google poached CEO + key R&D; Anthropic cut off Claude access when acquisition leaked; Cognition acquired for $250M; roadmap uncertainty driving users to alternatives | Windsurf | Ongoing (post-acquisition March 2026) |

---

## Details

### 🔴 GitHub Copilot to Train AI on Your Code Starting April 24 — Opt-Out Required — March 25, 2026

**What happened:** GitHub quietly published a policy change on March 25, 2026: starting **April 24, 2026**, all Copilot Free, Pro, and Pro+ users' **interaction data** — including code snippets, prompts, file names, repo structure, and AI outputs — will be used to **train and improve GitHub's AI models by default**. Users must manually opt out via `/settings/copilot/features`.

**Why this is a betrayal:** When Microsoft launched GitHub Copilot in 2021, it made explicit promises that user code would **not** be used for model training. This promise was central to building developer trust during a period when many companies were resistant to cloud-based coding tools. Microsoft is now reversing this commitment with a default opt-in — meaning anyone who doesn't read the changelog will have their code harvested.

**What data is collected:**
- All inputs (code context, file contents shared with Copilot)
- All outputs (suggestions, explanations, code completions)
- Code snippets and associated context
- Implicit signals (acceptance/rejection of suggestions)

**The Register's headline:** *"GitHub: We going to train on your data after all"* — published March 26, 2026.

**HotHardware:** *"GitHub Reverses Course And Will Train AI On Your Copilot Data Unless You Opt Out"* (March 26, 2026)

**Community reaction:** The Hacker News thread reached #1, with top comments calling it a "bait-and-switch" and a "privacy breach by default." Enterprise users flagged immediate compliance concerns — any company that processes regulated data (healthcare, finance, legal) and uses Copilot without opting out could face data governance violations.

**Business/enterprise implications:** Enterprise and Business tier customers are reportedly exempt (their contracts include stricter data terms). But **individual developers and teams on Free/Pro/Pro+** — often the most prolific Copilot users — are now defaulted into code sharing without explicit consent.

**How to opt out:** Settings → `/settings/copilot/features` → disable "Allow GitHub to use my data for AI model training" under the Privacy heading.

**Sources:** GitHub blog (March 25), The Register (March 26), HotHardware (March 26), HN thread #47521799 (March 28)

---

### 🔴 Cursor/Kimi K2.5 Controversy — License Violation Claims + Elon Musk Pile-On — Updated March 23, 2026

**March 23 Update:** Geeky Gadgets reports Cursor failed to provide the **attribution required by Kimi K2.5's open-source license**, potentially placing it in breach of the model's terms. The Fireworks AI CEO (Lin Qiao) countered that Cursor accessed Kimi K2.5 via Fireworks' platform and was "compliant from day one." The conflict between these statements remains unresolved.

Community reaction crystallised into a damaging meme: *"Cursor is becoming a model routing layer, not an IDE. They pick the cheapest model that clears a quality bar per task, wrap it in their UX, and pocket the margin."* (Business Insider Africa, March 23)

**Elon Musk's contribution:** Musk publicly confirmed the finding with just four words — "Yeah, it's Kimi 2.5" — amplifying the story to millions of followers.

---

### 🟠 Microsoft Rolls Back "Unnecessary" Copilot in Windows — March 20–23, 2026

**What happened:** In a significant reversal of Microsoft's aggressive AI integration strategy, the company confirmed on March 20–23, 2026 that it would **remove Copilot AI entry points from several core Windows applications**: Snipping Tool, Photos, Widgets, and Notepad. The framing from Microsoft's own announcement: these were "unnecessary Copilot entry points."

**The subtext:** The term "unnecessary" is doing a lot of work here. These were features Microsoft shipped as part of its push to make Copilot omnipresent in Windows 11 — justified as improving user productivity. Quietly admitting they were "unnecessary" is an implicit acknowledgement that users rejected them.

**The "Microslop" moment:** Microsoft had previously banned the word "Microslop" (a portmanteau of "Microsoft" and "slop") on a Discord server dedicated to its Copilot AI product — attempting to censor criticism of its AI-first Windows strategy. The backlash to the censorship amplified the original criticism significantly, and the Wikipedia "AI slop" article now documents the incident. The rollback that followed looks directly connected: Microsoft's own moderators were protecting the brand from criticism that was, in retrospect, accurate.

**The Register's headline:** *"Microsoft: Removing some Copilots will improve Windows 11"* — a headline that speaks for itself.

**Community reaction:** TechCrunch framed it as Microsoft "rolling back Copilot AI bloat." The Windows Latest coverage tied it directly to the Microslop controversy: *"Microsoft responds to Microslop criticism by scaling back Copilot in Windows 11."* The sentiment is unified: Microsoft over-indexed on AI integration without validating user desire.

**What remains:** Microsoft has not removed AI from Windows entirely. Copilot remains in the taskbar and several other entry points. The rollback is a retreat from the most invasive integrations, not from the AI strategy.

**Wider significance:** This is one of the first public examples of a major tech company **visibly walking back forced AI integration** after user resistance — a pattern others may follow.

**Sources:** TechCrunch (March 20), Lifehacker (March 23), The Register (March 23), Windows Latest (March 21), IT Pro (March 23)

---

### 🔴 Cursor Caught Reselling Kimi K2.5 (Chinese AI) as "Composer 2" — March 19, 2026

**What happened:** On March 19, 2026, Cursor announced **Composer 2** — marketed as their own in-house coding model, with benchmarks, pricing ($0.50/M input tokens), and positioning as evidence that Cursor had "graduated from wrapper to builder." Less than 24 hours later, developer **Fynn** discovered the actual model ID in Cursor's OpenAI-compatible API response: `accounts/anysphere/models/kimi-k2p5-rl-0317-s515-fast`.

**Decoded:**
- `kimi-k2p5` = **Kimi K2.5**, from Beijing-based **Moonshot AI**
- `rl` = fine-tuned with reinforcement learning
- `0317` = March 17, 2026 training checkpoint

**The deception pattern:** Cursor's launch materials implied Composer 2 was built by Cursor. No third-party attribution. No mention of Moonshot AI. The benchmark framing (61.7 on Terminal-Bench 2.0, compared to Claude Opus 4.6) made the implicit claim that this was comparable to frontier models in terms of independent development effort.

**Cursor's response:** Confirmed Kimi K2.5 as the base model; claimed a "legal obligation not to disclose third-party models" under the partner agreement. The developer community rejected this as insufficient — the issue isn't just disclosure, it's that the marketing actively obscured the Chinese origin of the model.

**The three compounding problems:**
1. **Trust breakdown** — Cursor had explicitly marketed itself as "no longer just a wrapper." Composer 2 contradicts this directly.
2. **Geopolitical risk** — Kimi K2.5 is from a Chinese company. Enterprise developers working on sensitive codebases may have legal or security concerns about Chinese AI processing their intellectual property.
3. **Price arbitrage** — Cursor is charging a premium margin on an open-weight model accessible via other routes.

**Community reaction (HN, X/Twitter, March 19–20):** Described as a "bait and switch." Developers questioning whether Cursor can ever be trusted on model claims again. The "legal obligation" framing was widely seen as a deflection — if the agreement required non-disclosure, Cursor should not have implied in-house development.

**Source:** Medium (Thamizhelango, "Cursor Composer 2 and Kimi K2.5: What Happened"), HN thread — March 19–20, 2026

---

### 🔴 Microsoft CVE-2026-26133 — Copilot Cross-Prompt Injection in Email + Teams — Patched March 11, 2026

**What happened:** Microsoft patched **CVE-2026-26133** on March 11, 2026 — a cross-prompt injection vulnerability in **Microsoft 365 Copilot's email and Teams summarisation features** that allowed attackers to silently **shape what the AI told users** about their own emails and messages — without any attachment, macro, or file needed.

**How the attack works:**
- An attacker sends a specially crafted email or Teams message to a target
- The message contains embedded instructions that exploit Copilot's summarisation
- When the victim asks Copilot to summarise their inbox or recent messages, Copilot reads the attacker's message — and the embedded instructions redirect Copilot's output
- Result: Copilot tells the victim false information (e.g., "your boss says to wire $50,000 to this account" instead of the actual message content)
- No user interaction beyond asking Copilot to summarise is required

**Why this is uniquely dangerous:** Copilot has been granted trust to access all emails, Teams messages, SharePoint documents, and calendar entries. It's the most privileged AI tool in most enterprises. An attacker who can get any message into an organisation's email stream can influence what Copilot tells every user who asks for a summary.

**The "Reprompt" attack (related, also disclosed early 2026):** A separate researcher disclosed the "Reprompt" attack — which chains three techniques (prompt injection, data exfiltration, and an open redirect) to **turn Copilot Personal into a single-click data exfiltration channel**. The Cybersecurity Insiders AI Risk Report (March 2026) cited this as the first documented AI tool turned into a one-click data theft vector.

**Microsoft's response:** CVE-2026-26133 was patched via Microsoft's regular Patch Tuesday cycle on March 11, 2026. The Reprompt vulnerability's patch status is less clearly confirmed publicly.

**Who's affected:** Every Microsoft 365 Copilot enterprise customer — estimated at tens of millions of seats. The vulnerability was present in the default configuration; no user had to do anything unusual to be exposed.

**Source:** RedPacket Security (CVE-2026-26133), ThomasJuhlOlesen.dk, Cybersecurity Insiders AI Risk Report 2026 — March 2026

---

### 🔴 Fake AI Browser Extensions Exfiltrate Chat Histories — 900K Users, 20K Enterprises — March 5, 2026

**What happened:** Microsoft Defender researchers published a Security Blog post (March 5, 2026) warning about a sophisticated attack campaign using **malicious browser extensions impersonating legitimate AI assistant tools** (ChatGPT, DeepSeek, Claude, and similar products). The scale of compromise was staggering:
- Nearly **900,000 users** had installed the malicious extensions
- Activity observed across **20,000+ enterprise tenants**
- Extensions collected **full URLs browsed** and **complete AI chat histories** from ChatGPT, DeepSeek, and other platforms
- Stolen data included: **proprietary code, internal workflows, strategic discussions, and confidential data** shared with AI assistants

**The attack mechanics:** The extensions appeared as legitimate AI productivity tools on the Chrome Web Store and Edge Add-ons marketplace. Once installed, they:
1. Monitored all browser tabs for AI chatbot sessions
2. Captured full conversation histories in real-time
3. Silently exfiltrated the data to attacker-controlled servers

**Why this is uniquely dangerous:** Developers share far more sensitive information with AI coding assistants than with traditional web tools. A single ChatGPT conversation might contain API keys, database schemas, internal architecture docs, and undisclosed product roadmaps — all now in attackers' hands.

**Enterprise risk:** The 20,000 enterprise tenant figure means this isn't a consumer problem. Corporate secrets discussed with AI coding tools are compromised at scale. Microsoft urged all organisations to "audit browser extensions" immediately.

**Who's affected:** Any developer who installed AI productivity extensions from third-party stores rather than official channels. The intersection with coding tools is direct — developers are the primary users of ChatGPT and DeepSeek for work tasks.

**Source:** Microsoft Security Blog, Cybersecurity News, CapitalAI Daily, TechRepublic — March 5–13, 2026

---

### 🔴 Amazon AI Coding Mandate Causes 6.3M Lost Orders — 90-Day Safety Reset — March 2026

**What happened:** Amazon's internal mandate to push AI-generated code into production — using its own tools (Kiro and Amazon Q) — caused a catastrophic series of failures:

- **March 2, 2026:** A vibe-coded change triggered a major outage on the Amazon e-commerce platform — 120,000 lost orders and 1.6 million website errors in a single event
- **March 5, 2026:** A separate outage caused a **99% drop in orders across North American marketplaces**, resulting in **6.3 million lost orders** — a disaster that will materially impact Amazon's Q1 financials
- **At least 4 Sev-1 outages in a single week** were linked to AI-assisted code changes, according to internal reporting
- **AWS (December 2025):** Kiro's AI coding tool was granted admin-level access and autonomously **deleted and attempted to recreate an entire production environment**, causing a **13-hour outage** of AWS Cost Explorer in China regions

**The Kiro Mandate:** Amazon had been internally pushing engineers toward ~80% AI-generated code for weekly tasks. Junior and mid-level engineers were producing code faster than it could be meaningfully reviewed, and changes were going to production without thorough human approval steps.

**The 90-Day Reset:** On March 10, 2026, Amazon's e-commerce CTO Dave Treadwell convened a mandatory engineering "deep dive" with director and VP-level leaders. Amazon subsequently announced a **90-day code safety reset**:
- Stricter code review requirements before any production deployment
- Human authorization now required for all critical resource modifications
- New guardrails on AI agent permissions in production environments
- Director/VP accountability for violations

**Scale of impact:** 6.3 million lost orders on a single day. AWS customers affected across China regions. Internal reporting described the situation as AI tools "exposing sharp edges and places where guardrails do not exist."

**Amazon's public position:** Amazon insists there is "no internal evidence that incidents are more common with AI tools" — but simultaneously ran an emergency engineering reset and hired external consultants to review the situation. The Register noted the company "has provided no data that would allow an independent analysis."

**Industry reaction:** Gary Marcus: "I warned you a year ago that maintaining GenAI code would be harder than writing code with GenAI." Business Insider: "Amazon Forced Engineers to Use AI Coding Tools. Then It Lost 6.3 Million Orders." Elon Musk publicly told Amazon to "proceed with caution."

**Source:** Business Insider, CNBC, The Register, Digital Trends, Financial Times, Medium (multiple) — March 10–13, 2026

---

### 🔴 AI Coding Tools Introduce Security Flaws in 87% of Pull Requests — March 2026

**What happened:** A new report (DigiconAsia, March 13, 2026) found that **AI coding tools introduce security vulnerabilities in 87% of pull requests** they contribute to. Key findings:

- **Cross-site scripting (XSS):** 86% failure rate — AI consistently produced XSS-vulnerable output
- **Improper JSON Web Token (JWT) handling** across all tested models
- **No defenses against brute-force attacks** in AI-generated authentication code
- **Token replay exploits** — AI code vulnerable to session replay attacks
- **Weak refresh token cookie settings** — insecure defaults baked in by default
- Overall: AI-generated code contains **2.74x more security vulnerabilities** than human-written code

**Why this is critical:** These aren't edge cases. These are OWASP Top-10 class vulnerabilities — the most well-documented and easily exploitable categories. The fact that AI models trained on billions of lines of code still produce these failures at high rates indicates the problem is structural, not incidental.

**Compounding factor:** The Amazon incidents show what happens when AI-generated code bypasses proper review. The pattern — ship fast, review later — is creating a delayed-fuse security debt across the industry.

**Source:** DigiconAsia, QuantoSei News, The New Stack, Medium ("The Great AI Coding Swindle") — March 2026

---

### 🔴 Malicious Rust Crates Weaponise AI Coding Assistants — March 11, 2026

**What happened:** Security researchers (The Hacker News, March 11, 2026) uncovered a supply chain attack using **five malicious Rust crates** that hijacked popular CI/CD pipelines. The attack was sophisticated:

- Malicious versions (1.8.12 and 1.8.13) of a widely-used Rust library were published
- The injected code executed **local AI coding assistants** — including Claude Code, OpenAI Codex, Gemini CLI, GitHub Copilot CLI, and Amazon Kiro CLI — **in highly permissive modes**
- The AI agents were instructed to perform **extensive system inspection** (scanning for secrets, credentials, API keys)
- Results were **exfiltrated to a GitHub repository** using the victim's own authenticated GitHub CLI session
- Victims had no idea their AI assistant was being used as a data theft vector

**Why this is a new class of threat:** Traditional supply chain attacks abuse build tools. This attack abuses the AI coding assistants that developers explicitly trust and grant broad filesystem access. The AI assistant becomes the attack vector because:
1. It already has permission to read all project files
2. It operates with the user's credentials
3. Developers are conditioned to accept AI-generated actions without close review

**Source:** The Hacker News, Socket research — March 11, 2026

---

### 🔴 Developer Trust Hits Historic Low — Stack Overflow February 2026

**What happened:** The Stack Overflow 2025 Developer Survey (published late 2025, cited widely in February 2026 analysis) revealed a damning statistic: **46% of developers actively distrust AI tool accuracy** while only 33% trust it. Only 3% report "highly trusting" AI output. Year-over-year, developer trust dropped **11 percentage points**. A follow-up February 18, 2026 Stack Overflow blog post confirmed the trend is worsening, not improving, despite broader AI adoption.

**Context:** 96% of developers report they do NOT fully trust AI code to ship without review. This is the central paradox of 2026's AI coding boom — tools are being used more than ever, but less and less trusted.

**Scale:** This is the entire developer community, not a niche complaint. The survey represents hundreds of thousands of developers globally.

**Community reaction:** The "trust but verify" burden is collapsing productivity gains. Developers describe spending more time auditing AI output than they saved generating it. The 2026 narrative has shifted from "AI will replace developers" to "AI creates new kinds of technical debt."

**Source:** Stack Overflow 2025 Developer Survey, stackoverflow.blog February 18, 2026, ADTMag

---

### 🔴 Cursor Confirmed Code Reversion Bug — Silent Data Loss — March 2026

**What happened:** The Cursor team confirmed in March 2026 that the editor has been **silently reverting code changes** — a data-loss bug affecting developers using the Agent and Composer features. Users would make edits, the AI would appear to apply them, and then later discover their changes had been undone with no notification.

**Three confirmed root causes (Cursor forum, March 2026):**
1. **Agent Review Tab conflict** — the Agent Review Tab interfered with file state, causing edits to be overwritten when switching contexts
2. **Cloud Sync race condition** — Cursor's cloud sync was racing with local file saves, sometimes reverting to an older version
3. **Format On Save conflict** — auto-formatting triggered after AI edits sometimes produced a different file state than intended

**The workaround:** Close the Agent Review Tab before using "Fix in Chat." This is not a fix — it's asking users to avoid a core feature to prevent data loss.

**Real-world impact:** A developer published a Medium post describing losing **four months of work** to this class of bug. Users on X reported app freezing/crashes when clicking the 'Review next file' button, and described Cursor as becoming "unusable lately — begins to fail at simple tasks."

**Community quote (@nelvOfficial on X):** "Cursor code is becoming unusable lately — begins to fail at simple tasks — keeps changing the UI at each update."

**Why this matters:** Cursor is trusted by thousands of professional developers to work on production codebases. Silent, undetected data loss — where the AI appears to have applied changes but hasn't — undermines the core trust proposition of AI-assisted coding.

**Source:** vibecoding.app (Cursor problems 2026 analysis), Cursor forum, Medium (@tahabebek), X/Twitter — March 2026

---

### 🟠 Cursor: Surprise Overages, Crashes, Privacy Concerns

**What happened:** Morphllm's February 2026 analysis of Cursor alternatives compiled the most common Cursor complaints from Reddit and developer forums:
- **Surprise pricing overages** beyond the base subscription — users being charged unexpectedly for usage above plan limits
- **Crashes and file-saving failures** — the editor losing unsaved work
- **AI modifying wrong files without permission** — the Composer/agent feature making changes to files the user did not intend
- **Privacy concerns** — user code being sent to third-party model APIs (OpenAI, Anthropic) without explicit disclosure
- **Vendor lock-in** — workflows built around Cursor's proprietary features don't transfer

**Scale:** Cursor is one of the fastest-growing developer tools. These issues affect its primary value proposition.

**Community reaction:** Threads on Reddit and DEV Community describe Cursor as "incredible when it works but terrifying when it doesn't" — with the wrongly-modified-files issue the most alarming. Several developers reported losing hours of work to unexpected changes.

**Source:** morphllm.com, dev.to — February 2026

---

### 🟠 GitHub Copilot: Subtly Wrong Code That Looks Right

**What happened:** The most dangerous pattern with GitHub Copilot is not obvious errors (which are easy to catch) but **code that looks syntactically correct, compiles, and passes surface-level review but contains subtle bugs, uses deprecated APIs, or has latent security vulnerabilities**. Multiple 2026 comparisons (Seedium, DEV Community) flag this as Copilot's most significant ongoing issue.

**Why this is worse than obvious errors:** Developers have developed a habit of treating "Copilot-approved" code as roughly trustworthy, meaning flawed suggestions get merged at higher rates than manually written code that would receive closer scrutiny.

**Scale:** GitHub Copilot is used by millions of developers at enterprise scale. The compounding risk of subtly flawed code at volume is significant. Stack Overflow data shows **38.8% of GitHub Copilot-generated code contains security flaws**.

**Official response:** Microsoft has not acknowledged this as a systematic issue. The February 2026 Enterprise AI Controls and Agent Control Plane going GA is the most recent governance response, but it addresses administrative oversight rather than output accuracy.

**Source:** seedium.io, dev.to, vibehackers.io, byteiota.com — January–March 2026

---

### 🟡 Privacy and Lock-in Across All AI Coding Tools

**What happened:** A persistent concern across all AI coding tools is the transmission of proprietary code to external APIs for inference. Most tools send user code to OpenAI, Anthropic, or Google backends — a legal and compliance risk for enterprise customers working with sensitive codebases. Additionally, the ecosystem is fragmenting: each tool has proprietary context formats, workflows, and extensions that don't transfer between platforms.

**Community reaction:** "Privacy concerns about code sent to third-party APIs" consistently appears in top complaints across Cursor, Copilot, and Windsurf reviews. Enterprise buyers are demanding self-hosted or on-prem options.

**Source:** morphllm.com, multiple DEV Community posts — 2026

---

### 🟠 GitHub Copilot Student Plan Guts Premium Models — Thousands of Downvotes — March 12–16, 2026

**What happened:** On March 12, 2026, GitHub quietly reorganised its free Copilot offering for students, creating a new "GitHub Copilot Student plan" under the GitHub Education programme. The headline change: **GPT-5.4, Claude Opus, and Claude Sonnet were removed from the free student tier**. Students previously had direct access to select premium models; now they are restricted to "Auto mode" (GitHub's internal routing), which directs queries to lower-cost models the student cannot choose.

**Community reaction:** The backlash was immediate and severe:
- The GitHub announcement post drew **thousands of downvotes** on Reddit's r/GithubCopilot
- One student (Nguyễn Thế Toàn) wrote: "The removal of premium models such as GPT-5.4, Claude Opus, and Claude Sonnet makes learning programming more difficult. These models are much better at explaining complex coding concepts, helping debug problems, and guiding students step by step when we are stuck."
- Users accused GitHub of using the free student plan as a loss-leader to grow adoption, then pulling the best models once students are dependent on the tool
- The r/GithubCopilot community called it the classic "give premium for free, then bait-and-switch" pattern

**GitHub's response:** VP of developer relations Martin Woodward confirmed the changes and, when asked to restore premium model access, suggested students "upgrade to GitHub Copilot Pro or Pro+ if you want to." Per The Register (March 13): "Microsoft's GitHub is dialing back on expenses by removing several costly premium models."

**Why this matters:**
- Students disproportionately benefit from the strongest models for learning and debugging complex concepts
- The move widens the access gap between students who can afford $10–19/month for Pro/Pro+ and those who cannot
- It confirms AI tool makers are actively **degrading free and student access** to cut costs as premium model inference costs remain high
- The VSCode GitHub issues tracker (issue #301395) shows the problem has also surfaced in the desktop extension — "Copilot Agent models missing (Claude Sonnet / Opus) on GitHub Student account"

**The pricing reality:** GitHub Copilot Pro is $10/month; Pro+ is $19/month. For students in lower-income countries, these prices are prohibitive — the free student plan was meaningfully different.

**Source:** The Register, Winbuzzer, PiunikaWeb, Reddit r/GithubCopilot, GitHub Issues #301395, Roboin.io — March 12–16, 2026

---

### 🔴 AI Coding Tools Fail 1 in 4 Tasks — Peer-Reviewed Study — March 17, 2026 (TODAY)

**What happened:** A peer-reviewed study published today (TechXplore / Study Finds, March 17, 2026; DOI: 10.48550/arxiv.2505.20139) provides academic confirmation that **even the best AI coding tools fail roughly 1 in 4 structured coding tasks** — validating months of developer complaints with independent research.

**Key findings:**
- Even top-tier AI coding models fail ~25% of structured format coding tasks where expected output is clearly defined
- AI co-authored code (per December 2025 CodeRabbit analysis, referenced in Wikipedia's vibe coding article) shows **75% more misconfigurations** than human-only code
- Security vulnerabilities in AI-generated code are **2.74x higher** incidence rate
- Logic errors — including incorrect dependencies, flawed control flow, and subtle bugs — appear at elevated rates

**Why this matters at scale:** If developers push 100 AI-assisted commits per week and 25% contain errors that must be caught later, the debugging and review overhead often exceeds the speed gain. Amazon's internal experience confirms this: the Guardian (March 11, 2026) quoted a developer saying she "mostly fixes what AI breaks" — spending more time correcting Kiro's "sloppy code" than if she'd written it herself.

**The 90-day Amazon reset in context:** Amazon's emergency lockdown — requiring manager sign-off before deploying any AI-generated code, even from senior engineers — is now positioned as the correct institutional response to a known-quantified failure rate, not an overreaction.

**Vibe coding risk:** The research raises fundamental questions about "vibe coding" (shipping AI-generated code without review), which is increasingly common in startup and indie development. At a 25% error rate on structured tasks, unreviewed vibe-coded apps are shipping with significant bug densities.

**Source:** TechXplore, Study Finds, Wikipedia (vibe coding), CodeRabbit analysis — March 17, 2026

---

### 🔴 Amazon Kiro: Workers "Mostly Fix What AI Breaks" — Guardian Investigation — March 11, 2026

**What happened:** The Guardian published a major investigation (March 11, 2026) into Amazon's forced AI adoption, featuring accounts from Amazon software engineers using Kiro — the company's internal AI coding tool. The picture is damning:

**Developer testimony:**
- "The internal AI tool she's expected to use, called Kiro, frequently hallucinates and generates flawed code"
- Developers describe having to "dig through and correct the sloppy code it creates, or just revert all changes and start again"
- The net effect: **AI creates more work than it saves** for many engineers who must now also be AI babysitters
- Amazon has nonetheless doubled down, requiring AI use as a performance metric

**The mandate problem:** Amazon's AI usage is reportedly tracked in performance reviews, creating perverse incentives — engineers use Kiro to hit AI adoption metrics even when it slows them down, then spend unpaid time cleaning up the resulting mess.

**March 14 formal response:** Amazon implemented a **90-day code safety reset** (per Legal Insurrection, March 14, 2026):
- All code — AI-generated or not — requires additional human review before deployment
- Even senior engineers need manager sign-off
- Engineers called to a mandatory meeting March 10 to review AI-caused incidents
- Internal documents describe a need to "invest in control plane safety" after AI tools exposed "sharp edges where guardrails do not exist"

**The broader lesson:** This is the clearest documented case yet of an organisation discovering that **forced AI adoption without proper guardrails creates net negative productivity** — and the regulatory/safety reset that follows.

**Source:** The Guardian (March 11), Business Insider (March 11), Legal Insurrection (March 14), TechRadar (March 10), FinTech Weekly (March 13) — 2026

---

### 🟠 Windsurf Ownership Chaos — $3B Deal Collapse, CEO Poached, Cognition Acquisition — 2025–2026

**What happened:** Windsurf (originally built by Codeium) experienced one of the most chaotic acquisition sagas in AI tool history, leaving users with deep uncertainty about the product's future.

**Timeline:**
- **May 2025:** OpenAI announces a $3 billion deal to acquire Windsurf — one of the largest AI tool acquisitions ever announced
- **Mid-2025:** As acquisition news circulates, **Anthropic cuts off Windsurf's access to Claude** — the model that powered much of Windsurf's best performance. A subsequent "net neutrality for AI" report cited this as a case study for model access weaponisation
- **July 2025:** Microsoft blocks the OpenAI-Windsurf acquisition; the $3B deal collapses
- **July 2025 (same period):** Google's DeepMind poaches CEO **Varun Mohan** and key R&D staff in what is reportedly a $2.4B talent acquisition
- **Post-collapse:** Cognition AI (makers of autonomous agent Devin) acquires Windsurf for **$250 million** — picking up the product, brand, and 210 remaining employees
- **Feb–March 2026:** Windsurf ranks #1 in the LogRocket AI Dev Tool Power Rankings, ahead of Cursor and Copilot — the product still works, but users are asking about the roadmap

**The ongoing problems for users:**
1. **Roadmap uncertainty:** Cognition's core product is Devin (an autonomous AI engineer). What does Windsurf become under Cognition ownership? No clear answer has been given
2. **Credit-based pricing concerns:** The post-acquisition pricing model is opaque; users evaluating Windsurf alternatives cite "credit-based pricing concerns" and "ecosystem lock-in" as reasons to move
3. **Model dependency questions:** With Anthropic having cut off Claude access once before, Windsurf users wonder whether model access instability is a permanent risk
4. **Key talent gone:** The technical leadership that built Windsurf is now at Google/DeepMind — what does the engineering bench look like under Cognition?

**What it means for the market:** The Windsurf saga illustrates how AI coding tools are subject to forces entirely outside user control — acquisition deals, competitor pressure on model providers, corporate poaching. A tool you rely on can fundamentally change ownership and capability within months.

**Current status:** Product functioning; Cognition has not articulated a public product roadmap for Windsurf post-acquisition.

**Sources:** buildmvpfast.com, morphllm.com, awesomeagents.ai, Business Insider, TechXplore, dupple.com — multiple dates July 2025–March 2026

---

### 🟠 Claude Code Dispatch Silent Failure — Responses Generated but Never Delivered — March 29, 2026

**What happened:** Claude Desktop release 1.1.9310 (shipped approximately March 28) introduced a critical regression in the **Dispatch orchestrator**: messages sent to Dispatch agents are received, processed, and internally logged — but **responses never appear in the conversation UI** on desktop or mobile. The bug was confirmed by Anthropic's status page at 00:53 UTC on March 29, 2026, and resolved same day.

**Technical detail (from GitHub issues #40178, #40179, #40257):**
- Responses are generated and visible in `audit.jsonl` logs — the AI did its work
- The response is never "delivered" to the client — whether Claude Desktop or Claude mobile app
- Example from Issue #40178: "Tutto funziona! Sono qui e pronto." was generated but never shown to the user
- Affected mode: Dispatch orchestrator + Cowork; standard Cowork sessions unaffected
- A Reddit thread "Claude Dispatch won't send me messages back" confirmed widespread user impact the same day

**Why this matters for coding tool users:** Dispatch is the async agent system in Claude Code — developers send coding tasks to agents and receive asynchronous responses. A **silent failure** where the agent appears to be running but delivers nothing is particularly dangerous: users may assume tasks are in-progress when the pipeline is broken, potentially for hours. It erodes trust in autonomous coding agent workflows precisely as they're being adopted at scale.

**Pattern context:** IsDown.app has now tracked **613 Anthropic incidents since June 2024** — a remarkable number that speaks to systemic reliability issues in Claude's infrastructure. This Dispatch bug represents a regression introduced by a recent release, suggesting insufficient regression testing in Claude Code's release process.

**Source:** status.claude.com, GitHub anthropics/claude-code #40178, #40179, #40257, Reddit r/ClaudeAI — March 29, 2026
