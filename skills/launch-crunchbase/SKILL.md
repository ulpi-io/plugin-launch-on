---
name: launch-crunchbase
description: |
  Create, claim, and maintain a source-governed Crunchbase company profile with five live organization benchmarks,
  verified company, people, funding, and news data, and account-gated form capture. Use when managing a Crunchbase
  company record.
---

<HUMAN-WRITING-RULES>
For every user-facing prose artifact produced by this skill, run the full embedded-mode process in `../../references/human-writing.md` before finalizing. Its no-fabrication rule and all 33 pattern checks are mandatory; preserve the intended platform voice and do not alter code, structured data, link targets, quotations, titles, or proper names.
</HUMAN-WRITING-RULES>

<EXTREMELY-IMPORTANT>
1. CRUNCHBASE IS A PRIVATE-MARKET INTELLIGENCE DATABASE, NOT A MARKETING PROFILE. Its data can cover organizations,
   people, funding rounds, investors, acquisitions, revenue/growth insights, news, and predictions. Never fabricate,
   round up, backdate, omit material qualifiers, or disclose confidential facts. Do not promise search rank, investor
   interest, predictive outcome, press, leads, fundraising, valuation, or business outcome.
2. USE $browse AND EXACTLY FIVE LIVE, COMPARABLE ORGANIZATION PAGES. On 2026-07-23 the current public surface showed
   Vultr, Anysphere (Cursor), Baseten, Mistral AI, and Replit as starting examples. Re-capture before use. Compare
   organization identity, location, website, categories, description, people, funding/news evidence, source links,
   completeness, and claim/update controls. Do not copy profile prose, data, investor facts, financial figures, or
   predictions.
3. CURRENT PUBLIC ROUTES INCLUDE `Create Profile` at `/add-new`, organization pages at `/organization/<slug>`, and
   account login. Create/edit controls and required fields are account-gated; capture every live entity type, field,
   source/verification, moderation, publication, and correction control after explicit authorization. Never guess.
4. HUMAN APPROVAL REQUIRED. Do not create/login to an account, create/claim/update a profile, submit funding/people
   data, attach sources, upload a logo, accept terms, or contact Crunchbase without explicit approval.
</EXTREMELY-IMPORTANT>

# Launch on Crunchbase

1. Return `COMPANY RECORD READY`, `CLAIM/CORRECTION FIRST`, `SOURCE EVIDENCE NEEDED`, or `NOT READY`. Confirm the
   legal/canonical company identity, control of website/email, public disclosure authority, factual location/categories,
   and a data steward.
2. Benchmark exactly five comparable current organization pages using `$browse`. Create `.ulpi/launch/crunchbase/`
   with `BENCHMARK.md`, `ENTITY-SOURCE-REGISTER.md`, `COMPANY-PACKET.md`, `PEOPLE-AND-FUNDING-REGISTER.md`,
   `FORM-CAPTURE.md`, `CHANGE-GOVERNANCE.md`, `CORRECTION-RUNBOOK.md`, `analytics.md`, and positioning.
3. Prepare sources for canonical name/domain, logo, overview, founded date, HQ/location, categories, employee count
   only if public/verified, leadership, products, funding/rounds/investors, acquisitions, news, and social links. Mark
   each fact public, confidential, unknown, disputed, or source-verified; do not submit unknowns.
4. After authorization, capture live add/claim fields and map every submitted fact to an authoritative source. Review
   sensitive founder, employee, financial, and investor data for consent/disclosure before submission. Verify
   publication/correction process and retain the exact submitted data.
5. After authorized publication/update, verify the public organization page, name, URL, location, categories, people,
   links, and sourced facts. Correct material errors through the proper route, maintain an evidence log, and measure
   only factual referral/context. End `LIVE — CRUNCHBASE COMPANY-DATA RUNBOOK ACTIVE`.
