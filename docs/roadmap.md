# Roadmap

Each phase is sized for one short session. Work through them in order; update
[PROGRESS.md](../PROGRESS.md) at the end of each session.

## Phase 0 — Project Setup

- Initialize git repo.
- Scaffold Astro project.
- Add Tailwind CSS.
- Add React integration (`@astrojs/react`).
- Base folder structure (`src/pages`, `src/components`, `src/layouts`, `src/content`).
- `.gitignore`.
- Netlify config skeleton (`netlify.toml`).

**Done when:** `astro dev` runs locally and shows a blank Tailwind-styled page; repo is committed.

## Phase 1 — Design System

- Define modern tech-forward palette (dark base + teal/indigo accent) as Tailwind theme tokens.
- Typography scale and font choice.
- Base layout shell: header/nav, footer, page container.

**Done when:** a shared `Layout.astro` renders consistent header/nav/footer with the palette applied,
usable by all pages.

## Phase 2 — Home Page

- Headline, short intro, service highlights, featured samples teaser, "Book a Call" CTA.

**Done when:** Home page is built using copy from [docs/content.md](content.md#home) and links to
Services, Portfolio, and Contact.

## Phase 3 — Services Page

- Four service areas: admin & transaction support, listings & marketing, lead & CRM management,
  tech support.

**Done when:** Services page renders all four areas with copy from
[docs/content.md](content.md#services).

## Phase 4 — Portfolio Page

- Sample projects, clearly labeled as samples: property landing page, flyers/social posts, lead
  follow-up email sequence, transaction tracker, automation demo, market report template.

**Done when:** Portfolio page lists all six samples with the "sample, not a real client project"
labeling from [docs/content.md](content.md#portfolio).

## Phase 5 — About Page

- Career-shift story, why the engineering background helps clients, US time zone working hours.

**Done when:** About page reflects the story outline in [docs/content.md](content.md#about).

## Phase 6 — Contact Page

- Contact form (Netlify Forms or Formspree), Calendly embed, email, LinkedIn, downloadable resume
  link.

**Done when:** form submits successfully (test submission) and all contact links/embeds work.

## Phase 7 — Blog Scaffolding

- Astro content collection config for blog posts.
- MDX post schema (title, date, tags, cover image, etc.).
- Blog listing page + individual post template.
- Image optimization and YouTube embed handling.

**Done when:** one placeholder/test post renders correctly end-to-end (listing → post page); no real
posts required yet.

## Phase 8 — Polish & SEO

- Meta tags per page, sitemap, favicon.
- Image optimization pass.
- Basic accessibility check (headings, alt text, contrast).
- Responsive check (mobile/tablet/desktop).

**Done when:** Lighthouse/manual pass shows no major SEO/accessibility/responsive issues.

## Phase 9 — Deploy

- Connect repo to Netlify.
- Verify production build.
- Confirm contact form works live.
- Custom domain: noted as a later follow-up, not required for this phase.

**Done when:** site is live on a Netlify subdomain and fully functional.
