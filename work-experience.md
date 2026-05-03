# Work Experience — Detailed

> The long-form version. `resume.md` has the trimmed bullets; this file has the full story for each role.

## Shipsy — Software Engineer
*April 2024 – Present · Gurgaon, India*

### Context
Shipsy is an enterprise logistics SaaS platform serving 100+ enterprise clients across multiple regions. The platform handles pickup scheduling, integrations with logistics partners, and configuration tooling for client onboarding. I work as a full-stack engineer across MongoDB, NestJS, and React, and I own features end-to-end from spec through production.

### What I'm responsible for
- Designing and shipping full-stack features across the order-management and integrations stack
- Owning automation, webhook, and configuration systems used across 100+ enterprise accounts
- Cross-team collaboration with ops, support, and partner-engineering teams to reduce manual workload and integration friction

### Notable wins

- **Pickup Scheduling System (90% reduction in manual ops):** Architected an end-to-end pickup-scheduling system with weekly pre-scheduling, nightly cron automation, and idempotent retry queues. Drove scheduling errors to near-zero across 100+ client accounts. Stack: MongoDB, NestJS, React.

- **AppFlowConfigV2 with LLM auto-config (release cycle: weeks → days):** Rebuilt the configuration platform in TypeScript/React, including an LLM-powered auto-config bot, modular schema validation, and live-preview tooling. Outcome: 70% fewer misconfigurations, 40% greater platform flexibility, and dramatically faster client onboarding across multiple regions. Trimmed configuration hand-offs between engineering and ops.

- **Multi-level webhook infrastructure (60% drop in integration failures):** Built a three-tier webhook system (task / client / customer) with exponential-backoff retry, dead-letter queues, and a real-time React observability dashboard. Hardened data-sync with logistics partners.

- **Enterprise auth — RBAC, SSO, 2FA (50% faster onboarding, zero post-launch incidents):** Designed RBAC data models, REST APIs, and React flows for vendor CRUD, SSO, and 2FA. Took enterprise security from zero to production with audit logging and policy-based access controls.

- **Integration marketplace (~30% drop in inbound ops tickets):** Led the full-stack rollout of an integration marketplace including webhook logs UI, AWB search, invoice filtering, and pickup-edit flow across 5+ microservices. Delivered self-serve tooling, RBAC-gated controls, and audit trails. Sustained 99.9% data-sync reliability across 100+ enterprise accounts.

### Things I've learned
[FILL IN — Honest reflections. Useful for "tell me about a time you failed" or growth-mindset questions. Tell me 1–2 things and I'll write this up cleanly.]

---

## Maximl — Software Development Engineer Intern
*January 2024 – March 2024*

### Context
Maximl is a connected-frontline operations platform with multi-tenant deployments across industrial clients. I joined as an SDE intern on the LLM-product side, focused on integrating LLMs into employee-training and engagement workflows.

### What I was responsible for
- Integrating LLM functionality into existing training products
- Building evaluation and measurement pipelines for LLM output quality

### Notable wins

- **LLM integration for training cohorts (40% engagement uplift, 25% higher comprehension):** Integrated Llama 2 via REST API and prompt tuning to generate context-aware, role-specific responses across PID training cohorts and multi-tenant deployments.

- **A/B testing & feedback pipeline (~20% prompt-accuracy lift):** Built A/B testing and user-feedback evaluation pipelines across 3 product teams. Measured LLM response relevance, logged telemetry, and systematically refined production prompts against golden-set benchmarks.

### Why I left
[FILL IN — internship ended naturally / kept professional answer for "why did you transition to Shipsy"]

---

## Amazon — Mentee, Amazon ML Summer School
*September 2023 – October 2023 · Remote*

### Context
Amazon's invite-only ML Summer School is a structured program where Amazon scientists deliver coursework on classical and modern ML. I was selected as a mentee for the 2023 cohort.

### What I did
- [FILL IN — list 1–2 topics covered (supervised learning, deep learning, NLP, RL, etc.)]
- [FILL IN — any project / capstone work or acknowledgment letter received]

### Why this matters
[FILL IN — One sentence on why this is on the resume — e.g., signals selectivity, formal ML grounding to complement the production LLM work at Maximl/Shipsy.]

---

## TheRightDoctors — Software Development Intern
*February 2023 – June 2023 · Hyderabad, India · Remote*

### Context
[FILL IN — One paragraph: what TheRightDoctors does, who their users are, and which team / problem area you joined.]

### What I built
- [FILL IN — Headline shipped feature: stack, scope, and impact]
- [FILL IN — Optional second item]

### Things I learned
[FILL IN — 1–2 sentences. Optional but useful for behavioral interviews.]

---

## LOKAL Entrepreneurs Empowerment — Software Development Intern
*October 2022 – January 2023 · Delhi, India · Remote*

### Context
[FILL IN — One paragraph: what LOKAL does and which team / problem area you joined.]

### What I built
- [FILL IN — Headline shipped feature: stack, scope, and impact]
- [FILL IN — Optional second item]

### Things I learned
[FILL IN — 1–2 sentences.]

---

## Kalvium — Web Development Intern
*June 2022 – August 2022 · Bengaluru, India · Remote*

### Context
[FILL IN — One paragraph: what Kalvium does and what team / project you joined.]

### What I built
- [FILL IN — Headline shipped feature: stack, scope, and impact]
- [FILL IN — Optional second item]

### Things I learned
[FILL IN — 1–2 sentences.]

---

## STAR-format stories (interview-ready)

> Pre-baked behavioral interview answers. Each follows: Situation → Task → Action → Result.

### Story: A time I led a project end-to-end
**Situation:** Shipsy had 100+ enterprise accounts where pickup scheduling was almost entirely manual, leading to scheduling errors and ops overhead.
**Task:** I was asked to design and ship an automated end-to-end scheduling system.
**Action:** I architected the system on MongoDB / NestJS / React, designed a weekly pre-scheduling layer, built nightly cron automation, and implemented idempotent retry queues to handle partial failures safely.
**Result:** 90% reduction in manual operations and scheduling errors driven to near-zero across 100+ accounts.

### Story: A conflict I navigated
[FILL IN — Tell me about a time you disagreed with a teammate or PM. Give me bullets, I'll write the STAR version.]

### Story: A failure and what I learned
[FILL IN — A time something didn't go as planned. Bullets are fine.]

### Story: A time I influenced without authority
[FILL IN — Useful for senior-IC interviews.]

### Story: A technically hardest problem I solved
**Situation:** AppFlowConfigV2 needed to support drastically faster client onboarding without sacrificing safety — misconfigurations were costing the company multiple hours of engineering time per client.
**Task:** Rebuild the configuration platform such that ops could self-serve safely, with engineers only needed for genuinely novel cases.
**Action:** I architected the rewrite in TypeScript/React, designed modular schema validation, built live-preview tooling so config changes could be visually previewed before commit, and integrated an LLM-powered auto-config bot for the long tail of standard configurations.
**Result:** 70% fewer misconfigurations, 40% greater platform flexibility, release cycle compressed from weeks to days.

### Story: A time I mentored or taught
**Situation:** As Coding Club Mentor at IIIT Kottayam (2023–24), I was responsible for technical onboarding and growth across 200+ students in 4 batches.
**Task:** Build a sustained tech-talk and workshop program covering DSA and full-stack web dev.
**Action:** Led DSA and web-dev talks across 4 batches, hosted 5+ React/Node.js/Git workshops, mentored 15+ juniors on their full-stack projects, and judged competitive programming contests.
**Result:** Sustained engagement with 200+ students; multiple mentees shipped working projects, including some that went into production.
