# Project Summary

## One-Sentence Summary

Built an AI-assisted content operations studio for Xiaohongshu that combines competitor analysis, inspiration memory, content generation, publishing workflows, comment-to-lead automation, and local scheduling.

## Problem

Operators often work across disconnected tools:

- browsing competitor content manually
- copying good ideas into notes
- drafting content in separate AI tools
- posting manually
- following up with comments and messages by hand

That workflow is repetitive, hard to scale, and difficult to turn into a reusable system.

## Solution

I built a monorepo-based workbench that brings these steps together:

- analyze competitor posts and comments
- save useful patterns into a memory layer
- use that memory during AI-assisted content generation
- publish through browser automation
- monitor comments and private messages
- turn interactions into leads and topic ideas

## My Role

End-to-end builder.

I designed the flow, implemented the web app, wired the automation, integrated Gemini, built local fallbacks, and cleaned the project into a public-facing portfolio repository.

## Interesting Technical Decisions

### Browser automation instead of pretending there is a stable public API

Some platform flows were too fragile to rely on private web endpoints alone.
I used Playwright-driven workflows and Python scraping fallbacks where that was more robust.

### Inspiration memory instead of one-off prompting

Rather than generating content from a blank prompt each time, I built a local memory file that stores competitor insights and reuses them during generation.

### Workspace isolation

I added workspace-aware memory and topic storage so different content directions or accounts would not contaminate each other.

### Local demo fallback

Because remote auth and storage dependencies are not always available in demo environments, I added local JSON-backed fallbacks for lead and monitor flows.

## What I Would Improve Next

- add stronger E2E test coverage for publish and monitor flows
- make account and workspace switching more explicit in the UI
- reduce platform-specific selector fragility
- package parts of the automation layer into cleaner standalone services
