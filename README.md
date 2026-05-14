# Derma.Log Web

This repository contains the public static website for Derma.Log.

The site is hosted via GitHub Pages and uses the canonical domain:

https://derma-log.eu

## Scope

This repository contains public website, legal, privacy, and support pages only.

No private app code, private implementation details, backend provider details, internal documentation, or private repository material belongs in this repository.

Legal page content is public-facing publication material derived from private source-of-truth legal documents. The public site should publish only the wording needed for web and App Store compliance.

## Structure

- `/` - homepage
- `/privacy/` - Privacy Policy
- `/terms/` - Terms of Service
- `/medical-disclaimer/` - Medical Disclaimer
- `/support/` - support information
- `/subscription-terms/` - Subscription Terms
- `/account-deletion/` - Account Deletion & Retention Notice
- `/export-backup/` - Data Ownership, Export & Backup Notice
- `/assets/styles.css` - shared static styling
- `/assets/brand/dermalog-logo.svg` - public Derma.Log logo asset

## Hosting

The site is hosted via GitHub Pages. The `CNAME` file sets the custom domain to `derma-log.eu`.

The site intentionally uses plain HTML and CSS only. It does not use JavaScript, analytics, cookies, package tooling, or external dependencies.

## Repository Documentation

Repository role and publication-boundary rules are documented in `Documentation/repository-boundary.md`. This documentation is for maintainers and is not part of the public website navigation.
