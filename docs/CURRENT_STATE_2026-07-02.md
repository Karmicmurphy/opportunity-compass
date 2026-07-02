# Current State - 2026-07-02

## Plain status

Opportunity Compass has enough research and structure to build a v0.1 prototype.

Do not keep researching in circles before building.

## Locked architecture

Opportunity Compass is the public-facing product lane.

It translates small AI-enabled work, freelance tasks, side gigs, hidden niche work, and task-platform opportunities into plain-English cards.

FlashRiver / CERT-RIVER / PRISM-RIVER is a separate modular trust/proof/salvage engine family.

FlashRiver can later plug into Opportunity Compass to generate or verify free-first work modules, but it is not required for v0.1.

Twis Holo Workshop is private and should stay out of the public Opportunity Compass product.

## Correct relationship

Opportunity Compass finds and explains the work.

FlashRiver can later assemble the free-first workbench.

CERT-RIVER / PRISM-RIVER handle proof, policy, boundaries, and trust inside that engine family.

Twis Holo Workshop is Randy's private workspace and should not be exposed or absorbed.

## What was checked

Notion did not contain a clean source-of-truth page for the project names.

Google Drive did not contain clean master docs named FlashRiver, CERT-RIVER, Artifact Compass, or Opportunity Compass, but it did show related free-tool research patterns.

The uploaded CERT_RIVER_PHASE755_FULL_REPAIR_AND_DEBUG_CLOSE.zip was inspected read-only. It reported PASS and contained the close package evidence for local workspace metadata, artifact integrity, receipt consistency, JSON parse health, ZIP integrity, and phase continuity.

Important boundary: that close package does not broaden into claims that all tools, cloud systems, providers, or future modules are secure or certified.

## Repo state

The Opportunity Compass repo now contains product specs, research passes, Salvage Picks, sample opportunities, source map, database schema, FlashRiver integration notes, and FlashRiver invention scope.

Recent important files added:

- docs/flashriver-integration-note.md
- docs/flashriver-invention-scope.md
- docs/research-pass-04-trust-risk-dive.md
- docs/research-pass-05-builder-readiness-dive.md
- docs/research-pass-06-competitor-pricing-dive.md
- docs/research-pass-07-data-model-handoff-dive.md

## Build rule going forward

Do not build Opportunity Compass like CERT-RIVER.

CERT-RIVER needed deep proof-chain discipline because it is a trust engine.

Opportunity Compass should be built as a fast product shell first.

Version 1 should be small, clickable, mobile-first, and static-data driven.

Do not wire live FlashRiver into v0.1.

Prepare fields for future FlashRiver modules, but keep the engine separate.

## v0.1 allowed scope

Allowed:

- landing page
- intake form
- opportunity feed
- card detail page
- Salvage Picks page
- Daily Top 5 page
- saved cards with local state
- pricing mockup
- admin import mock page
- admin review mock page
- static JSON seed data
- FlashRiver-ready workbench fields

Banned from v0.1:

- scraping
- auto-apply
- auto-message
- real payment processing
- real user accounts unless absolutely required
- real FlashRiver engine integration
- Twis Holo Workshop references
- private Google Drive or Gmail imports
- broad certification claims
- fake income promises

## Future FlashRiver-ready fields

Opportunity cards should prepare for later workbench modules with fields like:

- free_tool_stack
- local_tool_option
- cloud_tool_option
- paid_upgrade_options
- privacy_boundary
- license_note
- security_note
- module_name
- work_module_available
- setup_steps
- export_format
- human_review_step

## Correct next move

Create seed data and builder control materials.

Recommended next files:

- data/opportunities.json
- data/salvage-picks.json
- data/categories.json
- data/risk-labels.json
- data/daily-top-five.json
- AGENTS.md
- docs/codex-task-packet.md
- docs/zai-marathon-mission-packet.md
- docs/prototype-build-prompt.md

## Tool strategy

Use Codex for sharp repo-contained work.

Use Z.ai / GLM marathon mode for broader long-running build missions.

Do not babysit either tool with tiny repeated prompts.

Use mission packets, build fences, stop conditions, and sub-agent review roles.

## Packaging rule for AI builders

Every AI build mission should require a clean final project folder.

The final output should be one root folder with source, data, README, run instructions, and a short build report.

Prefer ZIP export. If the tool only produces TAR, the TAR must contain one clean root project folder.

## Next conversation starting point

Start by creating the seed data and builder control packets.

Do not reopen broad research unless a specific gap appears.
