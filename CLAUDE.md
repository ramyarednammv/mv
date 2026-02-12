# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Mindvalley marketing landing pages and email campaign repository. Static HTML/CSS sites for masterclass programs, newsletters, and email sequences deployed via Vercel.

## Tech Stack

- Pure HTML/CSS (no JavaScript framework)
- Vercel for hosting (automatic deployment on push to main)
- No build process, bundling, or dependencies

## Deployment

Push to `main` branch triggers automatic Vercel deployment. Manual deployment available via:
```bash
npx vercel
```

## Directory Organization

- **CLC/** - Certified Life Coach 2026 email sequences
- **AI Accelerator/** - AI-focused newsletter landing pages
- **Manifesting masterclassses/strategy-page/** - Multi-masterclass marketing pathway
- **Vishen's Newsletter/** - Newsletter archives
- **Entrepreneurship & AI masterclasses/** - Masterclass transcripts

Each program has its own directory. Landing pages are standalone HTML files with embedded CSS.

## Styling Patterns

Landing pages use consistent patterns:
- Dark themes with gradient backgrounds (purple/pink or orange/amber palettes)
- CSS custom properties for color theming
- Flexbox and CSS Grid for responsive layouts
- Backdrop filters and smooth transitions
- Mobile-first responsive design

## Vercel Configuration

Each deployable directory contains:
- `vercel.json` - SPA routing configuration (routes all paths to index.html)
- `.vercel/project.json` - Project ID linking

## Content Structure

- Landing pages: Self-contained HTML files (800-2400 lines typically)
- Transcripts: Plain text files for masterclass content
- Data exports: CSV files from Airtable for email/newsletter archives
- Strategy docs: Markdown files for campaign planning
