# XHS Content Ops Studio

> Portfolio project: an AI-assisted Xiaohongshu content operations studio built with Next.js, Playwright, Gemini, Supabase, and Python scraping workflows.

## Overview

This repository is the portfolio-facing presentation of a larger engineering project I built around Xiaohongshu content workflows.

The goal was not just to build a dashboard. The goal was to turn a messy operator workflow into a coherent software system:

- analyze competitor content
- save reusable insight
- feed that insight into AI content generation
- publish through browser automation
- monitor comments and private messages
- turn engagement into leads and future content ideas

## What This Project Demonstrates

- product thinking translated into concrete workflows
- browser automation against real-world platform constraints
- LLM-assisted generation, analysis, and reply suggestion
- local scheduling and fallback-oriented system design
- multi-workspace handling for multiple accounts or content directions
- hybrid engineering across TypeScript web apps and Python scraping logic

## Key Workflows

### Competitor Analysis

- search competitor notes
- fetch note details and comments
- generate structured analysis for hooks, persona, visual direction, and comment strategy
- save useful findings into an inspiration memory

### AI Content Creation

- take a topic and workspace context
- inject saved inspiration into prompts
- generate Xiaohongshu-ready titles, body copy, and tags
- support image analysis to improve fit between visual assets and copy

### Engagement Operations

- monitor comments from creator-facing flows
- classify comment intent
- convert comments into leads
- auto-reply to high-intent comments
- support private-message reading and reply workflows

### Publishing And Scheduling

- connect local logged-in accounts
- launch publish flows with Playwright
- create scheduled posting tasks
- run due tasks through a local execution route

## Engineering Highlights

- Next.js App Router workbench with route-based workflows
- Google Gemini integration for copy generation, analysis, and reply suggestions
- Playwright automation for publishing, comment replies, and message flows
- Python scraper fallback where direct web API paths proved fragile
- local JSON fallback stores for demo and degraded modes
- workspace-aware memory and topic backlog to isolate multiple business lines

## Tech Stack

- Next.js
- React
- TypeScript
- Playwright
- Python
- Supabase
- Google Gemini
- pnpm / Turborepo

## Portfolio Review Guide

If you are reviewing this project during hiring, the fastest path is:

1. read [PROJECT_SUMMARY.md](./PROJECT_SUMMARY.md)
2. scan [CASE_STUDY.md](./CASE_STUDY.md)
3. read [CODE_TOUR.md](./CODE_TOUR.md)
4. scan [RESUME_BULLETS.md](./RESUME_BULLETS.md)
5. open the main implementation repository

## Main Implementation Repository

Full source code:

- [hk-lifestyle-matrix](https://github.com/JacksonZZS/hk-lifestyle-matrix)

This portfolio repository exists to make the project easier to review without forcing people to start from a large monorepo.

## Why I Built It

Most social-media tooling either stays at the dashboard layer or relies on unstable private APIs without serious fallback handling.

I wanted to build something closer to real operator work:

- scrape signals
- turn them into reusable operating insight
- feed those insights into AI generation
- publish and follow up through real browser workflows

That made the project a strong testbed for product design, automation reliability, and practical LLM integration.

## Additional Notes

- [PROJECT_SUMMARY.md](./PROJECT_SUMMARY.md): concise project framing
- [CASE_STUDY.md](./CASE_STUDY.md): deeper architecture and tradeoffs
- [CODE_TOUR.md](./CODE_TOUR.md): where to look in the codebase
- [RESUME_BULLETS.md](./RESUME_BULLETS.md): resume-ready phrasing
