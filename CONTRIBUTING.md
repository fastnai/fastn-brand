# Contributing

Thanks for considering a contribution to the Fastn brand system. This repo is the source of truth for how Fastn looks and sounds. Contributions should strengthen the system, not expand its surface area.

## What we accept

- Accessibility improvements (contrast, focus, screen reader, reduced motion)
- Performance improvements (perf budget below)
- Bug fixes (rendering issues, broken tokens, typos, dead links)
- Adapter exports (Tailwind config, Style Dictionary build, Figma library)
- Documentation that clarifies an existing rule (do/don't examples, edge cases)

## What we don't accept

- A second accent color or chromatic decoration outside the existing accent gradient
- A second typeface or icon family
- Em dashes in copy. Use periods, commas, or parentheses instead.
- Decorative gradients on text, large surfaces, or backgrounds (the gradient is reserved for the primary CTA)
- Hover states that change hue (use brightness or opacity)
- Drop shadows on text or cards (only the CTA glow is allowed)

If your change requires one of these, open an issue first so we can discuss whether the system needs to evolve.

## Development

The project is plain HTML and CSS. No build step.

```bash
git clone https://github.com/fastnai/fastn-brand.git
cd fastn-brand
python3 -m http.server 8000
open http://localhost:8000/fastn-brand-system.html
```

Edit `fastn-brand-system.html`, `tokens.css`, or `tokens.json` directly. Refresh the browser. There is no compile step.

### Regenerating the share image

`og.html` is the source for `og.png` (1200x630 OpenGraph card). Regenerate the PNG when the wordmark, palette, or tagline changes:

```bash
node -e "
const puppeteer = require('puppeteer');
(async () => {
  const b = await puppeteer.launch();
  const p = await b.newPage();
  await p.setViewport({ width: 1200, height: 630, deviceScaleFactor: 2 });
  await p.goto('http://localhost:8000/og.html', { waitUntil: 'networkidle0' });
  await p.screenshot({ path: 'og.png' });
  await b.close();
})();
"
```

## Pull request checklist

Before opening a PR:

- [ ] The change keeps to one accent, one typeface, no em dashes.
- [ ] If you touched a token, you also updated `tokens.css`, `tokens.json`, the swatch in `fastn-brand-system.html`, the accessibility table, and `CHANGELOG.md`.
- [ ] If you added a color combination, you verified WCAG AA contrast and added the result to the accessibility table.
- [ ] Both dark and light themes render correctly.
- [ ] Page works at 320px viewport and at 200% zoom.
- [ ] Lighthouse a11y, best-practices, and SEO remain at 100. Performance stays at 90+.
- [ ] Color rows / interactive elements are keyboard-accessible with visible focus.
- [ ] No new dependencies. The repo is intentionally dependency-free.

## Versioning

This repo uses [semver](https://semver.org/). Any change to a token, font, or visual specification is a breaking change and ships as a major version. Adding a new state (e.g. a hint style) is minor. Bug fixes and content edits are patches. Every release is recorded in `CHANGELOG.md`.

## Voice

When writing copy for the site, README, or SKILL.md:

- Direct. Short sentences. Concrete nouns.
- Lead with the rule, then the why.
- Sentence case for headings. Title case only for the wordmark and proper nouns.
- Active voice, present tense.
- No marketing fog (revolutionary, supercharge, leverage, paradigm-shift).

## Reporting a security issue

If you find a security issue (XSS in the brand page, unsafe link, leaked credential in a logo asset), email security@fastn.ai instead of opening a public issue.
