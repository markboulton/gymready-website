# CLAUDE.md

## Quick Reference
- **Type**: Marketing website
- **Stack**: HTML/CSS/JS (static site)
- **Hosting**: Netlify
- **Ecosystem**: Part of GymReady product family (iOS app + website)
- **Related repos**: `~/Dev/gymready` (iOS app), `~/Dev/gymready-api` (Supabase/Netlify functions)

## Project Overview

GymReady Website is the marketing and landing page for GymReady — an iOS app for intelligent strength training. The site handles:
- Product marketing and feature showcase
- App Store download links
- Pricing/subscription info
- Privacy policy and terms of service
- Support/contact information

**Product positioning:** GymReady is NOT a workout tracker. It's the brain that sits on top of tracking data — mesocycle programming, fatigue management, deload intelligence, and volume analytics.

**Pricing:** 7-day free trial, then £4.99/mo or £39.99/yr. No free tier — all features included.

## Build & Deploy

```bash
# Local development
npx serve public          # Serve locally

# Deploy
# Netlify auto-deploys from main branch
# Build command: (none — static site)
# Publish directory: public
```

## Project Structure

```
public/              — Static site files (Netlify publish directory)
  index.html         — Main landing page
  privacy.html       — Privacy policy
  terms.html         — Terms of service
  support.html       — Support page
  assets/            — Images, icons, fonts
  css/               — Stylesheets
  js/                — Client-side scripts
netlify.toml         — Netlify configuration
```

## Design Principles

- Mobile-first responsive design
- Fast loading — minimal JS, optimised assets
- Consistent with GymReady app branding (dark theme, ascending bars icon)
- VeloReady product family visual alignment

## Workflow Rules

### Commit Protocol
- Format: `type(scope): description` (e.g., `feat(landing): Add hero section`)
- Types: feat, fix, style, content, chore, docs

### Code Change Protocol
1. Read affected code first
2. Follow semantic HTML
3. Keep accessibility in mind (WCAG 2.1 AA)
4. Test responsive behaviour

## Memory System

### File Index
**Durable (repo `.claude/memory/` — syncs via git):**
- `architecture.md` — Site structure and key patterns
- `TODO.md` — Task list
- `decisions.md` — Design/architecture decisions
- `common-bugs.md` — Bug patterns and fixes

**Transient (local `~/.claude/projects/.../memory/`):**
- `MEMORY.md` — Hub index, auto-loaded each session
- `session-log.md` — Rolling session history
