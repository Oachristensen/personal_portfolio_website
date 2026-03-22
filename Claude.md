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
- `index.html` — landing/fork page. Two paths: Engineering (work.html) and Maker (maker.html)
- `work.html` — professional portfolio: projects, background, resume, professional contact
- `maker.html` — community/hobbyist: tutorials, build logs, casual contact (Discord, etc.)
- `style.css` — shared stylesheet with CSS custom properties (used by all pages)
- `projects/` — individual project detail pages (to be added)

## Audience Routing
The PCB business card QR code can point to index.html (self-select) or directly to work.html / maker.html depending on context. At OpenSauce, industry people get the work path, makers get the maker path.

## Conventions
- Use CSS custom properties from `:root` for all colors
- `.section-label` for section headers (mono, uppercase, light)
- `.marker` class for yellow highlighter effect on inline text
- `.status-tag.now` for current/active items (red, with arrow)
- `.note` for italic pencil-gray annotations on cards
- Keep it semantic — no div soup
- No JavaScript unless absolutely necessary
- Tone: direct, specific, not trying too hard
