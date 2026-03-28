# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Insta-Haul is a hauling business. This repo contains:
- **brand/** — Logo and brand assets
- **docs/** — Private local business documents (not committed to any remote)
- **index.html / css/** — Website, served from repo root for GitHub Pages

## Repo Structure

```
brand/
  images/        # SVG logos and other brand assets
css/
  style.css      # All styles; CSS custom properties at :root
docs/            # Private local documents — never commit sensitive content
index.html       # Homepage (repo root, served by GitHub Pages)
website/         # Original working copy — root files are the live version
```

## Current Priorities

1. **Website frontend** — Build out `website/index.html` and `website/css/style.css`
2. **Private docs** — Maintain local business documents in `docs/` (kept out of any remote via .gitignore)

## Brand

- Colors: `--orange: #D94F00`, `--orange-mid: #F28C00`, `--yellow: #F5C200`, `--dark: #1A1A1A`
- Font: `'Trebuchet MS', 'Franklin Gothic Medium', Arial, sans-serif`
- Tagline: **FAST. RELIABLE. HAULING.**
- `brand/images/insta_haul_logo.svg` — Stacked logo (icon + wordmark + tagline); `-haul` is white for use on dark backgrounds
- `brand/images/insta-haul-logo-small.svg` — Horizontal lockup (small icon + wordmark); `-haul` is `#1A1A1A` for use on light backgrounds

## Website

Plain HTML/CSS — no build step, no dependencies.

- Entry point: `index.html` (repo root)
- Styles: `css/style.css` — CSS custom properties defined in `:root`
- Images referenced via relative path `brand/images/`
- Hosted on GitHub Pages at `loronajay.github.io/insta_haul`
- Open `index.html` directly in a browser to preview locally

**To add a new page:** copy `index.html`, adjust the `<nav>` active state and content. Shared styles live in `style.css`.

## Private Documents

The `docs/` folder holds sensitive local business documents (contracts, pricing, contacts, etc.). Always `.gitignore`d — never commit or push this folder.
