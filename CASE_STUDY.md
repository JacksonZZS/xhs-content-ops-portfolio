# Case Study

## Goal

Turn a real social content workflow into a coherent engineering project rather than a collection of scripts.

## Workflow I Wanted To Support

1. find high-performing competitor content
2. understand why it works
3. save reusable patterns
4. generate new content with those patterns in mind
5. publish through a real account workflow
6. track comments and private messages
7. convert engagement into leads and future content ideas

## Architecture Overview

### Web layer

A Next.js workbench handles:

- content creation
- competitor review
- comment monitoring
- messages
- scheduling
- analytics

### Automation layer

Playwright handles browser-driven tasks such as:

- publishing
- comment replies
- message replies
- account-aware browser sessions

### Scraping layer

Python-based scraping is used where browser-side extraction is more reliable than direct endpoint integration.

### AI layer

Gemini is used for:

- copy generation
- image analysis
- competitor breakdowns
- comment classification
- reply suggestions

## Key Tradeoffs

### Speed vs reliability

Direct web APIs can be faster, but browser-based automation and scraping often proved more resilient for unstable platform flows.

### Generality vs usability

I optimized for a usable operator workflow instead of a generalized framework first.

### Perfect architecture vs shipping

Some fallback layers exist because they made the demo and real operator flows more reliable, even if they are less elegant than a fully normalized service architecture.

## What This Shows About My Engineering Style

- I can translate workflow pain into system design
- I am comfortable blending product thinking with implementation detail
- I treat fallbacks and operational edges as part of the real system
- I care about making a project explainable, not just functional
