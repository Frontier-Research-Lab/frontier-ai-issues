# coding-tools — AI Issues Radar

_Last updated: 2026-03-22_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 0a | 🔴 Critical | Cursor caught reselling Chinese Kimi K2.5 as in-house "Composer 2" — developer exposes model ID in API response; Cursor admits while citing "legal obligation not to disclose"; geopolitical + trust fallout (March 19, 2026) | Cursor / Kimi K2.5 | Active (March 19, 2026) |
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
