# AGENTS.md

Instructions for AI coding agents working in this project.

## What this is

Osher turns a child's photo into a personalized 3D-printed character figure,
optionally hand-painted, ordered via WhatsApp. V1 is a single-page,
mobile-first landing site for parents in India: concept, character collection,
process, gallery, pricing, testimonials, and prominent WhatsApp CTAs.

Static site, no backend. Source of truth for product scope is the project
planning docs.

## Stack

- HTML5, CSS3, vanilla JavaScript
- Static assets: `css/`, `js/`, `images/` (WebP/AVIF preferred), `fonts/`
- No framework, no build pipeline, no database, no auth
- Hosting: GitHub Pages, custom Osher domain, HTTPS

## Commands

- Preview: `python3 -m http.server 8000` then open http://localhost:8000
- Alternative: open `index.html` directly, or `npx serve .`

No build, lint, typecheck, or preview-bundle commands exist.

Testing is opt-in. No unit test runner is configured, so there is no required
test gate yet. Browser testing is also opt-in; no browser harness is
configured. Do not invent test commands.

## Conventions

- Mobile-first, fully responsive (mobile, tablet, desktop)
- Touch-friendly, readable without zoom, no hover-dependent interactions
- Brand palette: Primary Navy `#2F39A9`, Secondary Blue `#2E6FA0`,
  Teal `#49A4BB`, Accent Mint `#15D8B3`, plus white/neutrals for contrast
- Fun, imaginative, premium; rounded cards, subtle animations, clear hierarchy
- Fast loading: optimized images, minimal JS
- WhatsApp CTAs use `wa.me` links with pre-filled enquiry message
- No customer data stored on site; photos/orders/payments via WhatsApp
- Keep changes minimal, match existing patterns, no unrelated refactors
- Concise comments only for non-obvious why; self-documenting names
