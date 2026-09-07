# SEO maintenance — 2026-09-07

This repository contains a static Next.js export, not the original application source. Changes to HTML must stay consistent with the accompanying RSC `.txt` files, embedded Flight payloads, and any affected client components. Changed JavaScript bundles were renamed to new content hashes so old caches cannot mix versions.

## Published changes

- More descriptive homepage, owner and trade landing-page copy and titles.
- Canonical and indexation metadata on five partner landing pages.
- A static `/ratgeber/` hub and three original organizational checklists.
- Footer links connecting the guides and existing thematic landing pages.
- WebP versions of eight app screenshots, retaining PNG originals.
- Sitemap URLs normalized to trailing slashes, missing Makler and guide pages included, stale fixed modification dates removed.

## Hosting

GitHub Pages uses `www.eigenheimverwalter.de` with enforced HTTPS. The bare domain currently points to an external server and redirects incorrectly to the GitHub account root. Fix that redirect in the hosting/domain administration to `https://www.eigenheimverwalter.de`, preserving the request path and query string. Repository changes do not control that external redirect.

Do not publish the original application source, `.git`, credentials, or private configuration to a web root. When the original Next.js source becomes available, port these changes into it before regenerating the export.

## Validation

Validate one H1, title, description and canonical on each indexable page; parse JSON-LD; resolve local assets and sitemap destinations. Test mobile and desktop with JavaScript enabled, including footer navigation to static guide pages. Search Console remains necessary to verify actual Google indexing and performance; no ranking outcome is assumed.
