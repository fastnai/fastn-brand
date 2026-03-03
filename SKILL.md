# Fastn Brand Skill

You are working on a project for **Fastn** (fastn.ai) — a developer-first integration platform. Apply these brand guidelines to every design, copy, and code decision.

## Identity

- **Name**: Fastn — always lowercase "fastn" in logos, title case "Fastn" in prose
- **Tagline**: Connect everything, ship faster
- **Personality**: Fast, precise, developer-friendly, quietly confident

## Colors

| Token | Hex | Usage |
|---|---|---|
| `--brand` | `#6C5CE7` | Primary — CTAs, links, focus rings, key UI elements |
| `--brand-hover` | `#5A4CD6` | Hover and pressed states |
| `--brand-light` | `#8F85E8` | Tags, labels, secondary accents |
| `--accent-violet` | `#A78BFA` | Gradient endpoint only — never as a standalone color |
| `--success` | `#10B981` | Positive / success states |
| `--warning` | `#F59E0B` | Warning / caution states |
| `--error` | `#EF4444` | Error / destructive states |

**Gradient**: `linear-gradient(135deg, #6C5CE7, #A78BFA)` — use sparingly for hero art, avatars, decorative accents. Never for body text or large surfaces.

## Typography

- **Sans**: Geist (weights 400–800) — headings, display, UI labels
- **Body**: Inter (weights 400–600) — body text, paragraphs, long-form content
- **Mono**: Geist Mono — code blocks, technical content, data
- **Display**: 96px, Geist weight 800, letter-spacing -0.04em
- **Headings**: Geist weight 700, letter-spacing -0.02em
- **Body text**: 16px, Inter weight 400, line-height 1.7

## Themes

The brand uses a dual-theme system. The primary color `#6C5CE7` stays identical in both.

### Dark (marketing, docs, landing pages)
| Surface | Value |
|---|---|
| Background | `#101014` |
| Card | `#18181E` |
| Border | `#2A2A36` |
| Body text | `#A0A0B8` |
| Headings | `#E4E4EC` |

### Light (app, dashboard, tools)
| Surface | Value |
|---|---|
| Background | `#FFFFFF` |
| Card | `#F5F5FA` |
| Border | `#E0E0EC` |
| Body text | `#3A3A55` |
| Headings | `#111118` |

## Product UI Palette

The product uses a separate warm-neutral palette. Electric Indigo appears **only** on the primary CTA button. Brand gradient is **prohibited** in product UI.

### Key Rules
1. `#6C5CE7` appears ONLY on the primary CTA. Nowhere else.
2. All grays use warm/brown undertones. Never blue-gray, never cool-gray.
3. Selection = subtle background shift + border darkening — not color.
4. Checkboxes are neutral (charcoal/warm gray) — never brand-colored.
5. Brand gradient (`#6C5CE7`→`#A78BFA`) is prohibited in product UI. Marketing only.
6. Semantic colors (success, warning, error, info) remain unchanged.

### Light Mode (Warm)
| Token | Hex | Usage |
|---|---|---|
| Background | `#FAF9F7` | Warm white |
| Card / Surface | `#FFFFFF` | |
| Card Selected | `#F5F4F0` | Warm selection tint |
| Section BG | `#F0EEE8` | |
| Border Default | `#E8E5DE` | |
| Border Selected | `#D4D0C8` | Softer emphasis |
| Heading Text | `#1A1816` | High-contrast warm black |
| Body Text | `#6F6B66` | |
| Muted / Placeholder | `#A8A49D` | |
| Checkbox Checked | `#3D3B37` | Deep charcoal, NOT brand |
| Checkbox Empty | `#D4D0C8` | |
| Primary CTA | `#6C5CE7` | Only chromatic element |
| Send / Icon BG | `#EEEDEA` | |
| Send / Icon Fill | `#8A8680` | |

### Dark Mode (Warm Dark)
| Token | Hex | Usage |
|---|---|---|
| Background | `#1A1918` | Warm brown undertone, never pure black |
| Card / Surface | `#222120` | |
| Card Selected | `#272622` | |
| Border Default | `#2B2A27` | |
| Border Selected | `#3E3D38` | |
| Heading Text | `#E3E1DA` | |
| Body Text | `#918F86` | |
| Muted / Placeholder | `#605E56` | |
| Checkbox Checked | `#A8A69E` | Warm light gray |
| Checkbox Empty | `#3E3D38` | |
| Primary CTA | `#6C5CE7` | Only chromatic element |
| Send / Icon BG | `rgba(255,255,255,0.04)` | |
| Send / Icon Fill | `#807E75` | |

## Voice & Tone

### Principles
1. **Clear over clever** — no jargon for jargon's sake
2. **Confident, not arrogant** — state facts, skip the hype
3. **Technical precision with warmth** — respect the developer, be approachable
4. **Developer-first** — assume technical literacy, skip the hand-holding

### Tone by Context
- **Marketing**: Bold, energetic, forward-looking
- **Documentation**: Precise, patient, example-driven
- **Error messages**: Calm, actionable, no blame
- **General**: Direct, helpful, quietly confident

### Vocabulary
**Prefer**: connect, integrate, automate, ship, build, fast, simple, powerful
**Avoid**: leverage, synergy, disrupt, revolutionary, game-changing, seamless, cutting-edge

### Writing Rules
- Use active voice
- Lead with the benefit, not the feature
- Short sentences. Short paragraphs.
- Use "you" — talk to the reader directly
- Code examples over abstract explanations
- Sentence case for headings (not Title Case)

## Logo Usage

- Use the wordmark (icon + "fastn") for primary placement
- Use the icon mark alone only when the brand is already established in context
- Minimum clear space: equal to the height of the "f" in the wordmark
- Never stretch, rotate, recolor, or add effects to the logo
- On dark backgrounds: white logo. On light backgrounds: black logo.

## Spacing & Layout

- Base unit: 4px grid
- Border radius: 8px (default for cards/buttons), 9999px for pills
- Use generous whitespace — let content breathe
- Maximum content width: 1200px for marketing, 1400px for dashboards
