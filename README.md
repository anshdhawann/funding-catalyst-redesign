# Funding Catalyst — Redesign Mockup

**Project:** `~/hermes-lab/funding-catalyst-redesign/`
**Live page:** https://www.thinairlabs.ca/services/funding-catalyst

A single-page HTML mockup of the redesigned Thin Air Labs Funding Catalyst page. No build step — all CSS and JS are inline in `index.html`.

## Files

| File | Purpose |
|---|---|
| `index.html` | The page — markup, CSS, and JS inline |
| `hero-leaf.png` | Transparent blue maple-leaf mark used in the hero right column |

## Tech Stack

- Single-file HTML (no framework, no build step)
- Inline `<style>` + `<script>`
- Fonts: **Source Serif 4** (headlines) + **Plus Jakarta Sans** (body/UI), via Google Fonts
- IntersectionObserver for scroll-reveal and stat count-up
- `prefers-reduced-motion` accessibility guard

## Design System

- **Background:** white (`#ffffff`) + alt section (`#f6f9fc`)
- **Accent:** `#79BDE9` (light) / `#5aa9dc` (strong)
- **Text:** `#0a1f2e` (primary) / `#5b6b7c` (muted)
- Typography split: serif headlines for authority, sans-serif for modern/tech feel
- McKinsey-inspired minimal hero with maple-leaf mark

## Section Order

1. Hero — headline, email capture, 2 proof stats, trust marquee
2. What we do — funding lifecycle (readiness → strategy → implementation → ongoing) + program capability strip
3. What the relationship looks like — ongoing partner cadence
4. Who we work with — stage / sectors / location / revenue
5. Case studies — 3 cards with real cover images
6. Who you'll work with — Funding Catalyst team (8 people, real headshots)
7. Quote — founder testimonial (Ammar Memon, Quickly)
8. FAQ — 5 questions
9. CTA banner
10. Footer — multi-column (Services, Company, Connect, Legal)

## SEO

- Semantic H1 + H2 hierarchy (single H1, section titles are H2)
- 4 JSON-LD schema blocks: ProfessionalService, Service, FAQPage, BreadcrumbList
- Open Graph + Twitter card meta (OG image asset needs to be created — see TODO)
- hreflang for en-CA / en-US / x-default
- Canonical URL set
- Meta description (~160 chars) + keywords

## TODO for Production

- [ ] Create OG image (1200×630 branded PNG) at `thinairlabs.ca/images/og/funding-catalyst-1200x630.png` — referenced in OG/Twitter meta but does not exist yet
- [ ] Replace placeholder telephone (`+1-403-000-0000`) in ProfessionalService schema with real number
- [ ] Add mobile hamburger menu (nav links currently hidden below 768px)
- [ ] Wire up email capture form to a real backend / email service
- [ ] Migrate to GA4 (no analytics currently wired)
