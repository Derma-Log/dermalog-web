# Derma.Log Web Repository Boundary

This document defines the role of the public `Derma-Log/dermalog-web` repository so the website does not drift into private app, infrastructure, or source-of-truth legal territory.

## Repository Purpose

`Derma-Log/dermalog-web` is the public product web presence for Derma.Log.

It exists to host:

- the public homepage
- Privacy Policy
- Terms of Service
- Medical Disclaimer
- support information
- public legal notices required for App Store and web review
- GitHub Pages configuration for `derma-log.eu`

This repository should remain small, static, and publication-focused.

## Identity Boundary

Derma.Log uses separated identities and repositories:

- `Derma-Log` is the public product GitHub user namespace.
- `Derma-Log/dermalog-web` is the public website repository.
- `Sstc89` is the founder/developer identity and may collaborate on the public repository.
- The private app/development repository remains the source of implementation truth and private legal source material.

Do not collapse these roles. Public website work should not require access to private app code.

## What Belongs Here

Content belongs in this repository when it is intended to be public and useful for website, trust, support, or App Store review surfaces.

Appropriate content includes:

- plain HTML/CSS pages served by GitHub Pages
- public-facing legal and support wording
- public product positioning
- static assets required by the website
- documentation about this public repository's purpose and publication rules

## What Does Not Belong Here

Do not add:

- private app source code
- backend provider details
- database schema details
- private implementation material
- private source-of-truth legal markdown files
- internal product planning documents
- private repository paths
- secrets, credentials, tokens, or environment files
- analytics, trackers, cookie banners, package tooling, or build systems unless explicitly approved

If a detail is useful only for app implementation, backend operation, or private governance, it does not belong in this repository.

## Legal Content Rule

Private legal documents may be used as source material, but this repository should publish only public-facing wording needed for web and App Store compliance.

When updating legal pages:

- preserve the medical, privacy, subscription, deletion, export, and research boundaries
- simplify dense legal source material into clear public website language
- avoid exposing internal document names, private paths, or private implementation references
- do not publish future/internal policies as normal linked public pages unless explicitly approved
- keep legal pages truthful to current public product behavior

## Product and Medical Positioning

Derma.Log is a calm, structured skin observation and record-keeping tool.

Public copy must preserve these truths:

- Derma.Log helps users document, organize, review, export, and discuss skin observations over time.
- Derma.Log is not a diagnostic service.
- Derma.Log does not diagnose disease or rule out disease.
- Derma.Log does not detect or rule out cancer.
- Derma.Log does not replace medical professionals or provide emergency care.
- Support is not medical care.
- Urgent symptoms should be handled through qualified medical professionals or local emergency services.

Avoid startup hype, fear language, AI scanner language, or medical certainty.

## Privacy and Research Boundary

Public copy must preserve these truths:

- Derma.Log records may contain sensitive personal data.
- Private use remains private by default.
- Ordinary private account use is not an active research contribution program.
- Any future research or evidence contribution must be optional, explicit, consent-based, separately governed, and legally reviewed before activation.
- Exports and backups may contain sensitive data and should be reviewed before sharing.

Do not claim anonymized exports are impossible to re-identify.

## Subscription, Export, and Deletion Boundary

Public copy must preserve these truths:

- Existing owned history should remain accessible across subscription transitions.
- Subscription limits may restrict new storage growth but should not hide or lock existing records.
- Privacy and dignity controls should not be premium-only.
- Account deletion is intended to be permanent once completed.
- Account deletion does not delete files already exported, shared, saved, or stored outside Derma.Log.
- Exports are not clinician-created medical records unless a clinician separately reviews and adopts them.
- Restore behavior should not be claimed beyond what the app explicitly supports.

## Website Technical Rules

The public website should remain:

- static GitHub Pages output
- plain HTML/CSS
- no JavaScript unless explicitly required
- no analytics
- no cookies
- no external trackers
- no external dependencies
- no npm or package tooling
- no GitHub Actions unless explicitly needed

Use root-relative links because the canonical deployment target is `https://derma-log.eu`.

The root `CNAME` file must contain exactly:

```text
derma-log.eu
```

## Change Checklist

Before publishing changes, verify:

- all public links resolve on the custom domain
- `CNAME` remains unchanged
- no private implementation or private repo references were added
- no forbidden medical or AI claims were introduced
- no JavaScript, analytics, cookies, external dependencies, package tooling, or workflows were added without approval
- legal page wording remains public-facing and implementation-truthful
