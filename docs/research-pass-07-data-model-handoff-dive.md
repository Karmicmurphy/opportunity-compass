# Research Pass 07 - Data Model and Handoff Dive

Date: 2026-07-02

## Purpose

This pass checks whether the research is ready to hand to a builder.

It focuses on data model, app behavior, and what should happen next.

## Core finding

Opportunity Compass now has enough information to build a v0.1 prototype.

More broad research is not needed before prototyping.

The next productive work is converting the docs into:

- seed data
- app screens
- static prototype
- admin mock flow
- clickable cards

## Required build inputs now available

The repo now contains:

- README
- product spec
- screen list
- opportunity card template
- sample opportunities
- Salvage Picks
- source map
- research workflow
- Artifact Compass salvage method
- research pass findings
- database schema
- builder handoff

## Prototype data model

For v0.1, use JSON files instead of a real database.

Recommended seed files:

- data/opportunities.json
- data/salvage-picks.json
- data/categories.json
- data/risk-labels.json
- data/daily-top-five.json

## Prototype behavior

### User side

Users should be able to:

- view landing page
- fill intake form
- browse opportunity cards
- filter by verdict
- filter by beginner fit
- filter by category
- open detail page
- save a card locally
- view Salvage Picks
- view Daily Top 5
- view pricing page

### Admin side

Admin should be able to:

- paste raw opportunity text into a mock form
- see a draft card layout
- edit fields manually
- assign verdict
- assign risk labels
- mark Salvage Pick
- approve or reject draft

For v0.1, admin actions can be mock state only.

## Data fields required in JSON

Each opportunity should include:

- id
- title
- category
- source_type
- beginner_fit
- verdict
- estimated_pay_range
- estimated_time
- tools_needed
- skills_needed
- hidden_buyer_pain
- what_this_really_means
- why_beginners_miss_it
- smallest_paid_offer
- suggested_first_message
- questions_to_ask
- deliverable_checklist
- red_flags
- green_flags
- risk_labels
- boundary_note
- where_to_find_buyers
- what_not_to_promise
- is_salvage_pick

## Builder instruction

Build the product as a working prototype first.

Do not add:

- scraping
- real integrations
- authentication
- payment processing
- real private data imports
- auto-apply
- auto-message

## Best next step

Create the prototype seed data and then hand it to a builder.

Recommended next files:

- data/opportunities.json
- data/salvage-picks.json
- data/categories.json
- data/risk-labels.json
- docs/prototype-build-prompt.md

## Stop decision

Stop broad research for now.

Seven passes produced enough actionable product structure.

Additional passes should only happen when there is a specific build gap, not just because more research is possible.
