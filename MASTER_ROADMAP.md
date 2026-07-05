# Master Roadmap

Internal planning document for Alexander Roman's developer career and Roman
Creative Studio's growth. Not linked from the live site — this is a
reference for staying organized, not visitor-facing content.

Status is reported honestly below, including the parts that were planned
but never actually built.

---

## Phase 1 — Resume & Foundation

**Status: Complete**

- `resume.html` — printable master resume with achievement-oriented bullets
  for Roman Creative Studio and 4Kingdom Podcast, a Print/Save-as-PDF
  button, and ATS-readable structure.
- Bracketed placeholders (`[Add phone]`, `[Add GitHub URL]`, `[Add LinkedIn
  URL]`, `[Add city, state]`) still need to be filled in before sending
  this resume to recruiters — search the file for `[Add`.
- Shared design system (`css/style.css`, `js/main.js`) that every later
  page builds on.

## Phase 2 — Portfolio & Case Studies

**Status: Complete**

- `index.html` — hero, project grid, About preview, contact section.
- `about.html` — full narrative bio.
- Two full case studies (`projects/roman-creative-studio.html`,
  `projects/4kingdom-podcast.html`), each covering all 18 sections:
  Overview, Problem, Goals, Research, Planning, Design Decisions, Solution,
  Technologies, Architecture, Challenges, Trade-offs, Accessibility,
  Responsive Approach, Performance, Testing, What I Learned, Future
  Improvements, Screenshots.
- Verified in a headless browser: no console errors, mobile nav works, and
  content stays visible with JavaScript disabled (a real bug was caught
  and fixed here — see the Architecture/Testing sections of either case
  study for the honest account).

## Phase 3 — Professional Presence

**Status: Complete**, except one item blocked on missing information.

Done:
- Case-study depth expansion (the 18-section structure above).
- **SEO pass**: canonical URLs, Open Graph + Twitter Card tags, and
  JSON-LD structured data on every page; a generated `og-cover.png`
  (`assets/images/`); `sitemap.xml` and `robots.txt` at the repo root.
  Uses `https://alexanderroman.dev` as a placeholder domain throughout —
  replace with the real deployed domain once one exists.
- **Real accessibility + performance audit**: ran actual Lighthouse
  audits (not estimates) against every page. Found and fixed three real
  issues — insufficient color contrast on muted text (`--text-tertiary`
  token, plus two component-specific colors), a heading-order skip
  (`h4` used without an `h3` ancestor), and a missing `<main>` landmark
  on every page. Before: 89 accessibility (home), 100/100/100 elsewhere.
  After: **100 performance / 100 accessibility / 100 best practices / 100
  SEO on all five pages**, re-verified with a fresh Lighthouse run plus a
  full functional re-check (no console errors, mobile nav intact, no
  visual regression).
- **Resume ATS refinement**: expanded the Skills line with true keyword
  synonyms (DOM Manipulation, Web Accessibility (WCAG), Version Control
  (Git & GitHub), Cross-Browser Compatibility, Static Site Deployment)
  without touching any bullet Phase 4.5 references.
