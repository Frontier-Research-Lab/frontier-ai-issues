# automation — AI Issues Radar

_Last updated: 2026-03-28_

## Top Issues

| # | Severity | Issue | Affected Tool | Status |
|---|----------|-------|---------------|--------|
| 0mar28 | 🔴 Critical | **LiteLLM supply chain attack — poisoned PyPI packages exfiltrate cloud secrets** — threat actor "TeamPCP" published backdoored LiteLLM versions 1.82.7 and 1.82.8 on March 24 via compromised Trivy CI/CD credentials; malware uses .pth file that auto-executes on Python startup (runs even without importing LiteLLM); harvests API keys, OAuth tokens, environment variables and sends to attacker; available for ~6 hours before removal; Kaspersky, Snyk, Arctic Wolf all confirmed; any automation pipeline that ran `pip install litellm` on March 24 should be treated as compromised | LiteLLM (AI automation dependency) | **Active — audit all installs from March 24** |
| 0NEW | 🔴 Critical | **NEW n8n RCE triple: CVE-2026-33660, CVE-2026-33696, CVE-2026-33663** — two new CVSS 9.4 RCE vulnerabilities published March 25: CVE-2026-33660 allows RCE through Merge node SQL mode (AlaSQL); CVE-2026-33696 achieves RCE through prototype pollution; CVE-2026-33663 allows credential interception. Patch to versions 1.123.27, 2.13.3, or 2.14.1 immediately — coming just weeks after "Ni8mare" exploit chain | n8n | **Active — patch to 1.123.27/2.13.3/2.14.1** (March 25, 2026) |
| 0 | 🔴 Critical | "Ni8mare" — CISA warns n8n max-severity CVE chain being actively exploited in wild: CVE-2026-21858 (unauthenticated file read) + CVE-2025-68613 (authenticated RCE) combined = full system takeover without login; n8n stores API keys, OAuth tokens for dozens of services (March 17, 2026) | n8n | Active exploit — patch NOW |
| 1 | 🔴 Critical | Zapier pricing rage — what started at $10/month has ballooned to $750+/month for basic automations; mass migration underway | Zapier | Ongoing |
| 2 | 🔴 Critical | "$40K/year Zapier lesson" — viral Reddit post documents company that burned $40K/yr on simple automations, now migrating entire stack | Zapier | Active (March 2026) |
| 3 | 🟠 Major | "Zapier Tax" — per-task pricing model penalises growth, destroying SaaS margins as automation volume scales | Zapier | Ongoing |
| 4 | 🟠 Major | AI agent workflow steps are Zapier's most expensive per-task items — AI-powered automations cost 5–10x more than traditional steps | Zapier / Make | Active |
| 5 | 🟠 Major | Make (formerly Integromat) — steep learning curve and performance slowdowns with heavy data volumes | Make | Ongoing |
| 6 | 🟡 Notable | n8n self-hosted maintenance burden; requires engineering resources most target users don't have | n8n | Ongoing |
| 7 | 🟠 Major | Make (Integromat) support response crisis — tickets taking days to resolve; critical business automation failures have no fast recovery path | Make | Ongoing (March 2026) |

---

## Details

### 🔴 LiteLLM Supply Chain Attack — TeamPCP Poisons PyPI Package, Cloud Secrets at Risk — March 24, 2026

**What happened:** On March 24, 2026, threat actor **TeamPCP** published two backdoored versions of the `litellm` Python package (**1.82.7** and **1.82.8**) to PyPI — the primary repository used by Python developers to install packages. The attack exploited a **compromised Trivy GitHub Action** in LiteLLM's own CI/CD pipeline to steal PyPI publishing credentials, then used them to push malicious versions.

**Why this is critical for AI automation:** LiteLLM is one of the most widely-used Python libraries in the AI ecosystem. It acts as a universal API gateway — allowing developers to route calls to OpenAI, Anthropic, Gemini, Cohere, and dozens of other LLMs through a single interface. It is embedded in countless AI automation pipelines, n8n deployments, Make/Zapier alternatives, and custom agent frameworks.

**The attack mechanism — .pth file:**
- The malware was delivered via a **`.pth` file** (Python path file)
- `.pth` files execute automatically when the Python interpreter starts — meaning the payload runs in **any Python process** on the infected machine
- The malware does NOT need to be explicitly imported to run — **simply having litellm installed is enough**
- The payload harvests: API keys, OAuth tokens, cloud credentials, environment variables, and other secrets

