# Fastn Brand System — v1.0

The official Fastn brand guidelines. Everything you need to represent Fastn correctly across any surface.

## Contents

| File | Description |
|---|---|
| [`fastn-brand-system.html`](./fastn-brand-system.html) | Interactive brand guidelines — open in any browser |
| [`tokens.json`](./tokens.json) | Design tokens for Figma, Style Dictionary, Tailwind |
| [`tokens.css`](./tokens.css) | CSS custom properties — drop into any project |
| [`SKILL.md`](./SKILL.md) | Claude AI skill — adds brand context to any AI-assisted work |

## Quick Start

Open `fastn-brand-system.html` in a browser — no build step needed.

Use tokens in your project:

```css
.button {
  background: var(--brand);       /* #4F3FFF */
  color: #fff;
  border-radius: var(--radius-3); /* 8px */
}
```

## Brand at a Glance

### Colors

| Token | Value | Use |
|---|---|---|
| `--brand` | `#4F3FFF` | Primary — CTAs, links, focus rings |
| `--brand-hover` | `#3B2DE8` | Hover/pressed states |
| `--brand-light` | `#7B6FFF` | Tags, labels, eyebrows |
| Gradient | `#4F3FFF to #FF4D8D` | Hero art, avatars — sparingly |
| `--success` | `#10B981` | Positive states |
| `--warning` | `#F59E0B` | Caution states |
| `--error` | `#EF4444` | Error states |

### Typography

- **Font**: Geist — weight 400-800
- **Mono**: Geist Mono — for all code and technical content
- **Display**: 96px, weight 800, tracking -0.04em
- **Body**: 16px, weight 400, line-height 1.7

### Dual Theme

| | Dark (marketing, docs) | Light (app, dashboard) |
|---|---|---|
| Background | `#09090E` | `#FFFFFF` |
| Card | `#111118` | `#F5F5FA` |
| Border | `#2E2E3A` | `#E0E0EC` |
| Body text | `#B0B0C8` | `#3A3A55` |

The brand primary `#4F3FFF` is **identical in both themes** — the visual thread connecting every surface.

## Using with AI (Claude)

Drop `SKILL.md` into a Claude Project as a project file. Every conversation will automatically apply Fastn brand.

## Version History

| Version | Date | Notes |
|---|---|---|
| 1.0 | Feb 2025 | Initial release — unified dark/light system, Electric Indigo primary |

---

**fastn.ai**
