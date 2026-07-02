# FlashRiver / CERT-RIVER Invention Scope

Date: 2026-07-02

## Status

This document captures the current understanding of FlashRiver / CERT-RIVER as a separate modular engine that can later be called by Opportunity Compass.

Twis Holo Workshop is private and is not part of the public Opportunity Compass product.

## Core invention

FlashRiver is a trust engine for digital work.

It is not a chatbot, not only a file checker, not only an audit report, and not only a prompt system.

It answers one question:

Can this claim, file, artifact, handoff, output, or decision actually be trusted, and exactly why?

## Core law

Assertion is not evidence.
Evidence is not proof.
Proof is not a certificate.
A certificate is not a receipt.
A receipt is not automatically current authority.

No certificate should claim more than the proof actually proved.

## Main parts

### FlashRiver

The whole system. The river everything flows through:

- files
- prompts
- handoffs
- receipts
- proof runs
- certificates
- artifacts
- recovered context
- restart packets
- audit trails

### CERT-RIVER

The proof and certification engine.

It decides:

- what was claimed
- what was tested
- what passed
- what failed
- what evidence exists
- what certificate can honestly be issued
- what must be quarantined
- what must not be trusted

### PRISM-RIVER

The policy layer.

It decides:

- what counts as safe
- what counts as out of scope
- what must be blocked
- what must be labeled
- what cannot be certified
- what human approval is required

CERT-RIVER proves. PRISM-RIVER governs.

### RiverKernel

The runner.

It executes bounded tasks:

- read file
- hash file
- run fixture
- compare output
- generate receipt
- record result

It should stay boring, small, and hard to lie to.

### Artifact Compass

The salvage and discovery layer.

It scans messy piles and separates:

- current authority
- stale material
- useful context
- missing evidence
- corrupted material
- dangerous-to-trust material
- archive candidates
- quarantine candidates

### Handoff System

The restart layer.

A proper handoff folder should include:

- README_START_HERE.md
- CURRENT_STATUS.md
- NEXT_PROMPT.md
- PROJECT_STATE.md
- RESTART_PACKET.md
- CERTIFICATE_LEDGER.md
- KNOWN_SCOPE_LIMITS.md
- receipts
- current authority links
- what not to trust

## What the invention does

### 1. Validates artifacts

Checks whether a file, ZIP, project folder, or handoff package is intact.

Examples:

- file exists
- file is non-empty
- ZIP opens
- JSON parses
- hash matches
- receipt matches
- manifest matches
- required files exist
- archive structure is sane

### 2. Separates evidence from claims

A system output is not automatically proof.
A passing script is not automatically certification.
A certificate is not automatically valid if the evidence changed.

### 3. Prevents stale authority

Old files can look official while no longer being current.

FlashRiver marks:

- current authority
- historical evidence
- stale handoff
- stale receipt
- superseded certificate
- quarantined artifact

### 4. Certifies narrow claims

FlashRiver does not certify vague broad claims like: this system is secure.

It certifies bounded claims like: for this local fixture, this archive path traversal case was denied and recorded.

### 5. Creates restartable project memory

Instead of depending on a giant chat thread, it creates restart packets that a future human, model, or machine can continue from.

### 6. Produces human-readable reports

The output should be usable by a human.

Example verdict:

VERDICT: QUARANTINE

Reason: The package contains useful context, but the receipt does not match the current ZIP.

Safe action: Do not continue from this as authority. Repair the receipt or restore the expected artifact.

## Current uploaded close package

Uploaded package reviewed in this conversation:

CERT_RIVER_PHASE755_FULL_REPAIR_AND_DEBUG_CLOSE.zip

Observed package SHA-256:

f85e92da8f5f225b670d76074e62712bcae32588dc14ff7a182054c071721f1c

Package structure:

- FULL_DEBUG_REPORT.md
- FULL_DEBUG_SUMMARY.json
- PHASE294_STALE_EXTERNAL_RECEIPT_BEFORE_PHASE755_FIX.json
- phase_file_inventory.csv
- receipt_artifact_consistency.csv
- top_level_json_parse.csv
- zip_integrity.csv

Reported result:

PASS

Reported debug counts:

- Top-level ZIPs tested: 512
- ZIP integrity failures: 0
- Top-level JSON files parsed: 120
- Top-level JSON parse failures: 0
- Phase directories scanned: 461
- Phase files scanned: 2219
- Empty phase files: 0
- Phase JSON parse failures: 0
- Receipt files checked: 118
- Receipt artifact failures: 0
- Receipt files with no recognized artifact key: 63
- Phase continuity gaps: 0

Important boundary:

This close package supports local workspace metadata and artifact integrity only. It does not broaden any proof, certificate, provider, cloud, live-system, or production claim.

## Productization path

The first standalone product should be:

CERT-RIVER Local Handoff Validator

Input:

- handoff folder
- ZIP
- bundle
- project archive
- proof packet

Output:

- PASS / FAIL / QUARANTINE
- what is current authority
- what is stale
- what is broken
- what can be repaired
- what must not be trusted
- next safe prompt/action

## Bigger product family

Potential tools:

1. Local Handoff Validator
2. Certificate Builder
3. Artifact Compass Salvage Tool
4. Project Restart Builder
5. Proof Ledger
6. AI Workflow Guard
7. Developer/Repo Audit Layer
8. Human-readable Audit Reports

## Opportunity Compass integration

Opportunity Compass should not absorb FlashRiver.

Opportunity Compass can call FlashRiver later as a separate modular engine.

Best later use:

- user finds an opportunity card
- user asks for a work module
- FlashRiver assembles a free-first tool path
- FlashRiver checks trust, boundary, privacy, license, and proof notes
- Opportunity Compass displays the resulting workbench to the user

For v0.1, do not wire a real engine call.

Use static fields first:

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

## What the invention is not

It is not:

- a generic chatbot
- a magic security guarantee
- a cloud security platform yet
- a replacement for legal compliance
- a finished app yet
- a claim that all tools are secure
- a claim that all AI outputs are true

It is a system for bounded trust decisions.

## Clean invention claim

FlashRiver is a local-first trust and certification framework for AI-assisted work. It validates digital artifacts, separates claims from evidence, binds proof runs to receipts, prevents stale context from becoming authority, quarantines unsupported material, and produces restartable handoff packages with human-readable trust verdicts.

## Practical invention claim

A tool that tells you whether a project handoff, AI output, archive, or proof packet can be trusted, and exactly what evidence supports that trust.

## Technical invention claim

A bounded certification pipeline that combines artifact hashing, manifest validation, receipt reconciliation, fixture-based proof execution, certificate scope control, authority-state tracking, quarantine handling, replay verification, and restart-packet generation into a deterministic local-first validation system.

## Emotional claim

FlashRiver is a way to stop important work from disappearing into chaos. It turns wreckage into evidence, evidence into structure, and structure into something another person or future self can continue.