**Timeline:**
- **March 24, 2026:** TeamPCP publishes 1.82.7 and 1.82.8 to PyPI
- **~6 hours later:** Packages removed from PyPI after detection
- **March 25–26:** Kaspersky, Snyk, Arctic Wolf publish analyses
- **March 27:** LiteLLM publishes security advisory + SHA-256 checksums for verified-safe versions

**Who is affected:** Any developer or automation pipeline that ran `pip install litellm` or `pip install --upgrade litellm` during the ~6 hour window on March 24. CI/CD systems that automatically update dependencies are most at risk.

**Immediate actions required:**
1. Run `pip show litellm` — if you see 1.82.7 or 1.82.8, you're compromised
2. Check for `litellm_init.pth` files: `find ~/.cache/uv -name "litellm_init.pth"` 
3. Rotate ALL credentials in environments where litellm was installed
4. Audit CI/CD runs from March 24

**Snyk:** *"On March 24, 2026, threat actor known as TeamPCP published backdoored versions of the litellm Python package after stealing PyPI credentials via a compromised Trivy GitHub Action in LiteLLM's CI/CD pipeline."*

**Sources:** Snyk (March 23), Arctic Wolf (March 25), Kaspersky blog (March 26), LiteLLM security advisory (March 27), Forbes (March 27)

---

### 🔴 New n8n Triple Vulnerability — RCE + Credential Theft CVEs — March 25, 2026

**What happened:** The n8n team published **three new security advisories** on March 25, 2026 — just eight days after the "Ni8mare" exploit chain entered CISA's KEV catalogue. This new batch includes two **remote code execution (RCE) vulnerabilities** and one **credential interception** vulnerability:

**CVE-2026-33660 — RCE via Merge Node SQL Mode (AlaSQL)**
- **CVSS 4.0 score: 9.4** (Critical)
- The Merge node's SQL mode in n8n allows user-controlled SQL queries via **AlaSQL**. AlaSQL is a JavaScript SQL library that executes in-process — meaning a crafted SQL payload can escape the query context and execute arbitrary JavaScript
- Attack vector: any workflow that uses the Merge node with SQL mode enabled
- Affected users: anyone running n8n with complex data transformation workflows

**CVE-2026-33696 — RCE via Prototype Pollution**
- **CVSS 4.0 score: 9.4** (Critical)
- A prototype pollution vulnerability in n8n's workflow data handling allows attackers to inject properties into JavaScript's base Object prototype
- Once the prototype is polluted, subsequent property access can trigger malicious code execution
- Attack vector: crafted workflow data or injected node inputs

**CVE-2026-33663 — Credential Interception**
- Rated "high" severity
- Allows an authenticated attacker to intercept unencrypted credentials stored in n8n's credential vault
- Particularly dangerous given n8n's design as a credential aggregator for dozens of external services

**What you need to do:** Patch immediately to:
- `1.123.27` (stable)
- `2.13.3` or `2.14.1` (next track)

**The pattern:** n8n has now had at least **5 critical+ CVEs in March 2026 alone**. Per Heise: *"In the recent past, the developers have released security updates for n8n twice a month."* This pace of critical security releases signals a systemic security debt in the codebase — not isolated bugs. For organisations running n8n with admin access to production credentials, the risk posture is now severe.

**Sources:** anonhaven.com (CVE detail, March 26), Heise Online (March 26), n8n security advisories (March 25)

---

### 🔴 "Ni8mare" — CISA Warns n8n Critical CVE Chain Actively Exploited — March 17, 2026

**What happened:** CISA added two chained n8n vulnerabilities to its **Known Exploited Vulnerabilities (KEV) catalogue** on March 17, 2026, confirming active exploitation in the wild. The "Ni8mare" attack chain — named by researchers — combines two CVEs to achieve **full system takeover without authentication**:

**The two CVEs chained:**
1. **CVE-2026-21858** (max/critical severity) — An unauthenticated file read vulnerability in n8n, caused by improper handling of webhooks. An attacker can read internal files (including credential storage) **without logging in**. CVSS score 9.9.
2. **CVE-2025-68613** (critical, authenticated RCE) — Remote Code Execution via improper isolation of workflow expressions from the Node.js runtime. User-controlled input can execute arbitrary code with n8n process privileges.

**The chain in practice:** Attackers use CVE-2026-21858 to read n8n's credential files unauthenticated → extract legitimate user credentials → use those credentials to trigger CVE-2025-68613's RCE → full control of the n8n host system.

