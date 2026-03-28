# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Insta-Haul is a hauling business. This repo contains:
- **brand/** — Logo and brand assets
- **docs/** — Private local business documents (not committed to any remote)
- **website/** — Frontend website (to be built)

## Repo Structure (Planned)

```
brand/
  images/        # SVG logos and other brand assets
docs/            # Private local documents — never commit sensitive content
website/
  index.html     # Homepage
  css/
    style.css    # All styles; CSS custom properties at :root
  images/        # Web-optimized images (separate from brand source files)
```

## Current Priorities

1. **Website frontend** — Build out `website/index.html` and `website/css/style.css`
2. **Private docs** — Maintain local business documents in `docs/` (kept out of any remote via .gitignore)

## Brand

- Colors: `--orange: #D94F00`, `--orange-mid: #F28C00`, `--yellow: #F5C200`, `--dark: #1A1A1A`
- Font: `'Trebuchet MS', 'Franklin Gothic Medium', Arial, sans-serif`
- Tagline: **FAST. RELIABLE. HAULING.**
- `brand/images/insta_haul_logo.svg` — Full stacked logo
- `brand/images/insta-haul-logo-small.svg` — Icon/horizontal lockup

## Website

Plain HTML/CSS — no build step, no dependencies.

- Entry point: `website/index.html`
- Styles: `website/css/style.css` — CSS custom properties defined in `:root`
- Images referenced via relative path `../brand/images/`
- Open `website/index.html` directly in a browser to preview

**To add a new page:** copy `index.html`, adjust the `<nav>` active state and content. Shared styles live in `style.css`.

## Private Documents

The `docs/` folder holds sensitive local business documents (contracts, pricing, contacts, etc.). Always `.gitignore`d — never commit or push this folder.
