# Portfolio Changes Log

Proof statement: "I'm an Information Science student who builds practical AI-powered and user-focused web solutions."
Primary action: "Connect with me for internship, project, or collaboration opportunities."

---

## v1 — Sitemap draft (pressure-tested)

Initial sitemap: Hero → Work → About → Contact.

**Issues identified:**
- CTA ("Let's Connect") only existed at the very top (Hero) and very bottom (Contact) — no reinforcement mid-scroll.
- About section included generic "interests" content unrelated to the proof statement.
- No skills/tech-stack summary for fast-scanning recruiters.
- No resume/CV path.
- Work section's "outcomes" were vague by default — flagged as a risk, not yet a fix.

---

## v2 — About rewritten

- Rewrote About around three lines, each tied directly to the proof statement:
  - **Who I am** → ties to "AI-powered and user-focused"
  - **What I build** → ties to "practical," grounded in problem types
  - **Current goal** → doubles as a bridge into Contact
- Removed generic "interests" content entirely.

---

## v3 — Sitemap finalized

- Added a **bridge CTA** in Work, right after the case studies — so visitors can act at peak interest instead of waiting through About.
- Added a **skills/tech-stack summary** placeholder in Work.
- Added a **Resume/CV link slot** in Contact.

---

## v4 — First build (real content)

Source: pulled real project/profile data from `github.com/pragnyamehar-create`.

**Content added:**
- Name, college (Dayananda Sagar College of Engineering, 3rd year Information Science & Engineering), email, LinkedIn, GitHub — all real.
- 3 projects pulled from GitHub:
  - **Quiz Craft** — AI quiz generator (Grok API) — flagged as the **flagship AI project**
  - **Eventara** — college event management system (full-stack, no AI)
  - **Findora** — lost & found management system (full-stack, no AI)

**Flag raised:** only 1 of 3 projects is genuinely AI-powered. Discussed three options (lead with Quiz Craft as flagship / find more AI work / soften the proof statement). **Decision: lead with Quiz Craft as flagship AI project, others presented as full-stack proof.**

**Design concept:** library-catalog / index-card motif (ties to Information Science field) — call-number tags per project (`AI.001`, `SYS.002`, `SYS.003`), monospace "ledger" labels, dotted rules, brass/ink color palette instead of a generic dark-mode template.

**Known gaps at this stage:**
- No real outcome metrics — outcome/impact lines are honest but soft (no fabricated numbers).
- No resume/CV link (none provided yet).
- Skills/stack summary existed in Hero and About, but **not** as its own scannable block inside Work.

---

## v5 — Gaps fixed + interactivity added

**Fixes:**
1. Added a **clickable skills bar** to the top of Work: `All / JavaScript / Node.js / AI-LLM APIs / MySQL / Auth`. Clicking a chip dims every project card that doesn't use that skill — filtering is functional, not just a static tag list.
2. Tagged each project with `data-skills` so filtering works:
   - Quiz Craft → `js, node, ai`
   - Eventara → `js, sql, auth`
   - Findora → `js, sql`
3. Resume: still not added live (no link/file provided). Added as a **commented-out 4th Contact tile**, ready to activate on request — Contact currently shows 3 tiles only.

**New interactivity:**
- **Scroll-reveal** — flagship card, project cards, connect-bridge, about grid, and contact links fade/slide into view on scroll. Disabled automatically if the visitor has `prefers-reduced-motion` on.
- **Scroll progress rail** — thin brass line at the top of the page tracking scroll position.
- **Copy-email button** — one-click copy of email address under the Contact email tile, with a "Copied ✓" confirmation state.

**Unchanged in this pass:** hero copy, about copy, project descriptions/outcomes, color palette, typography, layout structure.

---

## Open items (not yet resolved)

- [ ] Real outcome metrics or testimonials for Quiz Craft / Eventara / Findora (currently descriptive, not evidenced with numbers or quotes).
- [ ] Resume/CV link or file — needed to activate the 4th Contact tile.
- [ ] Judgment call: is the skills-filter interaction useful to a fast-skimming recruiter, or does it add friction versus just reading the stack flat? Not yet decided.