**Why this is uniquely catastrophic for automation users:**

n8n is routinely used as a central automation hub and credential store. A typical self-hosted n8n instance stores:
- API keys for cloud services (AWS, GCP, Azure)
- OAuth tokens for Google Workspace, Microsoft 365, Slack
- Database credentials (PostgreSQL, MySQL, MongoDB)
- CRM tokens (Salesforce, HubSpot)
- Communication service credentials (Twilio, SendGrid)
- Payment API keys (Stripe, PayPal)

Compromising an n8n instance typically means **instant access to every third-party service the automation stack touches** — the blast radius is the entire company's connected infrastructure.

**CISA's specific warning:** "One n8n server could expose your entire digital ecosystem." ClearanceJobs (March 17): "This cycle of incomplete patching is particularly dangerous for automation tools that serve as a central repository for sensitive API keys and OAuth tokens across the Enterprise."

**Scale of exposure:** n8n has hundreds of thousands of self-hosted instances globally, used by agencies, startups, and enterprises. The self-hosted nature means patching rates are slower than cloud-managed tools — many instances run outdated versions indefinitely.

**Current status:** A patch has been released. CISA's inclusion in KEV means US federal agencies must patch within 3 weeks; private sector is strongly advised to treat this as P0. Organisations still running n8n below the patched version are actively being targeted.

**Community reaction:** The disclosure landed in the middle of n8n being recommended as the primary Zapier/Make escape valve for cost-conscious automation users. The irony is sharp: users fleeing Zapier's pricing landmine ran into n8n's security landmine.

**Source:** CISA KEV, Dataminr, LinuxSecurity, SecurifyAI, RedPacket Security, ClearanceJobs — March 14–17, 2026

---

### 🔴 Zapier Pricing Explosion — $10/month → $750+/month

**What happened:** A October 2025 Reddit post — "TIRED OF ZAPIER" — encapsulated a community boiling point. Long-time Zapier users report their costs have exploded from an accessible entry price to **over $750/month for basic automations** that haven't fundamentally changed. The root cause is Zapier's **per-task pricing model**: every step in every Zap counts as a billable task. As businesses grow and automate more, costs compound rapidly.

**The March 2026 Reddit verdict** (r/automation "Honest Review: Which automation tool is actually worth it in 2026?"):
- **Zapier**: "Still the easiest for simple API-to-API stuff. But the cost per task is insane once you scale."
- **The brutal summary**: "Zapier and Make are the most successful scams in SaaS history. They charge you per 'task' for literally moving data between two APIs — something that costs fractions of a cent in compute."

**Scale of impact:** This is not a niche complaint. Zapier is one of the most widely-used business automation tools globally. The pricing structure actively penalises successful users — the more you automate (and presumably the more value you get), the more you pay.

**The "Zapier Tax" concept** (from r/SaaS, March 2026): By 2026, the term "zapier tax" has entered the SaaS vocabulary. It describes the phenomenon where a growing company's automation costs balloon faster than their revenue, because Zapier's per-task model means you are "literally being penalized for your own growth."

**Community migration:** Users are moving to n8n (self-hosted, no per-task fees) and Make as alternatives, despite both having significant drawbacks (see below).

**Source:** Reddit r/automation, Reddit r/zapier, Reddit r/SaaS — October 2025–March 2026

---

### 🟠 Make (Integromat) — Learning Curve and Slow Performance

**What happened:** Make is the most-recommended Zapier alternative for users who need visual workflow control. However, it has consistent complaints:
- **Steep learning curve** — the visual interface is powerful but non-obvious; new users frequently get stuck
- **Performance slowdowns with heavy data** — workflows processing large volumes of data run slowly
- **Hidden costs** — like Zapier, costs escalate with volume (though generally more slowly)

**Community reaction:** Make is frequently described as "better than Zapier but still frustrating." It captures users fleeing Zapier's pricing but doesn't satisfy users who want simple, fast, cheap automation.

**Source:** Reddit r/automation, Reddit r/SaaS — 2026

---

### 🟡 n8n — Self-Hosted Maintenance Burden

**What happened:** n8n (open-source, self-hosted workflow automation) is the main "escape hatch" from Zapier/Make's pricing. Zero per-task fees. But it comes with a significant trade-off: **it requires infrastructure knowledge to run, maintain, and update**. For the typical SMB owner who just wants their CRM to talk to their email tool, spinning up and managing an n8n instance is a non-starter.

