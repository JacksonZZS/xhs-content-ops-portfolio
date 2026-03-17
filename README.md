# XHS Content Ops Studio Portfolio

Portfolio project: an AI-assisted Xiaohongshu content operations studio built with Next.js, Playwright, Gemini, Supabase, and Python scraping workflows.

## What This Project Demonstrates

This repository is a portfolio-focused presentation of a larger content operations system I built for Xiaohongshu workflows.

It demonstrates how I approach:

- productizing messy operator workflows into usable software
- browser automation with Playwright against real-world platform constraints
- AI-assisted content generation and structured analysis with Gemini
- local scheduling, lead capture, and multi-workspace state handling
- combining TypeScript web apps and Python scraping logic in one system

## Core Flows

### 1. Competitor Analysis

- search competitor notes
- fetch note details and comments
- generate structured analysis for hooks, persona, visual direction, and comment strategy
- save useful findings into a local inspiration memory

### 2. AI Content Creation

- take a topic and workspace context
- inject stored inspiration memory
- generate Xiaohongshu-ready titles, body copy, and tags
- support image analysis to improve fit between visuals and copy

### 3. Engagement Operations

- monitor comments from creator-facing flows
- classify comment intent
- convert comments into leads
- auto-reply to high-intent comments
- surface private-message and reply workflows

### 4. Publishing And Scheduling

- connect local logged-in accounts
- launch publishing flows with Playwright
- create scheduled posting tasks
- run due tasks through a local execution route

## Why I Built It

Most “social media tools” stop at dashboards or mock APIs.

I wanted to build something closer to real operational work:

- scrape competitor signals
- turn them into reusable insight
- feed those insights into AI generation
- publish and follow up using actual browser workflows

That made the project a good testbed for product design, automation reliability, local operator tooling, and LLM integration.

## Engineering Highlights

- Next.js App Router workbench with focused API routes
- Google Gemini integration for generation, analysis, and reply suggestions
- Playwright-based automation for publish, comment, and message flows
- Python scraper fallback for flows where direct web APIs are fragile
- local JSON fallback stores for demo mode when remote dependencies are unavailable
- workspace-aware memory and topic backlog so multiple content directions stay separated

## Tech Stack

- Next.js
- React
- TypeScript
- Playwright
- Python
- Supabase
- Google Gemini
- pnpm / Turborepo

## Repo Structure

```text
portfolio/
├── README.md
├── PROJECT_SUMMARY.md
├── RESUME_BULLETS.md
└── CASE_STUDY.md
```

## Best Way To Review This Project

If you are reviewing this as a hiring manager or interviewer, the best order is:

1. read `PROJECT_SUMMARY.md`
2. scan `CASE_STUDY.md`
3. read `RESUME_BULLETS.md`
4. then open the main source repository

## Main Source Repository

The full implementation lives in the main codebase this portfolio repo was derived from.

This portfolio version exists to make the project easier to review during hiring conversations.
