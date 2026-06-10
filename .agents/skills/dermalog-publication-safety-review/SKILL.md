---
name: dermalog-publication-safety-review
description: Use when reviewing Derma.Log public-facing website, App Store, legal, support, social media, screenshot caption, campaign, or brand copy before publication. Checks medical claims, privacy/research boundaries, subscription/export/deletion promises, static web constraints, and separation from the private app repository/project.
---

# Derma.Log Publication Safety Review

## Review Scope

Use this skill as a final gate for public-facing Derma.Log material across website, App Store, and social/media surfaces.

## Required Checks

### Repository Boundary

- No private app code, private repository paths, backend provider details, database schema details, private legal source files, secrets, credentials, internal plans, or implementation-only material.
- App implementation remains in the private app repository/project.

### Medical Claims

- No diagnosis, screening, triage, treatment, cancer detection, cancer rule-out, disease prediction, or emergency-care substitution claims.
- No local risk computation or risk inference in public UI/copy.
- Support is not medical care.
- Urgent symptoms route to qualified medical professionals or local emergency services.

### Privacy And Research

- Private use remains private by default.
- Ordinary private account use is not described as research participation.
- Any research/evidence contribution is optional, explicit, consent-based, separately governed, and legally reviewed before activation.
- Do not claim anonymized exports are impossible to re-identify.

### Subscription, Export, And Deletion

- Existing owned history should remain accessible across subscription transitions.
- Storage limits may restrict new growth but should not hide or lock existing records.
- Privacy and dignity controls should not be premium-only.
- Account deletion is intended to be permanent once completed.
- Deletion does not delete files already exported, shared, saved, or stored outside Derma.Log.
- Exports are not clinician-created medical records unless a clinician separately reviews and adopts them.
- Do not promise restore behavior beyond what the app explicitly supports.

### Website Constraints

- Static HTML/CSS only unless explicitly approved.
- No JavaScript, analytics, cookies, external trackers, package tooling, build systems, or GitHub Actions unless explicitly approved.
- `CNAME` remains exactly `derma-log.eu`.

## Output Format

Lead with blocking issues if any. If none, state that no publication blockers were found. Then list any non-blocking wording improvements or assumptions that need owner confirmation.
