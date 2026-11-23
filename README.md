# Kaizen Docs

**The public product report for [Kaizen](https://github.com/devvbuilds-png/Orchestral-AI): what it is, why it exists, how it's built, and where it's going.**

Live: https://kaizen-docs.vercel.app

## What it is / why I built it

Kaizen is a structured product knowledge base, and the product itself is hard to explain in a single landing-page headline. I wanted one place where someone (a recruiter, a collaborator, or a curious builder) could follow the whole story: the problem, the architecture, the honest trade-offs, and the roadmap.

This site is that place. It's written as a builder's report rather than marketing copy, with a short, readable page for each part of the story.

## Pages

| # | Route | Content |
|---|-------|---------|
| 01 | `/` | What is Kaizen |
| 02 | `/why` | The problem worth solving |
| 03 | `/build` | How it's built: pipeline, agents, stack, known gaps and debt |
| 04 | `/story` | How it started |
| 05 | `/roadmap` | What's live, in progress, and planned |

## Features

- Sidebar navigation with an active-page state and a mobile hamburger menu
- Reusable `StatusTable` component for live, in-progress and planned items on the roadmap
- Serif and mono type pairing (Lora + IBM Plex Mono via `next/font`)
- Static pages with no backend and no environment variables

## Tech stack

- Next.js 14 (App Router), React 18, TypeScript
- Tailwind CSS
- Deployed on Vercel

## Run locally

```bash
npm install
npm run dev      # http://localhost:3000
```

`npm run build`, `npm start` and `npm run lint` are also available.

## Project structure

```
app/          one folder per page (why, build, story, roadmap) + root layout and styles
components/   Sidebar, StatusTable
```

## Status

Live on Vercel; updated as Kaizen ships.
