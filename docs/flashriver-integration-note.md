# FlashRiver Integration Note

Date: 2026-07-02

## Purpose

This note locks the architecture boundary between Opportunity Compass and the user's separate FlashRiver engine family.

## Correct separation

Twis Holo Workshop is private.

It is the user's personal workshop and should not be treated as part of the public Opportunity Compass product.

Opportunity Compass may call external modules, but it should not absorb or expose Twis Holo Workshop.

## FlashRiver engine family

FlashRiver / CERT-RIVER / PRISM-RIVER should be treated as one separate modular engine family.

Its role is not just to recommend tools.

Its role is to assemble free-first work modules from small verified tool fragments.

Plain-language function:

- send out small workers
- find the free or low-cost tool fragments needed for a task
- grab only what is needed
- check basic trust, security, license, privacy, and usability boundaries
- assemble those pieces into a small usable work module
- provide fallback paid options only when the free path is not enough

## How Opportunity Compass uses it

Opportunity Compass translates the opportunity.

FlashRiver builds or prepares the work module.

Example flow:

1. Opportunity Compass card says: PDF to Spreadsheet Cleanup.
2. User asks for a workbench.
3. FlashRiver searches for the smallest safe free-first tool path.
4. FlashRiver returns the module: tool list, steps, privacy boundary, export format, fallback options, and human review checklist.

## Public product boundary

The public product should say:

Opportunity Compass helps users understand small AI-enabled work and, when available, can generate a free-first work module through a separate verification engine.

The public product should not say:

- Twis Holo Workshop is part of the platform
- every tool is fully certified safe
- every workbench is legally guaranteed
- every task can be automated
- paid tools are required by default

## Commercial feature idea

Potential paid feature:

Build My Workbench

This feature generates a task-specific work module for an opportunity card.

Example modules:

- Review Reply Workbench
- FAQ Draft Workbench
- PDF Cleanup Workbench
- Canva Flyer Cleanup Workbench
- Social Post Batch Workbench
- Workflow Map Workbench
- Website Copy Cleanup Workbench

Each module should include:

- free-first tool path
- setup steps
- local/private option when needed
- cloud option when appropriate
- paid upgrade option only if justified
- boundary note
- deliverable checklist
- export format
- human review step

## Current recommendation

Do not build FlashRiver integration inside v0.1 yet.

For v0.1, represent the idea with static fields:

- free_tool_stack
- paid_upgrade_options
- privacy_boundary
- license_note
- work_module_available
- module_name

This lets Opportunity Compass prove the product experience before wiring a real engine call.

## Next build step

Create seed data with these fields so the prototype is ready for later FlashRiver integration without exposing the private workshop.
