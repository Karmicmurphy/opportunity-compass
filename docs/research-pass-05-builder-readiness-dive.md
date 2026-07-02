# Research Pass 05 - Builder Readiness Dive

Date: 2026-07-02

## Purpose

This pass turns the research into product structure for v0.1.

The goal is to make Opportunity Compass buildable without losing the original idea.

## Core finding

Opportunity Compass v0.1 should be a manual-curation prototype.

Do not build scraping first.
Do not build auto-apply.
Do not build buyer messaging.
Do not require paid APIs.
Do not require private data.

Build the card system, feed, Salvage Picks, and admin import flow first.

## v0.1 product rules

### 1. Manual first

The first version should use manually entered or pasted opportunities.

Reason: This protects quality, avoids platform problems, and lets the card format mature before automation.

### 2. Cards are the product

The valuable part is not the link. The valuable part is the translation.

Each card explains:

- what this really means
- hidden buyer pain
- beginner fit
- tools needed
- estimated pay/time
- smallest paid offer
- questions to ask
- deliverable checklist
- red flags
- green flags
- verdict

### 3. Salvage Picks are packages

Salvage Picks should not look like normal listings.

They should look like practical small service packages:

- Review Reply Pack
- FAQ Draft Pack
- Canva Cleanup Pack
- PDF to Spreadsheet Pack
- Workflow Map Pack

### 4. Risk labels are required

Every card should show risk labels or state why risk is low.

Recommended labels:

- Needs Clarification
- Scope Creep Risk
- Pay/Scope Mismatch
- Access Risk
- Sensitive Data Risk
- Expert Work Risk
- Platform Risk

### 5. Beginner fit must be honest

Do not call everything beginner-friendly.

Use:

- High: general writing, cleanup, formatting, simple review, owner-approved drafts
- Medium: workflow mapping, data cleanup, content review, task platforms
- Low: expert review, regulated domains, advanced coding, production automation

## Required v0.1 screens

1. Landing page
2. Intake form
3. Opportunity feed
4. Opportunity detail page
5. Salvage Picks page
6. Daily Top 5 page
7. Saved opportunities page
8. Admin import page
9. Admin review/edit page
10. Pricing mockup page

## Required v0.1 filters

- verdict
- beginner fit
- category
- estimated time
- estimated pay range
- tools needed
- Salvage Pick
- risk label

## Recommended card categories

- AI content review
- AI response evaluation
- AI training and task work
- local business AI help
- review replies
- FAQ drafts
- marketplace listing cleanup
- PDF and spreadsheet cleanup
- Canva cleanup
- social post batching
- workflow mapping
- customer message templates
- website copy cleanup
- AI video prompt/script prep
- domain expert AI evaluation
- trust and risk check

## Admin workflow

### Admin import page

Admin pastes:

- raw opportunity text
- source type
- source name
- original link placeholder
- notes

### Draft card generator

The system creates a draft card with:

- title
- category
- verdict
- beginner fit
- risk labels
- summary fields
- questions to ask
- deliverable checklist

### Admin review page

Admin can:

- edit card
- approve card
- reject card
- mark Touch
- mark Watch
- mark Trash
- mark Scam Risk
- mark Too Advanced
- publish to feed
- publish to Salvage Picks

## Suggested data structure changes

Add these fields to opportunities:

- risk_labels: array
- boundary_note
- where_to_find_buyers
- what_not_to_promise
- task_clarity_score
- deliverable_clarity_score
- beginner_fit_score
- pay_scope_fit_score
- trust_score
- risk_score
- is_package
- package_name

## Seed data for prototype

Use the current 12 sample opportunities and the 12 Salvage Picks.

Do not use raw scraped content.
Do not use private screenshots.
Do not use copied job posts.

## Build recommendation

Best first build:

- Next.js or React
- simple JSON seed data
- local state for saving cards
- static pages or simple mock backend
- no auth required for first demo
- admin pages can be mock-only in v0.1

## Not in v0.1

Do not build these yet:

- scraping
- auto-apply
- auto-message
- payment processing
- real user accounts
- browser extensions
- complex AI agents
- private Gmail import
- real Fiverr/Upwork integrations

## Next pass decision

At this point, the product is buildable at prototype level.

Further research is optional and should only be done if it answers a specific gap:

- competitor positioning
- pricing
- SEO/content strategy
- final data model
- prototype handoff
