# Z.ai / GLM Marathon Mission Packet - Opportunity Compass v0.1

## Mission

Build Opportunity Compass v0.1 as a complete, download-ready, mobile-first web prototype.

Use the repo docs and data. Work autonomously. Do not require human babysitting for normal implementation details.

## Product

Opportunity Compass is a plain-English opportunity translator and bullshit filter for small AI-enabled work, beginner-friendly freelance tasks, hidden niche gigs, and small-business support packages.

It is not a generic job board.
It is not a guru funnel.
It is not a scraping platform.

Core promise:

Find small AI gigs worth touching. Avoid the bullshit.

## Build only v0.1

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
- local save state
- FlashRiver-ready workbench preview fields
- README/run instructions
- build report

Banned:

- scraping
- auto-apply
- auto-message
- real payment processing
- real authentication unless already scaffolded and simple
- real FlashRiver engine integration
- Twis Holo Workshop references
- private data imports
- Gmail/Drive imports
- broad certification claims
- fake income promises
- large backend architecture

## Repo sources to read first

Read these before building:

- README.md
- AGENTS.md
- docs/CURRENT_STATE_2026-07-02.md
- docs/product-spec.md
- docs/screen-list.md
- docs/database-schema.md
- docs/flashriver-integration-note.md
- docs/flashriver-invention-scope.md
- data/opportunities.json
- data/salvage-picks.json
- data/categories.json
- data/risk-labels.json
- data/daily-top-five.json

## Required sub-agent checks

Use internal review passes or sub-agents if available:

### Product Scope Guard

Check that the build stays inside v0.1 and does not add banned features.

### UX Reviewer

Check mobile layout, card readability, navigation, and plain-language flow.

### Data Shape Checker

Check that JSON data loads correctly and fields display where useful.

### Safety / Trust Reviewer

Check that there are no fake income promises, no broad certification claims, no private data, and no Twis Holo Workshop leakage.

### Bug Fixer

Run the app, find broken routes/imports/build errors, and fix them.

### Packaging Auditor

Make sure the final output is one clean project folder with source, data, README, run instructions, and build report.

## Work order

1. Inspect repo structure.
2. Choose simplest suitable web stack if no app exists.
3. Build pages and routes.
4. Load static JSON data.
5. Build card components.
6. Build filters.
7. Build detail page.
8. Build saved cards with local state.
9. Build Salvage Picks and Daily Top 5 pages.
10. Build pricing page.
11. Build admin import/review mock pages.
12. Add FlashRiver-ready workbench preview sections.
13. Run checks.
14. Fix errors.
15. Create final build report.
16. Package final project folder.

## Packaging rule

Final result must be one clean root folder.

Preferred final folder name:

opportunity-compass-v0.1

The folder should include:

- source code
- data files
- package file
- README
- run instructions
- build report

Prefer ZIP export.

If only TAR/TAR.GZ is available, the archive must contain one clean root project folder, not loose scattered files.

## Stop conditions

Stop only for real blockers:

- missing repo access
- required paid service or secret
- destructive action uncertainty
- ambiguous product decision that would change scope
- impossible build environment

Do not stop for styling uncertainty.
Do not ask for approval for normal implementation choices.
Do not expand scope to avoid a decision.

## Final answer required

When complete, report:

- what was built
- files changed
- how to run locally
- checks run
- packaging format
- known limitations
- next recommended version
