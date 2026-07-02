# AGENTS.md

## Project

Opportunity Compass is a plain-English opportunity translator and bullshit filter for small AI-enabled work, beginner-friendly freelance tasks, hidden niche gigs, and small-business support packages.

## Core rule

Build the v0.1 product shell first.

Do not turn this into a certification engine, scraping platform, payment system, or full backend.

## Current build goal

Create a mobile-first prototype using static seed data.

The prototype should let a user:

- view a landing page
- fill a simple intake form
- browse opportunity cards
- filter by verdict, beginner fit, category, and risk label
- open a card detail page
- save and unsave cards locally
- view Salvage Picks
- view Daily Top 5
- view a pricing mockup
- use mock admin import and review pages

## Data

Use the JSON seed files in `data/`:

- `data/opportunities.json`
- `data/salvage-picks.json`
- `data/categories.json`
- `data/risk-labels.json`
- `data/daily-top-five.json`

Do not replace seed data with scraped data.

Do not add private data.

## FlashRiver boundary

FlashRiver / CERT-RIVER / PRISM-RIVER is a separate modular engine family.

Do not wire real FlashRiver into v0.1.

Opportunity cards may show FlashRiver-ready fields such as free tool stack, paid upgrade options, privacy boundary, module name, setup steps, and work module availability.

Twis Holo Workshop is private and must not be included in this public product.

## Banned from v0.1

Do not add:

- scraping
- auto-apply
- auto-message
- real payment processing
- real user accounts unless explicitly requested
- Gmail or Google Drive imports
- Twis Holo Workshop references
- real FlashRiver engine calls
- broad certification claims
- fake income promises
- unbounded agent workflows

## Design tone

Plain, blunt, practical, trustworthy.

No guru language.
No fake side-hustle hype.
No crypto-style neon scam look.

## Recommended stack

Use a simple, common web stack if starting from scratch:

- React or Next.js
- TypeScript if convenient
- static JSON data
- local state/localStorage for saved cards
- simple CSS or Tailwind if already configured

Avoid unnecessary dependencies.

## Quality checks

Before finishing:

- run install if needed
- run build or typecheck if available
- fix obvious errors
- verify JSON imports/load paths
- verify mobile layout is usable
- verify cards can be opened
- verify filters work
- verify saved cards work locally
- verify admin pages are clearly mock-only

## Stop conditions

Stop only for true blockers:

- missing repo permissions
- missing dependency setup that cannot be inferred
- required paid service or secret
- destructive file operation
- ambiguous product decision that would change scope

Do not stop for minor styling uncertainty.
Do not expand scope to avoid making a decision.

## Final response requirements

When done, summarize:

- files changed
- how to run locally
- checks run
- known limitations
- what should be built next
