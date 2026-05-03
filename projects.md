# Projects

## Flee Outpass Portal

**One-liner:** Full-stack biometric outpass system for a 2,000+ student campus, in production at IIIT Kottayam.
**Stack:** TypeScript, React, Redux, Node.js, Express.js, MongoDB, JWT
**Link:** [outpass.iiitkottayam.ac.in](https://outpass.iiitkottayam.ac.in)
**Status:** Shipped — live in production for 6+ months, used daily for ID-card entry/exit, attendance tracking, and admin controls for 2,000+ users.

**Why I built it:** The campus's existing outpass workflow was paper-based, slow, and error-prone. There was no audit trail, no real-time approval mechanism, and no integration with the campus biometric system.

**What it does:** Students request outpasses through a Redux-powered React frontend; wardens and admins approve via role-based dashboards; the system integrates with biometric ID-card hardware for entry/exit logging and email/SMS gateways for real-time notifications. Every action is audit-logged.

**Hardest part / what I learned:** Designing the RBAC system to handle three user types (student / warden / admin) with overlapping but distinct permission sets, while keeping outpass lookups under 150 ms even at peak concurrent load. I learned a lot about MongoDB indexing strategy, in-memory caching for high-frequency reads, and how much CDN edge caching matters on low-bandwidth campus networks.

**Impact / numbers:**
- 80% faster processing vs. the paper system, zero record-keeping errors
- Sub-second access for 2,000+ concurrent users
- <150 ms outpass lookups
- Officially recognized by the IIIT Kottayam Management Board (honored on-stage)

---

## CardWise

**One-liner:** AI-powered credit card recommendation engine that scores user spending profiles against 100+ card benefits.
**Stack:** React, TypeScript, Node.js, REST APIs, custom recommendation engine
**Link:** [cardwise-delta.vercel.app](https://cardwise-delta.vercel.app)
**Status:** Shipped — live, deployed via Vercel with GitHub Actions CI/CD.

**Why I built it:** Credit card recommendation sites are usually generic top-10 lists. I wanted to build something that actually personalized recommendations to a user's spending pattern across categories like travel, dining, online shopping, etc.

**What it does:** Users describe their spending profile across 10+ categories; the backend runs a multi-dimensional preference-matching algorithm using async parallel scoring against 100+ card benefit profiles, and returns the top-5 personalized matches in under 2 seconds.

**Hardest part / what I learned:** Bundle optimization. The first build was bloated with everything bundled together; getting it down to a fast, accessible, PWA-grade experience while keeping all the functionality required deep work with Webpack Bundle Analyzer, tree-shaking, code splitting, response caching, and Lighthouse-driven CI gating.

**Impact / numbers:**
- Top-5 personalized recommendations in <2 seconds
- 35% smaller bundle, 40% fewer backend calls after optimization
- Lighthouse 95+ scores
- WCAG AA accessibility (semantic HTML, ARIA, keyboard navigation, screen-reader support)
- Rich social previews (Open Graph + meta tags)

---

## Side experiments / academic work

- **Hackathon Winner — Hacktivity, IIIT Kottayam:** 1st place among 95+ teams. The hackathon was where the **Flee Outpass Portal** was originally built end-to-end in 24 hours; the project was then matured and shipped to production over the following months, eventually being adopted by the institute (see the full project write-up above).