**The paradox:** The users most burned by Zapier's pricing are often small businesses with low technical capacity — exactly the users who can't operationalise n8n without hiring a developer to do it.

**n8n Cloud** (the managed version) addresses the maintenance issue but reintroduces pricing pressure — users on the cloud version are paying again, reducing the cost advantage.

**Source:** Reddit r/SaaS, hatchworks.com — 2026

---

### 🔴 "$40K/Year Zapier Lesson" — Viral Reddit Post — March 2026

**What happened:** A Reddit post in r/SaaS (March 2026) titled "We Burned $40K/Year on Zapier Before We Finally Woke Up" went viral in the automation and SaaS communities. The poster described a company that had gradually scaled Zapier usage over three years, adding integrations as the business grew, until they opened an annual bill and discovered they'd been paying over $40,000 per year — for automations that move data between APIs in tasks that cost fractions of a cent in actual compute.

**The community reaction:** The post resonated strongly because it's not an edge case. The Zapier pricing model is specifically designed to be invisible at small scale (the "gateway drug" of free/cheap entry tiers) and catastrophic at medium scale. The per-task pricing means costs compound quietly month-over-month as businesses grow.

**The specific pain points documented:**
- Zapier AI steps (LLM-powered workflow actions) cost 5–10x more per execution than standard API-to-API steps
- A workflow that was $50/month in 2022 cost $600/month in 2025 after the AI steps migration
- No cap on monthly spending — the bill arrives after the damage is done
- Cancelling means rebuilding every integration from scratch

**Migration horror:** The poster spent 6 months rebuilding their entire automation stack in n8n self-hosted after the discovery. "We gained our sanity back, but lost six months of engineering time. The ROI math doesn't work either way."

**Source:** Reddit r/SaaS — March 2026

---

### 🟠 AI Agent Steps Are Zapier's Most Expensive Items

**What happened:** As Zapier and Make introduced AI-powered steps (LLM calls, AI classification, intelligent routing), they priced them at a significant premium over standard trigger-action steps. In Zapier's task billing model:
- Standard steps (e.g., send Slack message, update Airtable row): 1 task
- AI steps (e.g., classify with ChatGPT, summarise email): 5–10 tasks per execution

A workflow that previously cost 1,000 tasks/month becomes 5,000–10,000 tasks/month when AI steps are added — pushing users from the Professional plan ($30/month) into the Teams tier ($100+/month) immediately.

**Why this matters:** AI automation is the stated future of the category. If the pricing model makes AI steps unaffordable for SMBs, the companies that need AI automation most (lean teams, small businesses) are priced out. The large enterprises that can afford it don't need the cost savings as urgently.

**Community verdict (r/automation, March 2026):** "Zapier's AI steps are a trap. They get you hooked on automating with AI during the free trial, then the bill comes in."

**Source:** Reddit r/automation, Zapier pricing documentation — March 2026

---

**Overall picture for 2026 automation market:**

The space is deeply dysfunctional for mid-market users. Large enterprises use custom solutions. Technical founders self-host n8n. Everyone in between is trapped in Zapier/Make pricing escalation. The emergence of AI agent workflows (LLM-powered steps, not just trigger-action) is adding new complexity without solving the underlying pricing problem — and AI steps are among the most expensive per-task items in Zapier's catalogue.

---

### 🟠 Make (Integromat) Support Response Crisis — Days-Long Wait Times — March 2026

**What happened:** Community analysis published in March 2026 (roborhythms.com, "Zapier Alternatives 2026") specifically flagged **Make's support response time** as a major operational risk: "Support response time is another legitimate complaint about Make. I have seen reports of tickets taking several days to get a response, which matters if something breaks in a business-critical workflow on a Friday afternoon."

**The severity:** Make's visual canvas platform is used by agencies and SMBs for complex, high-stakes automations. When a critical workflow breaks (payment processing, customer onboarding, inventory sync), waiting several days for support is not an option — it represents direct revenue loss.

**Zapier context:** Zapier's per-task pricing makes it unsustainable at scale. Make's lower pricing comes with this support reliability trade-off. Neither platform is reliably solving the mid-market automation problem.

**Community verdict:** "Make is fine when it works — but when it breaks and you're waiting 3 days for support on a business-critical automation, the pricing advantage evaporates."

**Source:** roborhythms.com Zapier Alternatives 2026 analysis — March 2026
