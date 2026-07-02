# Builder Handoff

Use this document to hand Opportunity Compass to a builder such as Codex, Z.ai, Lovable, Replit, Bolt, Cursor, or a human developer.

## Build target

Build Opportunity Compass v0.1 as a mobile-first web app prototype.

## Product definition

Opportunity Compass is a beginner-friendly platform that helps people find, understand, judge, and act on small AI-related money opportunities.

It is not a normal job board.
It is an opportunity translator and bullshit filter.

Core promise:

> Find small AI gigs worth touching. Avoid the bullshit.

## Required screens

1. Landing page
2. Intake form
3. Opportunity feed
4. Opportunity detail page
5. Salvage Picks page
6. Daily Top 5 page
7. Saved opportunities page
8. Admin import page
9. Admin review page
10. Pricing page

## Required data

Use fake/sample data only.

Do not include real private data, API keys, emails, addresses, payment details, scraped private content, or copied paid-platform content.

## Required features for v0.1

- Display sample opportunity cards
- Filter by verdict
- Filter by category
- View opportunity details
- Save/unsave opportunities locally or with simple mock state
- Show Salvage Picks
- Show Daily Top 5
- Admin import form for raw pasted text
- Admin review page with draft card fields
- Pricing mockup

## Opportunity card fields

- title
- source
- category
- beginner fit
- verdict
- estimated pay range
- estimated time
- tools needed
- skills needed
- hidden buyer pain
- what this really means
- why beginners miss it
- smallest paid offer
- suggested first message
- questions to ask
- deliverable checklist
- red flags
- green flags
- original link placeholder
- saved status
- salvage pick candidate

## Design direction

Plain, practical, blunt, mobile-first.

Avoid:

- fake guru styling
- neon crypto look
- overpromising money
- cluttered dashboards
- corporate buzzword overload

Prefer:

- clear cards
- strong verdict labels
- simple navigation
- readable spacing
- direct copy
- trust-building warnings

## Suggested tech stack

Any simple modern web stack is acceptable.

Good default:

- React or Next.js
- TypeScript if available
- simple JSON seed data for v0.1
- Tailwind or basic CSS
- no paid API required for first prototype

## Stop conditions

Do not stop for minor design uncertainty.
Do not add paid API requirements.
Do not add scraping.
Do not add auto-apply or auto-message behavior.
Do stop if a step requires real secrets, private user data, or paid account credentials.

## First builder mission

Build the static/data-driven prototype first. Use sample data. Make the card format and screen flow work before adding real integrations.
