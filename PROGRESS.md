# Progress

Reference: [docs/roadmap.md](docs/roadmap.md) (all phases, with "done when" criteria) ·
[docs/content.md](docs/content.md) (site copy)

## Current Phase

Phase 1 — Design System. Phase 0 is complete: repo scaffolded and live on GitHub.

## Completed

- [x] **Phase 0 — Project Setup** — git repo initialized; Astro scaffolded with `@astrojs/react`
      and Tailwind v4 (`@tailwindcss/vite`); base folders `src/components`, `src/layouts`,
      `src/content` created; `npm run build` and `npm run dev` verified working, Tailwind
      utilities compiling correctly. Pushed to GitHub:
      https://github.com/vincentsotoya/real-estate-va-portfolio (branch `main`).

## Current Task

- [ ] **Phase 1 — Design System**: define the modern tech-forward palette (dark base +
      teal/indigo accent) and typography as Tailwind theme tokens; build the shared layout shell
      (`Layout.astro` with header/nav, footer, page container) that every later page reuses.

## Next

- [ ] Phase 2 — Home Page
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
