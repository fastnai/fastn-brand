# Fastn Brand System

The official guidelines, design tokens, and logo assets for the Fastn brand. Color, type, logo, voice, and components in one place.

Live page: https://fastnai.github.io/fastn-brand/

## Philosophy

Color is punctuation, not prose. One accent (the indigo gradient) carries every primary action. Everything else is neutral grayscale. Hierarchy comes from weight and spacing, never from a second color.

## What's in the repo

| File | Purpose |
|---|---|
| `fastn-brand-system.html` | Interactive brand guidelines. Open in any browser. |
| `tokens.css` | CSS custom properties. Drop into any project. |
| `tokens.json` | Source-of-truth tokens. Style Dictionary / Figma / Tailwind importable. |
| `SKILL.md` | Project file for Claude. Adds brand context to AI-assisted work. |
| `logos/` | Logo files (wordmark PNG, icon PNG, social variants). |

## Quick start

Open the page locally:

```bash
git clone https://github.com/fastnai/fastn-brand.git
cd fastn-brand
open fastn-brand-system.html
```

Use the tokens in your project:

```html
<link rel="stylesheet" href="tokens.css">
```

```css
.button-primary {
  background: linear-gradient(90deg, var(--accent-1), var(--accent-2));
  color: var(--on-accent);
  box-shadow: 0 0 28px var(--accent-glow);
  border-radius: var(--r-2);
}
```

## At a glance

### Accent

| Token | Value | Use |
|---|---|---|
| `--accent-1` | `#6C5CE7` | Gradient start, focus rings |
| `--accent-2` | `#A78BFA` | Gradient end, inline links |
| `--accent-glow` | `rgba(124, 92, 231, 0.45)` | 28px outer glow on primary CTA |

The gradient `linear-gradient(90deg, #6C5CE7, #A78BFA)` is reserved for the primary CTA. Inline links use `--accent-2` (solid). Never apply the gradient to text, large surfaces, or decorative elements.

### Typography

Inter, weights 400 / 500 / 600 / 700. One typeface. Hierarchy from size and weight.

| Role | Size | Weight | Tracking |
|---|---|---|---|
| Display | 44 | 700 | -0.03em |
| H1 | 32 | 700 | -0.025em |
| H2 | 24 | 700 | -0.02em |
| H3 | 18 | 600 | -0.005em |
| Body | 16 | 400 | normal |
| Small | 14 | 400 | normal |

### Themes

Two themes, same restraint. The accent is identical in both. Surfaces flip.

| | Dark | Light |
|---|---|---|
| Background | `#18181B` | `#FFFFFF` |
| Surface 1 | `#1F1F23` | `#F4F4F6` |
| Border | `#2A2A30` | `#E4E4E8` |
| Heading | `#FFFFFF` | `#18181B` |
| Body | `#BDBDC4` | `#44444A` |
| Supporting | `#8A8A92` | `#6E6E76` |

## Using with Claude

Drop `SKILL.md` into a Claude project (or paste it as a system message). Every conversation in that project will follow Fastn brand guidelines by default.

## Logos

| File | Use |
|---|---|
| `logos/fastn-logo-740px.png` | Wordmark, large (2307 x 1611) |
| `logos/fastn-logo-400px.png` | Wordmark, web-ready (400 x 248) |
| `logos/fastn-icon-rounded.jpg` | Icon mark, rounded square (424 x 424) |
| `logos/fastn-icon-square.jpg` | Icon mark, square |
| `logos/fastn-icon-linkedin.jpg` | LinkedIn profile sized |

Rules:

- Use the wordmark for marketing surfaces. Use the icon for compact placements (avatars, favicons, sign-in screens).
- White wordmark on dark backgrounds, black wordmark on light backgrounds. Apply `filter: invert(1)` to the PNG, or use a colored variant.
- The icon-rounded asset is self-contained (dark square + white icon). Use as-is on any background.
- Never stretch, rotate, recolor, or add effects to the logo.
- Minimum clear space equal to the height of the "f" in the wordmark.

## Accessibility

Every shipped token combo passes WCAG 2.1 AA for its intended use:

| Pair | Ratio |
|---|---|
| Text 1 on Background | 16.9:1 (AAA) |
| Text 2 on Background | 9.1:1 (AAA) |
| Text 3 on Background | 5.0:1 (AA) |
| White on Indigo CTA | 4.8:1 (AA) |
| Indigo link on Background | 5.8:1 (AA) |

Focus rings use `box-shadow: 0 0 0 3px rgba(108,92,231,0.40)`. Reduced-motion preferences are honored. The page is keyboard-navigable.

## License

MIT. See [LICENSE](./LICENSE).

The Fastn name, wordmark, and icon are trademarks of Fastn. The code and tokens in this repository are MIT-licensed and free to reuse; the logo assets remain Fastn's trademarks and should only be used to refer to or integrate with Fastn.

## Contributing

This is the source of truth for the Fastn brand. Contributions that strengthen the system (token additions, accessibility improvements, framework adapters) are welcome. Contributions that introduce a second accent color, a second typeface, decorative gradients, or marketing fluff will not be accepted.
