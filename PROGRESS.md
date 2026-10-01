# Progress

Reference: [docs/roadmap.md](docs/roadmap.md) (all phases, with "done when" criteria) ·
[docs/content.md](docs/content.md) (site copy)

## Current Phase

Phase 5 — About Page. Phases 0–4 (setup, design system, home, services, portfolio) are complete.

## Completed

- [x] **Phase 0 — Project Setup** — git repo initialized; Astro scaffolded with `@astrojs/react`
      and Tailwind v4 (`@tailwindcss/vite`); base folders `src/components`, `src/layouts`,
      `src/content` created; `npm run build` and `npm run dev` verified working, Tailwind
      utilities compiling correctly. Pushed to GitHub:
      https://github.com/vincentsotoya/real-estate-va-portfolio (branch `main`).

- [x] **Phase 1 — Design System** — palette (`bg`, `surface`, `surface-2`, `border`, `text`,
      `muted`, `teal`, `indigo`) and fonts (Space Grotesk headings, Inter body, JetBrains Mono
      accents, self-hosted via `@fontsource-variable/*`) defined as Tailwind v4 `@theme` tokens in
      `src/styles/global.css`; `src/layouts/Layout.astro` provides head/meta, skip link, sticky
      header with active-page nav + mobile menu, "Book a Call" CTA, footer, and page container.
      `index.astro` uses it as a smoke test. Verified: `npm run build` passes; desktop and 390px
      mobile render correctly; menu toggles; fonts load; contrast AA-compliant (body text 16:1,
      muted 6.3:1, teal 9.6:1, indigo 6.4:1).

- [x] **Phase 2 — Home Page** — `src/pages/index.astro` rebuilt with real copy from
      [docs/content.md](docs/content.md#home): hero (eyebrow, headline, intro, "Book a Call" +
      "See the Work" CTAs), "Where I Fit In" service-highlight grid (condensed from the four
      Services categories, links to `/services`), "Sample Work" teaser (portfolio disclaimer +
      chips for the six sample items, links to `/portfolio`), and a closing "Book a Call" CTA
      banner linking to `/contact`. `/services`, `/portfolio`, and `/contact` don't exist yet
      (later phases) so those links are placeholders. Verified: `npm run build` passes; desktop
      render (1440px, via Claude in Chrome) confirmed. Mobile-width screenshot could not be
      verified this session — the browser tool's `resize_window` call reported success but the
      captured viewport stayed at desktop width — so 390px rendering relies on the same
      `sm:`/`lg:` Tailwind patterns already confirmed responsive in Phase 1's `Layout.astro`
      (grid, flex-wrap, stacked CTAs) rather than a fresh screenshot; worth a manual check next
      session.

- [x] **Phase 3 — Services Page** — `src/pages/services.astro` renders all four service areas
      (Admin & Transaction Support, Listings & Marketing, Lead & CRM Management, Tech Support) with
      copy from [docs/content.md](docs/content.md#services), plus a "Book a Call" closing CTA.
      Copy stays at the "process/technical aptitude" level (no unconfirmed CRM/MLS/Canva names).
      Verified: `npm run build` passes and emits `/services`. Committed on branch
      `phase-3-services`, not yet merged to `main`. Visual/mobile render not re-checked.

- [x] **Phase 4 — Portfolio Page** — `src/pages/portfolio.astro` lists all six samples from
      [docs/content.md](docs/content.md#portfolio), each tagged "Sample project", with a page-level
      note that none of it is real client work, and a "Book a Call" CTA. Descriptions use only the
      content.md wording (no invented results or tools). Verified: `npm run build` passes and emits
      `/portfolio`. Not yet visually checked (desktop or 390px). Branch `phase-4-portfolio`.

## Current Task

- [ ] **Phase 5 — About Page**: see [docs/roadmap.md](docs/roadmap.md).

## Next

- [ ] Phase 6 — Contact Page
- [ ] Phase 7 — Blog Scaffolding
- [ ] Phase 8 — Polish & SEO
- [ ] Phase 9 — Deploy

See [docs/roadmap.md](docs/roadmap.md) for what each phase covers and its "done when" criteria.

## Blockers

None.

## Recent Decisions

- **React over Vue** for interactive components — practice goal; both are on the resume, and this
  site's interactivity is minimal enough that the choice is low-stakes either way.
- **Vercel over Netlify** for deploy — `netlify.toml` removed (Vercel needs no config file for
  Astro); contact form plan narrowed from "Netlify Forms or Formspree" to **Formspree only**,
  since Netlify Forms only works when hosted on Netlify.
- **Contact form provider: Formspree**, wired up in Phase 6.
