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
