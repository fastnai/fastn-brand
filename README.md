# Fastn Brand System — v1.0

The official Fastn brand guidelines. Everything you need to represent Fastn correctly across any surface.

## Contents

| File | Description |
|---|---|
| [`logos/`](./logos) | Official Fastn logo files (SVG, PNG, JPG) |
| [`fastn-brand-system.html`](./fastn-brand-system.html) | Interactive brand guidelines — open in any browser |
| [`tokens.json`](./tokens.json) | Design tokens for Figma, Style Dictionary, Tailwind |
| [`tokens.css`](./tokens.css) | CSS custom properties — drop into any project |
| [`SKILL.md`](./SKILL.md) | Claude AI skill — adds brand context to any AI-assisted work |

## Logos

| File | Description |
|---|---|
| [`fastn-logo.svg`](./logos/fastn-logo.svg) | Full logo with wordmark (SVG, scalable) |
| [`fastn-logo-740px.png`](./logos/fastn-logo-740px.png) | Full logo with wordmark (PNG, 740px) |
| [`fastn-logo-400px.png`](./logos/fastn-logo-400px.png) | Full logo with wordmark (PNG, 400px) |
| [`fastn-icon-rounded.jpg`](./logos/fastn-icon-rounded.jpg) | Icon mark only, rounded square background |
| [`fastn-icon-square.jpg`](./logos/fastn-icon-square.jpg) | Icon mark only, square background |
| [`fastn-icon-linkedin.jpg`](./logos/fastn-icon-linkedin.jpg) | Icon mark sized for LinkedIn |

## Quick Start

Open `fastn-brand-system.html` in a browser — no build step needed.

Use tokens in your project:

```css
.button {
  background: var(--brand);       /* #6C5CE7 */
  color: #fff;
  border-radius: var(--radius-3); /* 8px */
}
```

## Brand at a Glance

### Colors

| Token | Value | Use |
|---|---|---|
| `--brand` | `#6C5CE7` | Primary — CTAs, links, focus rings |
| `--brand-hover` | `#5A4CD6` | Hover/pressed states |
| `--brand-light` | `#8F85E8` | Tags, labels, eyebrows |
| Gradient | `#6C5CE7 to #A78BFA` | Hero art, avatars — sparingly |
| `--success` | `#10B981` | Positive states |
| `--warning` | `#F59E0B` | Caution states |
| `--error` | `#EF4444` | Error states |

### Typography

- **Headings**: Geist — weight 400-800
- **Body**: Inter — weight 400-600, for body text and long-form content
- **Mono**: Geist Mono — for all code and technical content
- **Display**: 96px, Geist weight 800, tracking -0.04em
- **Body text**: 16px, Inter weight 400, line-height 1.7

### Dual Theme

| | Dark (marketing, docs) | Light (app, dashboard) |
|---|---|---|
| Background | `#101014` | `#FFFFFF` |
| Card | `#18181E` | `#F5F5FA` |
| Border | `#2A2A36` | `#E0E0EC` |
| Body text | `#A0A0B8` | `#3A3A55` |

The brand primary `#6C5CE7` is **identical in both themes** — the visual thread connecting every surface.

## Using with AI (Claude)

Drop `SKILL.md` into a Claude Project as a project file. Every conversation will automatically apply Fastn brand.

## Version History

| Version | Date | Notes |
|---|---|---|
| 1.0 | Feb 2025 | Initial release — unified dark/light system, Electric Indigo primary |

---

**fastn.ai**
