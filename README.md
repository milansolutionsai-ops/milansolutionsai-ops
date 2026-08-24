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

**A member challenge platform for a 170,000-contact subscription business**
Sole designer, engineer and operator. Public bilingual site, membership-gated signup validating against live CRM state, member portal with weekly challenges and evidence uploads and a live leaderboard, an admin console, and the full email journey. **870 participants, 96% profile completion, 3,600+ submissions in the first three weeks, and roughly 80% active-participant retention** from week one to week three.
`Next.js` `React` `TypeScript` `Supabase` `GoHighLevel` `Vercel`

**An attribution-recovery layer for custom-built funnels**
GoHighLevel only attaches native attribution to contacts its own tracking script creates. Build a custom landing page instead of using their builder and every lead loses its first-touch data, permanently, with nothing to tell you it happened. The fix inverts the problem: deliberately lose the create race, let the platform's tracker win, then enrich the record it made. Degrades to an API create on timeout so a lead is never lost, and writes a log line per lead because the failure mode is otherwise invisible.

**A 23-agent autonomous system, running for four months on under $50**
My own operating system: content generation and scheduling, comment drafting with human approval, publishing, intelligence gathering, meeting prep. Scheduled on Postgres cron, executed on serverless, with per-agent token cost written to the database next to latency and status, and a kill switch on every agent so any one can leave production without a deploy. **477 commits, 900+ tests.** About half the fleet is switched off at any time, which is the point.

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
