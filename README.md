# Milan Veljkovikj

**I own the technical layer at companies too small to have one.** CRM and martech engineering, AI automation, and the applications that sit on top of both. Usually as the only technical person in the room.

Currently AI & Automation Architect at [Web My Money](https://webmymoney.com), a bilingual digital marketing agency, where I build and run the systems behind client acquisition, retention and reporting.

---

### What I actually do

**Make platforms do things they don't want to do.** Most of my work lives at the seam between a martech platform, a custom front end, and the data someone needs out of both. That seam is where the interesting failures are: the race conditions, the silent data loss, the attribution that vanishes without telling anyone.

**Build and operate AI systems that stay cheap.** Not demos. Scheduled agents that run unattended for months, with per-call cost attribution and kill switches, because the question that matters isn't whether an agent works, it's whether it quietly bankrupts you.

**Ship whole products alone.** Design, frontend, backend, database, CRM integration, email infrastructure and deliverability, as one person, for real users.

---

### Selected work

**[A member challenge platform for a large subscription business](https://github.com/milansolutionsai-ops/membership-challenge-platform-case-study)**
Sole designer, engineer and operator. Public bilingual site, membership-gated signup validating against live CRM state, member portal with weekly challenges and evidence uploads and a live leaderboard, an admin console, and the full email journey. **870 participants, 96% profile completion, 3,600+ submissions in the first three weeks, and roughly 80% active-participant retention** from week one to week three.
`Next.js` `React` `TypeScript` `Supabase` `GoHighLevel` `Vercel`

**[Keeping GoHighLevel's native attribution on custom-built pages](https://github.com/milansolutionsai-ops/ghl-native-attribution)**
GoHighLevel only attaches native attribution to contacts its own tracking script creates. Build a custom landing page instead of using their builder and every lead loses its first-touch data, permanently, with nothing to tell you it happened. The fix: put a rule-compliant plain HTML form and the platform's own tracker inside an iframe, so a real user submit is a genuine top-level navigation from the tracker's point of view. The platform creates and attributes the contact; the parent app never reloads and enriches the same record by email. Falls back to an API create when the tracker is blocked, which is 15 to 40% of traffic, so a lead is never lost.

**[An internal content platform that removed the developer from every copy change](https://github.com/milansolutionsai-ops/agency-content-studio-case-study)**
Every headline and price on the agency's marketing sites used to be a pull request. Built a slot-based platform where editors fill named slots and cannot restructure a page, with preview-first editing into the real components. The public content API deliberately holds no credentials, because content about to be published is not a secret, and the one genuinely privileged operation (cache invalidation) verifies an Ed25519 signature instead of a shared token. Live; the whole team uses it.
`Next.js` `TypeScript` `Supabase` `Vercel`

**A 23-agent autonomous system, running for four months on under $50**
My own operating system: content generation and scheduling, comment drafting with human approval, publishing, intelligence gathering, meeting prep. Scheduled on Postgres cron, executed on serverless, with per-agent token cost written to the database next to latency and status, and a kill switch on every agent so any one can leave production without a deploy. **477 commits, 900+ tests.** About half the fleet is switched off at any time, which is the point.

---

### Free tools

Things I built for my own work and cleaned up for anyone to use.

**[map: a Claude Code skill that keeps you able to explain your own system](https://github.com/milansolutionsai-ops/claude-code-map-skill)**
After every finished piece of work, Claude posts a 5-line map in the chat: the flow, where it lives, what isn't tested, and a decision only when there's a real one. Plus a one-page map per project that survives context compaction, and a live-checked brief before client calls.

**[claude-code-guardrails: three safety hooks](https://github.com/milansolutionsai-ops/claude-code-guardrails)**
No SQL write without a matching dry run, no risky click in a client's live system without a human, no secrets left in session transcripts. Runs outside the model, so the agent can't forget it or talk past it.

**[scoping-kit: quoting AI-assisted work](https://github.com/milansolutionsai-ops/claude-code-scoping-kit)**
Three Claude Code skills. Every estimate shows the market quote next to your real AI-assisted hours plus a calendar date, a client feature list becomes a verified SOW, and an actuals log retunes the numbers after 3 real jobs.

**[draw-it: one diagram of how a system works](https://github.com/milansolutionsai-ops/claude-code-draw-it)**
Claude reads a codebase and draws one hand-drawn diagram of a single flow: where each piece runs, the steps in order, what costs money per run, and what fails silently.

**[consult: one decision, several AI models](https://github.com/milansolutionsai-ops/claude-code-consult)**
For decisions that are expensive to get wrong: one prompt goes to OpenAI, Gemini and Grok at once, then Claude reports where they agree, where they conflict and what changes the call.

**[session-mesh: Claude sessions that know about each other](https://github.com/milansolutionsai-ops/claude-code-session-mesh)**
Long-running sessions share a registry and a change log, ask each other for context directly, and hand off cleanly to a fresh session.

**[AI visibility self-check](https://github.com/milansolutionsai-ops/ai-visibility-self-check)**
10 checks a business owner can run by hand in about 15 minutes to see whether ChatGPT and Perplexity recommend them, plus a scorecard and a sample report.

**[review-inbox: review your AI's work without reading the chat](https://github.com/milansolutionsai-ops/claude-review-inbox)**
The agent's output lands in a local inbox. You mark it OK or Change with timed notes, and the next Claude turn picks up the feedback by itself, fixes it, and shows a before/after check per note.

**[media-toolkit](https://github.com/milansolutionsai-ops/media-toolkit)**
A full AI video studio for €0 a month, driven by Claude Code on a laptop CPU.

---

### Stack

**Build:** TypeScript, Next.js, React, Node, Tailwind
**Data:** Supabase, PostgreSQL, row-level security, pgvector
**AI:** Claude API, agent orchestration, multi-step pipelines, token cost instrumentation, Vapi and Voiceflow for voice and chat
**Automation:** Make.com (Advanced Certified), n8n, Zapier, Airtable
**CRM and martech:** GoHighLevel, lifecycle and funnel architecture, attribution and conversion tracking, email deliverability (SPF, DKIM, DMARC)
**Ship:** Vercel, GitHub Actions, Playwright, Vitest

---

### Why this profile looks quiet

Most of what I build is private or belongs to clients. The agency work lives in an organization account, the client products are commercial, and my own systems hold personal data. What's here is the small public remainder.

The contribution graph is the honest version.

---

### Elsewhere

**Portfolio and case studies:** https://milan-solutions.vercel.app
**LinkedIn:** https://www.linkedin.com/in/milan-veljkovikj
**Based in** North Macedonia, working remote across European hours.