- **LinkedIn content**: [headline, About, experience, skills, and featured
  projects](https://claude.ai/code/artifact/055489d9-bcbe-412a-8a50-f04e00aac535),
  plus a real generated 1584×396 banner image (sent as a file, laid out to
  clear the profile-photo overlap zone).

**Still blocked:**
- GitHub profile README (`<username>/<username>` repo) — needs your
  actual GitHub username before it can be created.

Say the word and any of these can be picked up from here.

## Phase 4 — Interview Readiness & Job Search

**Status: Complete.** Delivered as reference tools/documents (Claude
artifacts tied to this account, not repo files):

| Sub-phase | Deliverable |
|---|---|
| 4.1 | [Technical Skill Roadmap](https://claude.ai/code/artifact/255f46fe-c601-4a02-8b12-2e973ec61484) — 14-skill, 5-tier junior-readiness roadmap |
| 4.2 | [Portfolio Expansion Plan](https://claude.ai/code/artifact/1c8f8f5e-2275-4665-854f-963371c051f4) — 5 new project specs |
| 4.3 | [Interview Preparation](https://claude.ai/code/artifact/becceae5-42df-47ca-9691-29cef3190a79) — 9 technical topics + real STAR stories |
| 4.4 | [Job Search Tracker](https://claude.ai/code/artifact/9d6ebd77-1220-4618-9ec9-a115adaa6beb) — working application CRM |
| 4.5 | [Resume Variants + Cover Letter](https://claude.ai/code/artifact/27668995-a448-48d7-8a70-15134e4b15fa) |
| 4.6/4.7 | [Ongoing Practices & Habits](https://claude.ai/code/artifact/b67621c2-8311-4974-827c-1ff5f280dddb) — GitHub/LinkedIn cadence + growth habits |
| 4.8 | [Progress Dashboard](https://claude.ai/code/artifact/d63036b5-ac6a-48dc-92a5-528bbd6b327d) — junior-roadmap milestone + funnel tracker |

## Phase 5 — Career Growth & Roman Creative Studio

**Status: Complete.**

| Sub-phase | Deliverable |
|---|---|
| 5.A | [Multi-Year Engineering Roadmap](https://claude.ai/code/artifact/c0b810fe-9078-4115-96ef-872ca94d8af5) — 14 skills, 3 years, past the junior ceiling |
| 5.B | [Portfolio Evolution + Content Strategy](https://claude.ai/code/artifact/3325c256-7fb0-4274-a6b3-77855b9839ad) |
| 5.C | [Agency Operations + Growth](https://claude.ai/code/artifact/84734022-aebc-463c-be62-a7b6f5a14e47) — Roman Creative Studio, formalized (contracts section requires attorney review before use) |
| 5.D | [Continuous Growth System](https://claude.ai/code/artifact/40fb9e43-9b10-4037-876b-2abce32ac549) — OSS + professional development as a Now/Year 1/Year 3 progression |
| 5.E | [Long-Term Success Dashboard](https://claude.ai/code/artifact/613dfe1f-67e4-40e7-81e5-ff08f2097325) — career/engineering/portfolio milestones + agency growth stage |

## Phase 6 — Long-Term Excellence & Continuous Improvement

**Status: Complete.**

Most of what Phase 6 asked for — Engineering Excellence, Portfolio
Evolution, Professional Habits, Business Growth, Community Involvement,
Success Metrics — is already covered by Phase 5's deliverables above, so
it isn't duplicated here. What's genuinely new to Phase 6 follows.

### Career reflection (quarterly)

A repeatable retrospective, meant to live in this repo rather than a
Claude artifact — so the git history itself becomes the record of past
reflections, not just the current answers.

**How to use it:** each quarter, copy the template below into a new file
at `docs/reflections/YYYY-QX.md` (e.g. `docs/reflections/2026-Q3.md`),
answer it honestly, and commit it.

```markdown
# Reflection — 2026-Q3

**What new skills did I develop this quarter?**


**Which project best demonstrates my current ability, and why?**


**What feedback have I received** (from a job, clients, code review, or
the community)?


**What should I improve next quarter?**


**What no longer reflects my best work, and should be updated or retired?**

```

### Personal brand consistency

One identity statement, reused everywhere, so a recruiter (or a client)
recognizes the same person telling the same story across every surface:

> Self-taught front-end developer who builds fast, conversion-focused
> websites for real clients — currently running Roman Creative Studio and
> co-hosting 4Kingdom Podcast.

Quarterly consistency check (pair with the reflection above):

- [ ] Portfolio hero, About page, and `resume.html` summary all use
      language consistent with the identity statement above
- [ ] GitHub profile bio matches
- [ ] LinkedIn headline + About section match
- [ ] Roman Creative Studio's own "about the founder" copy (if any) is
      consistent, not contradictory
- [ ] 4Kingdom Podcast bio states the same real facts (co-host, developer)
      without turning into tech-marketing content for that audience —
      keeping the audience separation from Phase 5.B

---

## What's next

**Immediate:**
- Fill in `resume.html`'s bracketed placeholders before sending it anywhere.
- Replace the `https://alexanderroman.dev` placeholder domain in every
  `og:url`/canonical tag, `sitemap.xml`, and `robots.txt` once the site has
  a real deployed domain.
- Share your GitHub username to unblock the one remaining Phase 3 item
  (the profile README).

**Ongoing:**
- One `docs/reflections/YYYY-QX.md` file per quarter.
- The personal-brand checklist above, reviewed at the same cadence.
- The Phase 4.8 and 5.E dashboards, reviewed weekly and quarterly
  respectively (they say this themselves, but it's worth repeating here).
