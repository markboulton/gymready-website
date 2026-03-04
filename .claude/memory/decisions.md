# GymReady Website — Architecture Decisions

## ADR-001: Static HTML over framework (2026-03-04)
**Decision:** Plain HTML/CSS/JS with no build step or framework.
**Rationale:** Marketing site is simple, doesn't need React/Next.js overhead. Faster load times, simpler deploys, easier to maintain. Can always add a framework later if needed.

## ADR-002: Netlify hosting (2026-03-04)
**Decision:** Host on Netlify.
**Rationale:** Already using Netlify for gymready-api functions. Single platform for website + API. Built-in CDN, forms, analytics, deploy previews.

## ADR-003: Dark theme matching iOS app (2026-03-04)
**Decision:** Dark background with green accent, matching the iOS app's design system.
**Rationale:** Brand consistency across app and website. VeloReady product family alignment.
