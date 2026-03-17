# Code Tour

This project is backed by a larger source repository:

- [hk-lifestyle-matrix](https://github.com/JacksonZZS/hk-lifestyle-matrix)

Below are the code areas worth reviewing first.

## 1. Create Workflow

File:

- `apps/web/src/components/create/create-workflow.tsx`

Why it matters:

- shows the main operator-facing flow
- ties topic input, AI generation, image handling, and publishing together
- demonstrates product flow design in the UI layer

## 2. Browser Automation Layer

File:

- `apps/web/src/lib/xhs/publisher.ts`

Why it matters:

- central Playwright integration for publish, comments, and messages
- handles logged-in local profiles
- contains multiple fallback paths for unstable platform behavior

## 3. Comment Monitor Service

File:

- `apps/web/src/lib/comments/monitor-service.ts`

Why it matters:

- turns raw engagement into structured operator actions
- classifies comments, stores leads, triggers auto-replies, and generates topic ideas
- demonstrates orchestration across AI, storage, and automation layers

## 4. Competitor Analysis Route

File:

- `apps/web/src/app/api/competitor/analyze/route.ts`

Why it matters:

- converts scraped notes and comments into structured analysis
- shows how I use LLM output for practical operator intelligence, not just generic text generation

## 5. Inspiration Memory

Files:

- `apps/web/src/lib/content-memory.ts`
- `apps/web/src/app/api/generate/route.ts`

Why it matters:

- demonstrates how useful competitor patterns are persisted and fed back into future generation
- shows a simple but effective retrieval-style workflow without overengineering

## 6. Python Scraper Fallback

Files:

- `apps/xhs-automation/src/scraper/content_scraper.py`
- `apps/xhs-automation/run_competitor_scraper.py`

Why it matters:

- shows how I added a browser-driven scraping fallback when direct endpoint paths became unreliable
- demonstrates cross-language integration between Python scraping and the Next.js app

## Suggested Review Order

1. `create-workflow.tsx`
2. `publisher.ts`
3. `monitor-service.ts`
4. `competitor/analyze/route.ts`
5. `content-memory.ts`
6. `content_scraper.py`
