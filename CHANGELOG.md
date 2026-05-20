# Changelog

All notable changes to the Fastn brand system are documented here.
The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and the project uses [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

Token, font, and visual changes that affect consumers are marked **breaking** under the major version they ship in.

## [Unreleased]

## [3.0.0] - 2026-05-20

### Changed (breaking)
- Replace the indigo + sky-blue palettes with a single Electric Indigo accent gradient (`#6C5CE7` to `#8E76F2`).
- Switch typography to Inter only. Geist and Geist Mono removed.
- New surface palette across dark and light themes (`#18181B`/`#1F1F23` and `#FFFFFF`/`#F4F4F6`).
- Replace atomic-only tokens with atomic + semantic aliases. `--t1` etc. still work; new `--color-text-primary` etc. are preferred for app code.
- Drop the Product UI warm palette.

### Added
- Light theme with `prefers-color-scheme` auto-detection and persistent user override.
- Self-hosted Inter (latin subset, 83KB woff2) instead of Google Fonts.
- Disabled and loading states for buttons.
- Input error and hint state styles.
- `forced-colors` (Windows High Contrast) media query.
- Print stylesheet.
- Open Graph and Twitter share meta tags plus `og.png` (1200x630).
- "Don't" section with five misuse patterns illustrated side-by-side.
- WCAG AA contrast table for every shipped combo.

### Fixed
- Inline link contrast in light theme (was 2.72, now 4.86 AA).
- Input placeholder contrast in both themes (was 2.48/2.67, now 4.60/5.17 AA).
- White text on the CTA gradient endpoint (was 2.72, now 3.48 AA-large via `19px / 700`).
- Color rows are now `<button>` elements, keyboard-accessible.

### Removed
- Geist, Geist Mono typefaces.
- Brand gradient as a decorative element (now reserved for the primary CTA).
- `PLAN.md` (was an internal planning doc).

## [2.0.0] - 2026-05-17

### Changed
- Soften brand palette and dark theme for eye comfort. Brand `#4F3FFF` to `#6C5CE7`; pink accent replaced with soft violet `#A78BFA`; dark surfaces lifted from `#09090E` to `#101014`; headings softened from pure white to `#E4E4EC`.

### Added
- Product UI warm palette for product surfaces.
- Inter as the body typeface alongside Geist.

## [1.0.0] - 2026-02-17

### Added
- Initial brand system release with dark and light themes, Electric Indigo primary, brand gradient, and Geist/Inter/Geist Mono typography.
- `fastn-brand-system.html` interactive guidelines.
- `tokens.css`, `tokens.json` design tokens.
- Logo assets (wordmark PNG, icon variants).
- `SKILL.md` Claude project file.
