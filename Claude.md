# Portfolio Site

Static HTML/CSS portfolio for Owen — embedded systems / hardware engineering.

## Stack
- Plain HTML + CSS (no frameworks, no build step)
- Deployed on Vercel from GitHub
- Google Fonts: IBM Plex Mono + Instrument Serif

## Aesthetic
- Engineering notebook / graph paper — green gridlines, off-white paper, red margin line
- Warm and approachable, not corporate. Casual but technically credible.
- Serif headings (Instrument Serif), monospace body text (IBM Plex Mono)
- Color vocabulary: ink (dark text), pencil (muted), red-ink (accents/current), blue-ink (links/tags), highlight (yellow marker)

## Structure
- `index.html` — main landing page. The professional portfolio: projects, background, resume, professional contact. Links out to the maker page (nav + a pointer in the contact section).
- `maker.html` — community/hobbyist: tutorials, build logs, casual contact (Discord, etc.). Reached via the "Maker" link from `index.html`.
- `style.css` — shared stylesheet with CSS custom properties (used by all pages)
- `projects/` — individual project detail pages

## Audience Routing
There's no self-select fork anymore — `index.html` (the professional portfolio) is the front door, so recruiters and engineers land on the work directly, with the maker side one click away. The PCB business card QR code points to the bare domain (→ `index.html`); it can still deep-link straight to `maker.html` for maker-context handouts (e.g. at OpenSauce).

## Conventions
- Use CSS custom properties from `:root` for all colors
- `.section-label` for section headers (mono, uppercase, light)
- `.marker` class for yellow highlighter effect on inline text
- `.status-tag.now` for current/active items (red, with arrow)
- `.note` for italic pencil-gray annotations on cards
- Keep it semantic — no div soup
- No JavaScript unless absolutely necessary
- Tone: direct, specific, not trying too hard
