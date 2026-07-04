# Funding Catalyst — Redesign Mockup

**Project:** `~/hermes-lab/funding-catalyst-redesign/`

A single-page HTML mockup of the redesigned Thin Air Labs Funding Catalyst page.

## What Changed

| Area | Before | After |
|---|---|---|
| **Title tag** | `Thin Air Labs \| Funding Catalyst` | `Grant Writing & Non-Dilutive Funding for Calgary Startups \| Thin Air Labs` |
| **Meta desc** | No location, no keywords | $95M, Calgary, grant writers, program names |
| **H1 structure** | 4 x `<h1>` | 1 x `<h1>` + `<h2>` for subsections |
| **Canonical** | Double slash bug (`//services`) | Fixed single slash |
| **JSON-LD** | None | Service + LocalBusiness + FAQ + Breadcrumb + Review |
| **OG/Twitter** | No image, weak copy | Proper cards + image placeholder |
| **Eligibility** | None | "Who this is for" — filters by stage, sector, geography |
| **Process** | None | 4-step timeline (qualify → strategy → apply → report) |
| **Clients** | One logo carousel | Grouped by sector (Health, Climate, FinTech, Energy) |
| **Form** | "Connect with us" (blind CTA) | 3-question qualification form with routing logic |
| **FAQ** | None | 5 questions with FAQ schema |
| **CTA** | "Connect with us" | "Check your fit" / "Start qualification check" |
| **Analytics** | UA-XXXXX (deprecated) | N/A (needs GA4 migration) |
| **Pricing signal** | None | FAQ addresses cost model + no percentage cut |

## Key Design Decisions

1. **Qualification-first funnel** — The form filters BEFORE a meeting gets booked. Unqualified leads get resources, not a sales call.
2. **Self-selection eligibility box** — Reduces unqualified form submissions before they even start.
3. **No "free strategy call" CTA** — The CTA is "Check your fit" which leads to the form, not a calendar.
4. **FAQ answers the money questions** — Pricing, success rate, timeline — all addressed without requiring a call.
5. **Process visibility** — A founder can see the full engagement scope before reaching out.

## To Do for Production

- [ ] Fix the canonical URL bug on the live Webflow page
- [ ] Update title + meta description in Webflow page settings
- [ ] Change H1s to single H1 + H2s in Webflow
- [ ] Add the JSON-LD schemas to the page head
- [ ] Add OG image (1200x630 branded graphic)
- [ ] Replace UA-XXXXX with GA4 measurement ID
- [ ] Build the qualification form with actual backend routing
- [ ] Write alt text for case study images
- [ ] Add internal links from blog posts to this page
