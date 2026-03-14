# coding-tools — AI Issues Radar

_Last updated: 2026-03-14_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 1 | 🔴 Critical | Amazon's AI coding mandate caused 6.3M lost orders + 90-day safety reset — Kiro & Q implicated in multiple Sev-1 outages | Kiro / Amazon Q | Active |
| 2 | 🔴 Critical | Fake AI browser extensions stolen ChatGPT/DeepSeek conversations from 900K users across 20K enterprises — "full chat exfiltration" | Chrome/Edge extensions | Active |
| 3 | 🔴 Critical | AI coding tools introduce security flaws in 87% of pull requests — cross-site scripting had 86% failure rate | All AI coding tools | Ongoing |
| 4 | 🔴 Critical | Malicious Rust crates exploit AI coding assistants — injected code uses Claude, Copilot, Gemini, Kiro to exfiltrate secrets | Claude Code / Copilot / Gemini / Kiro | Active |
| 5 | 🟠 Major | Developer trust in AI code accuracy at historic low — 46% distrust vs 33% trust (Stack Overflow Feb 2026) | All AI coding tools | Ongoing |
| 6 | 🟠 Major | Cursor: surprise pricing overages, crashes, file-saving failures, AI modifying wrong files without permission | Cursor | Ongoing |
| 7 | 🟠 Major | GitHub Copilot: suggests code with subtle bugs, outdated APIs, and security flaws that look correct at a glance | GitHub Copilot | Ongoing |
| 8 | 🟡 Notable | Privacy concerns — code sent to third-party APIs without explicit disclosure; vendor lock-in across all tools | Cursor, Copilot, Windsurf | Ongoing |

---

## Details

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
