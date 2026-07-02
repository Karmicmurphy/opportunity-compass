# Codex Task Packet - Opportunity Compass v0.1

## Mission

Build Opportunity Compass v0.1 as a mobile-first static-data web prototype.

This is a repo-contained build task.

## Product definition

Opportunity Compass is not a job board.

It is a plain-English opportunity translator and bullshit filter for small AI-enabled work, beginner-friendly freelance tasks, hidden niche gigs, and small-business support packages.

Core promise:

Find small AI gigs worth touching. Avoid the bullshit.

## Build fence

Build v0.1 only.

Allowed:

- landing page
- intake form
- opportunity feed
- card detail page
- Salvage Picks page
- Daily Top 5 page
- saved cards page
- pricing mockup page
- admin import mock page
- admin review mock page
- static JSON seed data
- local saved state
- FlashRiver-ready fields displayed as static workbench preview info

Banned:

- scraping
- auto-apply
- auto-message
- real authentication
- real payment processing
- real FlashRiver engine integration
- Twis Holo Workshop references
- Google/Gmail/Drive imports
- private data
- fake income promises

## Data source

Use these files:

- data/opportunities.json
- data/salvage-picks.json
- data/categories.json
- data/risk-labels.json
- data/daily-top-five.json

## Required user flow

A user should be able to:

1. land on the homepage
2. understand what the product does
3. go to the feed
4. filter cards
5. open a card
6. read what the opportunity really means
7. see risk labels and boundaries
8. see free tool stack and workbench preview fields
9. save a card
10. view saved cards
11. view Salvage Picks and Daily Top 5
12. view pricing

## Required admin mock flow

Admin should be able to:

1. paste raw opportunity text into a form
2. see a draft card layout
3. manually edit mock fields
4. assign verdict
5. assign risk labels
6. mark Salvage Pick
7. approve or reject mock draft

This can be local mock state only.

## Design direction

Mobile-first.
Card-based.
Plain language.
Trustworthy.
No fake guru style.
No income hype.
No clutter.

## FlashRiver display rule

Show FlashRiver-ready fields as static workbench preview information:

- free tool stack
- local option
- cloud option
- paid upgrade options
- privacy boundary
- license note
- security note
- module name
- setup steps
- export format
- human review step

Do not call a real FlashRiver engine.

## Done criteria

The task is done when:

- app runs locally
- feed loads cards from seed data
- filters work
- detail page works
- saved cards work locally
- Salvage Picks load
- Daily Top 5 loads
- pricing page exists
- admin mock pages exist
- README or run instructions are accurate
- build/typecheck passes if configured

## Final summary required

Report:

- what was built
- files changed
- how to run it
- checks run
- remaining limitations
- next best step
