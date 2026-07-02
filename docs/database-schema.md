# Database Schema Draft

This is a v0.1 planning schema for Opportunity Compass.

Use this as a planning document, not final production code.

## Build principle

For v0.1, use static JSON or a simple database. The schema exists so the product stays clear when moving from documents to prototype.

## users

Optional for v0.1. Add later if authentication is needed.

Fields:

- id
- email
- display_name
- plan: free / paid
- created_at
- updated_at

## intake_profiles

Stores user preferences and beginner-fit matching data.

Fields:

- id
- user_id
- skill_level: beginner / intermediate / advanced
- available_time: 15_minutes / 30_minutes / 1_hour / 2_plus_hours
- income_goal: 10_today / 25_today / 50_this_week / recurring
- skills: array or related table
- preferred_categories: array
- avoid_categories: array
- created_at
- updated_at

## opportunities

Stores approved opportunity cards.

Fields:

- id
- title
- source
- source_type
- category_id
- beginner_fit: high / medium / low
- verdict: touch / watch / trash / scam_risk / too_advanced
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
- risk_labels: array
- boundary_note
- where_to_find_buyers
- what_not_to_promise
- original_link_placeholder
- is_salvage_pick
- is_package
- package_name
- status: draft / approved / rejected / archived
- created_at
- updated_at

## opportunity_scores

Stores scoring used to explain verdicts.

Fields:

- id
- opportunity_id
- task_clarity_score: 1-5
- deliverable_clarity_score: 1-5
- beginner_fit_score: 1-5
- pay_scope_fit_score: 1-5
- trust_score: 1-5
- risk_score: 1-5
- account_access_required: yes / no
- sensitive_data_risk: none / low / medium / high
- expertise_required: none / basic / intermediate / expert
- recommended_verdict
- created_at
- updated_at

## risk_labels

Stores reusable risk labels.

Fields:

- id
- name
- description
- severity: low / medium / high

Starter labels:

- Needs Clarification
- Scope Creep Risk
- Pay/Scope Mismatch
- Access Risk
- Sensitive Data Risk
- Expert Work Risk
- Platform Risk

## categories

Stores opportunity categories.

Fields:

- id
- name
- description
- created_at
- updated_at

Starter categories:

- AI content review
- AI response evaluation
- AI training and task work
- Local business AI help
- Review replies
- FAQ drafts
- Marketplace listing cleanup
- PDF and spreadsheet cleanup
- Canva cleanup
- Social post batching
- Workflow mapping
- Customer message templates
- Website copy cleanup
- AI video prompt/script prep
- Domain expert AI evaluation
- Trust and risk check

## saved_opportunities

Stores user-saved opportunities.

Fields:

- id
- user_id
- opportunity_id
- notes
- created_at

## admin_imports

Stores raw imported or pasted material before card approval.

Fields:

- id
- source_type
- source_name
- original_link_placeholder
- raw_text
- admin_notes
- generated_card_json
- review_status: new / reviewed / approved / rejected
- created_at
- updated_at

## daily_briefs

Stores Daily Top 5 collections.

Fields:

- id
- title
- brief_date
- summary
- created_at
- updated_at

## daily_brief_items

Stores the five opportunities in each brief.

Fields:

- id
- daily_brief_id
- opportunity_id
- rank
- reason_included
- suggested_next_move

## salvage_pick_packages

Optional table if Salvage Picks become separate packaged products instead of normal cards.

Fields:

- id
- opportunity_id
- package_name
- buyer_pain
- starter_price
- tools_needed
- deliverable_checklist
- boundary_note
- where_to_find_buyers
- what_not_to_promise

## safety note

Do not store private user data, real secrets, API keys, personal addresses, payment information, private screenshots, or copied paid-platform content in public seed files.
