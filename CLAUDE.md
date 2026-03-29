# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Pure static HTML typewriter-style editor website. No build system, no npm, no framework.

## Structure

- `index.html` — Main editor (contenteditable div, download via print, samples link)
- `samples.html` — Sample letters showcase
- `sample_*.html` — Individual sample letter pages
- `*.woff2`, `*.ttf` — Web fonts (Special Elite, Huiwen Mincho)

## Commands

No build commands. Open `index.html` directly in a browser to develop.

## Notes

- All pages share identical top-bar styling and inline SVG logo
- Fonts are loaded from local files with `font-display: fallback`
- Paper color toggle (white/gray) is implemented via inline JS on all pages
- Download is handled via `window.print()` which targets the browser print dialog
