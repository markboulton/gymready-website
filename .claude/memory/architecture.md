# GymReady Website — Architecture

## Site Structure
```
public/                    — Netlify publish directory
  index.html               — Landing page (hero, features, pricing)
  privacy.html             — Privacy policy
  terms.html               — Terms of service
  support.html             — Support/contact
  css/
    style.css              — Main stylesheet
  js/                      — Client-side JS (minimal)
  assets/                  — Images, icons, fonts
netlify.toml               — Netlify build & redirect config
```

## Stack
- **Static HTML/CSS/JS** — no build step, no framework
- **Netlify** — hosting, CDN, form handling, analytics
- **Design** — dark theme, green accent (#4ade80), matches iOS app branding

## Ecosystem
- **gymready** (iOS app) — links to website for privacy/terms/support
- **gymready-api** — Supabase + Netlify functions (separate)
- **gymready-website** — this repo, marketing site

## Design Tokens (aligned with iOS app)
- Background: #0a0a0a
- Surface: #141414
- Surface alt: #1a1a1a
- Border: #222
- Text: #f0f0f0
- Muted: #999
- Accent: #4D9FFF (blue, matches app GRColorScale.accent dark mode)
- Accent hover: #3D7FE5 (app GRColorScale.accent light mode)
