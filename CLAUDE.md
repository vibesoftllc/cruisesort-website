# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

CruiseSort is a pre-launch cruise search and comparison platform targeting US travelers. The site is a static HTML landing page hosted on GitHub Pages at `cruisesort.com`.

## Structure

This is a single-file static site — all HTML, CSS, and JavaScript lives in `index.html`. There is no build step, no framework, no package manager.

## Development

Open `index.html` directly in a browser. There is no dev server or build process.

To preview changes: open the file in a browser or use a simple local server:
```
python3 -m http.server 8000
```

## Design System

Colors are defined as CSS custom properties at the top of `index.html`:
- `--navy` / `--deep` / `--ocean`: background blues
- `--teal` / `--teal-light`: primary action color
- `--gold` / `--gold-light`: accent/highlight color
- `--white` / `--mist` / `--text`: typography

Fonts: Playfair Display (headings, serif) and DM Sans (body, sans-serif) loaded from Google Fonts.

## Deployment

Push to `main` — GitHub Pages auto-deploys. The `CNAME` file maps the custom domain `cruisesort.com`.

## Current State

The site is a "coming soon" landing page. The email signup form (`handleSignup`) is purely client-side with no backend — it just updates the UI. No actual email collection is wired up yet.
