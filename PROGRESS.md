# Progress

Reference: [docs/roadmap.md](docs/roadmap.md) (all phases, with "done when" criteria) ·
[docs/content.md](docs/content.md) (site copy)

## Current Phase

Phase 2 — Home Page. Phases 0 (setup) and 1 (design system) are complete.

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

## Current Task

- [ ] **Phase 2 — Home Page**: see [docs/roadmap.md](docs/roadmap.md).

## Next

- [ ] Phase 3 — Services Page
- [ ] Phase 4 — Portfolio Page
- [ ] Phase 5 — About Page
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
