---
name: dermalog-public-website
description: Use when creating, editing, or reviewing Derma.Log public website pages, legal/support pages, static HTML/CSS, GitHub Pages configuration, public screenshots, badges, or website copy in dermalog-web. Enforces the public repository boundary, static-site rules, medical claim limits, and Derma.Log's calm clinical design language.
---

# Derma.Log Public Website

## First Checks

- Read `Documentation/repository-boundary.md` before changing product positioning, legal text, support text, privacy text, subscription text, deletion text, export text, or App Store compliance wording.
- Confirm the change belongs in this public web repository. If it needs private app code, backend details, database schema, private legal source files, or internal planning, stop and ask for the public-safe source wording instead.

## Technical Rules

- Keep the site static: plain HTML/CSS served by GitHub Pages.
- Do not add JavaScript, analytics, cookies, external trackers, package tooling, build systems, or GitHub Actions unless explicitly approved.
- Keep `CNAME` exactly `derma-log.eu`.
- Use root-relative links for public pages and assets.
- Use existing page structure, CSS tokens, and assets first.
- Do not hardcode new colors, spacing, typography, or shadows when a token already exists in `assets/styles.css`.

## Copy Rules

- Derma.Log helps users document, organize, review, export, and discuss skin observations over time.
- Derma.Log is not a diagnostic service and does not detect or rule out cancer.
- Support is not medical care.
- Urgent symptoms should go to qualified medical professionals or local emergency services.
- Avoid fear language, startup hype, AI scanner language, medical certainty, and unsupported clinical claims.
- Keep wording calm, clinical, structured, concise, and public-facing.

## Verification

Before finishing website work, check:

- public links resolve with root-relative paths
- no private implementation, repository, backend, schema, or source-document references were added
- no forbidden medical or AI claims were introduced
- legal/support pages remain public-facing and truthful to current product behavior
- static-site rules remain intact
