# Fastn Brand Skill

You are working on a project for Fastn (fastn.ai), a platform for trustworthy agents and high-value workflows. Apply these brand guidelines to every design, copy, and code decision.

## Philosophy

Color is punctuation, not prose. One accent (the indigo gradient) carries every primary action. Everything else is neutral grayscale. Hierarchy comes from weight and spacing, never from a second color.

If a design feels visually busy, the fix is almost always to remove color, not add it.

## Identity

- Name: Fastn. Always lowercase "fastn" in logos and product UI. Title case "Fastn" in prose.
- Tone: Direct, confident, without ceremony. Engineer briefing a teammate.
- We sell trust. Every visual choice should feel calm, deliberate, and high-signal.

## Color

### Accent (the only chromatic color)

| Token | Value | Use |
|---|---|---|
| `--accent-1` | `#6C5CE7` | Gradient start, focus rings |
| `--accent-2` | `#A78BFA` | Gradient end, inline link color |
| Gradient | `linear-gradient(90deg, #6C5CE7, #A78BFA)` | Primary CTA only |
| Glow | `0 0 28px rgba(124, 92, 231, 0.45)` | Outer glow on primary CTA |

The accent appears on three things, nothing else:

1. The primary CTA button (gradient fill plus glow).
2. Inline links inside body text (solid `--accent-2`).
3. Focus rings on interactive elements.

It must not appear on: section labels, badges, eyebrow tags, hover states for non-action elements, decorative dividers, icons, or background tints.

### Dark theme (default)

| Surface | Hex |
|---|---|
| Background | `#18181B` |
| Surface 1 (cards, inputs) | `#1F1F23` |
| Surface 2 (hover) | `#26262B` |
| Border | `#2A2A30` |
| Border high | `#3A3A42` |
| Text 1 (headings) | `#FFFFFF` |
| Text 2 (body) | `#BDBDC4` |
| Text 3 (supporting) | `#8A8A92` |
| Text 4 (disabled, non-text) | `#5C5C64` |

### Light theme

| Surface | Hex |
|---|---|
| Background | `#FFFFFF` |
| Surface 1 | `#F4F4F6` |
| Surface 2 | `#EAEAEE` |
| Border | `#E4E4E8` |
| Border high | `#CFCFD5` |
| Text 1 | `#18181B` |
| Text 2 | `#44444A` |
| Text 3 | `#6E6E76` |
| Text 4 | `#A4A4AC` |

### Semantic (sparingly)

| Token | Hex | Use |
|---|---|---|
| `--success` | `#10B981` | Positive states only |
| `--warning` | `#F59E0B` | Caution states only |
| `--error` | `#EF4444` | Destructive, error states only |

## Typography

Inter, throughout. No secondary or monospace typeface in brand surfaces. Inter weights 400, 500, 600, 700.

| Role | Size | Weight | Tracking |
|---|---|---|---|
| Display | 44 | 700 | -0.03em |
| H1 | 32 | 700 | -0.025em |
| H2 | 24 | 700 | -0.02em |
| H3 | 18 | 600 | -0.005em |
| Body | 16 | 400 | normal |
| Small | 14 | 400 | normal |

For technical documentation, monospace is allowed inside code blocks only. Use the platform default (`ui-monospace`, no custom face).

## Logo

- Use the wordmark for marketing, web, and documentation.
- Use the icon mark (`fastn-icon-rounded.jpg`) for compact placements: avatars, favicons, app icons, sign-in cards.
- White wordmark on dark backgrounds, black wordmark on light. Use `filter: invert(1)` on the PNG, or use a colored variant.
- The icon-rounded asset is self-contained (dark square plus white icon). Use as-is on any background.
- Never recolor, stretch, rotate, or add effects to the logo.
- Minimum clear space equal to the height of the "f" in the wordmark.

## Components

### Primary CTA

```html
<button class="btn btn-primary">Connect agent</button>
```

```css
.btn-primary {
  background: linear-gradient(90deg, #6C5CE7, #A78BFA);
  color: #FFFFFF;
  box-shadow: 0 0 28px rgba(124, 92, 231, 0.45);
  padding: 16px 20px;
  border-radius: 8px;
  font-weight: 600;
}
.btn-primary:hover { filter: brightness(1.05); box-shadow: 0 0 40px rgba(124, 92, 231, 0.45); }
```

### Secondary buttons (passkey, Google, Microsoft)

```css
.btn-secondary {
  background: var(--s1);
  color: var(--t1);
  border: 1px solid var(--border);
  padding: 16px 20px;
  border-radius: 8px;
  font-weight: 600;
}
```

### Inputs

```css
.input {
  background: var(--s1);
  border: 1px solid var(--border);
  border-radius: 8px;
  padding: 14px 16px;
  color: var(--t1);
}
.input:focus {
  border-color: var(--accent-1);
  box-shadow: 0 0 0 3px rgba(108, 92, 231, 0.20);
  outline: none;
}
```

### Inline links

```css
a {
  color: var(--accent-2);
  text-decoration: none;
  font-weight: 600;
}
a:hover { text-decoration: underline; text-underline-offset: 3px; }
```

## Voice and tone

### Principles

1. Direct over decorated. Short sentences. Concrete nouns. No marketing fog.
2. Specific over sweeping. "Reduces tool-call latency by 60%" beats "blazing fast."
3. Verbs over adjectives. If you can't show it doing something, cut it.
4. One idea per sentence. If a sentence has two commas and an em dash, it's two sentences.

### We say

- Trustworthy agents for high-value workflows.
- Compress tool chains. Aggregate actions.
- Decisions you can audit.

### We don't say

- Revolutionary. Game-changing. Paradigm-shift.
- Unlock the power of. Supercharge. Leverage.
- The future of AI is here.

### Mechanics

- Sentence case for UI strings and headings. Title case for the wordmark and proper nouns.
- Use "you," talk to the reader directly.
- Code examples over abstract explanations.
- Active voice, present tense.
- Do not use em dashes. Use periods, commas, or parentheses instead.

## Spacing and layout

- Base unit: 4px grid.
- Border radius: 8px for inputs and buttons, 14px for cards, 9999px for pills and avatars.
- Use generous whitespace. Let content breathe.
- Narrow centered columns (around 560px) for read-heavy surfaces. Wider only when content demands it.

## Don't list

- A second accent color.
- A second typeface.
- Decorative gradients on text or backgrounds.
- Em dashes in copy.
- Title Case headings.
- Drop shadows on text or cards (the only shadow allowed is the CTA glow).
- Border colors that aren't from the surface scale.
- Hover states that change hue.
