# Derma.Log Web

This repository contains the public static website for Derma.Log.

The site is hosted via GitHub Pages and uses the canonical domain:

https://derma-log.eu

## Scope

This repository contains public website, legal, privacy, and support pages only.

No private app code, private implementation details, backend provider details, internal documentation, or private repository material belongs in this repository.

Legal page content is public-facing publication material derived from private source-of-truth legal documents. The public site should publish only the wording needed for web and App Store compliance.

## Structure

- `/` - international English homepage and default locale
- `/knowledge/` - English Knowledge Library index and educational articles
- `/da/` - Danish homepage and Danish-localized public pages
- `/da/knowledge/` - Danish Knowledge Library index and educational articles
- `/da/press/` - Danish press description and key facts
- `/privacy/` - Privacy Policy
- `/terms/` - Terms of Service
- `/medical-disclaimer/` - Medical Disclaimer
- `/support/` - support information
- `/subscription-terms/` - Subscription Terms
- `/account-deletion/` - Account Deletion & Retention Notice
- `/export-backup/` - Data Ownership, Export & Backup Notice
- `/assets/styles.css` - shared static styling
- `/assets/brand/dermalog-logo.svg` - public Derma.Log logo asset
- `/output/pdf/dermalog-da-a4-poster.pdf` - Danish A4 poster with verified App Store QR code

## Hosting

The site is hosted via GitHub Pages. The `CNAME` file sets the custom domain to `derma-log.eu`.

The site intentionally uses plain HTML and CSS only. It does not use JavaScript, analytics, cookies, package tooling, or external dependencies.

The international English site remains the default at the root URL. Danish pages use the `/da/` path and link back to the English equivalent. Geographic locale routing, if enabled, belongs at the hosting edge and must not be implemented with client-side JavaScript in this repository.

## Repository Documentation

Repository role and publication-boundary rules are documented in `Documentation/repository-boundary.md`. This documentation is for maintainers and is not part of the public website navigation.

## Need-specific page pattern

The bilingual eczema/rash documentation page uses `/knowledge/en/eczema-rash-history/`
and `/da/knowledge/eczema-rash-history/`. It reuses the existing article and phone-image
classes: documentation need, Spot / repeated image-backed Logs, one authentic interface
example, non-diagnostic boundary, matching App Store CTA, related reading and trust links.
Language links retain the same documentation context. Both homepage headers link to
the Knowledge Library; each locale’s library and existing image-history article link
to the matching documentation page.

`Documentation/cpp-destinations.json` records Apple-returned CPP identities, checked
public URLs and language behavior. Null routes mean no page has been assigned; this
registry does not create or authorize additional pages. The homepage retains its
existing default App Store destination. Unavailable need-specific destinations have
no automatic fallback.

The page pair is included in `/sitemap.xml` with the existing canonical public pages.
Keep this static sitemap aligned with published routes. There is no repository build
command or sitemap generator; validate static links and HTML directly.
