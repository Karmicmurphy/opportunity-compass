# Database Schema Draft

This is a first-pass schema for Opportunity Compass v0.1.

Use this as a planning document, not final production code.

## users

Stores basic user account data if authentication is added later.

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
- original_link_placeholder
- is_salvage_pick
- status: draft / approved / rejected / archived
- created_at
- updated_at

## categories

Stores opportunity categories.

Fields:

- id
- name
- description
- created_at
- updated_at

Starter categories:

- AI writing and editing
- Review replies
- Prompt work
- AI image prompts
- AI music prompts
- Spreadsheet cleanup
- PDF/data cleanup
- Simple automation
- Local business AI help
- Marketplace listing cleanup
- Resume/profile help
- Simple web/app prototype

## saved_opportunities

Stores user-saved opportunities.

Fields:

- id
- user_id
- opportunity_id
- notes
- created_at

## admin_imports

Stores raw imported/pasted material before card approval.

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

## safety note

Do not store private user data, real secrets, API keys, personal addresses, payment information, or copied paid-platform content in public seed files.
