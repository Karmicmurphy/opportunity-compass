# Research Pass 04 - Trust and Risk Dive

Date: 2026-07-02

## Purpose

This pass turns warning signs into product logic for Opportunity Compass.

The app should not only show opportunities. It should help users decide whether an opportunity is worth touching, watching, trashing, avoiding, or treating as too advanced.

## Core finding

Trust and risk must be part of every opportunity card.

The user should never have to open a listing and guess whether it is safe, realistic, too advanced, or just vague noise.

## Verdict model

### Touch

Use when the opportunity has:

- clear task
- clear deliverable
- reasonable scope
- beginner-safe tools
- no account access required
- no money required from worker
- no sensitive data handling
- no advanced credentials needed

### Watch

Use when the opportunity may be useful but needs clarification.

Common causes:

- vague deliverable
- unclear pay
- unclear task count
- unclear acceptance rules
- mixed beginner and advanced skills
- platform reputation is mixed
- qualification test exists but scope is unclear

### Trash

Use when the opportunity is not worth time even if it is not clearly unsafe.

Common causes:

- overcrowded low-value work
- unrealistic expectations
- too much work for too little pay
- no clear buyer pain
- pure hype
- no defined deliverable
- repeated generic AI language with no real task

### Scam Risk

Use when warning signs appear.

Common causes:

- upfront payment required
- money movement requested
- strange payment method
- personal or financial information requested too early
- high pay for vague easy work
- pressure to act fast
- off-platform messaging pressure
- fake recruiter feel
- unclear company identity
- task platform asks the worker to pay to continue
- work requires unnecessary account access

### Too Advanced

Use when the opportunity is real but not beginner-safe.

Common causes:

- legal, medical, financial, insurance, security, or regulated expertise
- advanced coding or production engineering
- expert domain review
- enterprise automation
- data privacy or compliance risk
- high-liability deliverables

## Score fields

Each card should eventually include these internal scoring fields:

- task_clarity_score: 1-5
- deliverable_clarity_score: 1-5
- beginner_fit_score: 1-5
- pay_scope_fit_score: 1-5
- trust_score: 1-5
- risk_score: 1-5
- account_access_required: yes/no
- sensitive_data_risk: none/low/medium/high
- expertise_required: none/basic/intermediate/expert
- recommended_verdict

## Red flag checklist

Flag the card when any of these appear:

- worker must pay before earning
- unclear company or buyer identity
- off-platform pressure
- unrealistic pay for easy vague tasks
- private financial details requested early
- account login requested
- free large test task
- unclear acceptance rules
- vague remote-work language
- rushed hiring pressure
- buyer will not define scope
- platform has many complaints about payment or access

## Green flag checklist

Increase confidence when these appear:

- task is clearly described
- deliverable is countable
- buyer provides examples
- payment method is normal for the platform
- no login access needed
- no sensitive data needed
- scope is fixed
- owner reviews final work
- acceptance rules are written down
- paid trial is small and clear

## Opportunity Compass user-facing warning labels

### Needs Clarification

Use when the job may be real but the scope is too vague.

### Scope Creep Risk

Use when the buyer asks for a small thing but hints at unlimited revisions, undefined batches, or ongoing unpaid support.

### Pay/Scope Mismatch

Use when the work may be real but the offered pay is too low for the task size.

### Access Risk

Use when the job asks for login access, admin access, or unnecessary private files.

### Sensitive Data Risk

Use when the work involves customer lists, private records, health information, financial documents, or other sensitive data.

### Expert Work Risk

Use when the listing requires professional judgment but is marketed like beginner work.

### Platform Risk

Use when the platform or buyer model is known for inconsistent task supply, opaque review, or unclear acceptance rules.

## Product rule

Every opportunity card should answer:

- What could go wrong?
- What should the user ask before touching it?
- What boundary protects the user?
- What verdict fits the evidence?

## App behavior for v0.1

Do not build automatic scam detection first.

Start with manual admin labels:

- verdict
- red flags
- green flags
- risk labels
- boundary note

Later, scoring can become semi-automated.

## Next pass

Pass 5 should turn the research into build-ready product structure: card schema, filters, admin workflow, and prototype requirements.
