# Plan: Soften Dark Theme (Completed)

Goal: Reduce eye strain in dark theme by softening contrast and lifting surfaces from near-black.

## What changed

### 1. Dark theme surfaces — lifted and softened

| Token | Before | After | Why |
|-------|--------|-------|-----|
| `--bg` | `#09090E` | `#101014` | Lifted from near-black, less harsh |
| `--s1` / card | `#111118` | `#18181E` | Better surface separation |
| `--s2` | `#18181F` | `#1E1E26` | Neutral mid-surface |
| `--s3` | `#22222C` | `#262630` | Softer raised surface |
| `--border` | `#2E2E3A` | `#2A2A36` | Less visual noise |
| `--border-hi` | `#3E3E50` | `#38384A` | Softer hover border |

### 2. Text — reduced glare

| Token | Before | After | Contrast | Why |
|-------|--------|-------|----------|-----|
| `--t1` heading | `#FFFFFF` | `#E4E4EC` | ~12.8:1 AAA | Off-white eliminates glare |
| `--t2` body | `#B0B0C8` | `#A0A0B8` | ~6.4:1 AA | Softer, still very readable |
| `--t3` muted | `#60607A` | `#6E6E84` | ~3.5:1 | Slightly lifted for readability |

### 3. Hero glow — toned down

Radial gradient opacity reduced from 0.12 to 0.08.

## Files modified

- `tokens.css` — dark theme CSS variables
- `tokens.json` — source design tokens
- `fastn-brand-system.html` — CSS variables, color swatches, accessibility examples
- `SKILL.md` — brand skill documentation
- `README.md` — quick-reference color table

## Brand color softening

| Token | Before | After |
|-------|--------|-------|
| `--brand` | `#4F3FFF` (electric indigo) | `#6C5CE7` (soft indigo) |
| `--brand-hover` | `#3B2DE8` | `#5A4CD6` |
| `--brand-light` | `#7B6FFF` | `#8F85E8` |
| `--accent` | `#FF4D8D` (hot pink) | `#A78BFA` (soft violet) |
| gradient | purple→pink | `#6C5CE7`→`#A78BFA` (tonal purple) |

## What stayed the same

- Light theme tokens
- Product UI warm palette (both light and dark)
- Typography, spacing, radius, motion
- Semantic colors (success, warning, error, info)
- Logo usage rules
