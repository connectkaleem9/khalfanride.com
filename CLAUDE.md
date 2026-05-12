# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Business website for **khalfanride.com** — a professional service/ride business website. The goal is a fast, responsive, SEO-optimized static or SSR site.

## Tech Stack (to be decided / update as setup is finalized)

- **Framework**: Next.js (App Router) — update if different
- **Styling**: Tailwind CSS
- **Language**: TypeScript
- **Package Manager**: npm (or update to pnpm/yarn if changed)

## Common Commands

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Start production server
npm start

# Lint
npm run lint

# Type check
npx tsc --noEmit

# Run tests
npm test

# Run a single test file
npm test -- <path/to/test-file>
```

## Architecture

Update this section once the project scaffold is in place. Key things to document here:

- **Routing**: how pages/routes are organized
- **Data fetching**: where API calls or CMS queries live
- **Components**: shared vs page-specific split
- **Styles**: any global theme tokens or Tailwind config customizations
- **Environment variables**: which `.env` keys are required and what they control

## Skills / Slash Commands (`.claude/skills/`)

Invoke with `/skill-name` in any prompt:

| Skill | When to use |
|---|---|
| `/seo-audit` | Audit any page for technical SEO, on-page, structured data, bilingual issues |
| `/competitor-research` | Analyze a competitor URL or search for new ones, output gap analysis |
| `/content-planner` | Plan page content, blog topics, seasonal campaigns, WhatsApp broadcasts |

## AI Agents (`.claude/agents/`)

Invoke these with `@agent-name` in any prompt:

| Agent | When to use |
|---|---|
| `@copywriter` | Writing/editing any user-facing text, headlines, CTAs, FAQs |
| `@seo-optimizer` | Meta tags, JSON-LD schema, keyword strategy, page SEO audits |
| `@ui-designer` | Component design, Tailwind layouts, RTL/LTR support, color/type |
| `@whatsapp-booking` | WhatsApp CTA buttons, pre-filled message templates, booking widget |
| `@translator` | English ↔ Arabic translation with Islamic/cultural context |
| `@pricing-manager` | Route fares, pricing tables, `lib/pricing.ts` data, fare logic |

## Environment Variables

Copy `.env.example` to `.env.local` for local development. Required keys:

| Key | Purpose |
|-----|---------|
| `NEXT_PUBLIC_WA_NUMBER` | WhatsApp phone number in international format (e.g. `966XXXXXXXXX`) |
| `NEXT_PUBLIC_GA_ID` | Google Analytics measurement ID |
