---
name: launch-selecthub
description: |
  Claim and maintain an accurate SelectHub software product profile with five live category-product benchmarks,
  verified vendor ownership, buyer-facing feature and pricing evidence, and current claim-form capture. Use when
  listing or correcting a product on SelectHub.
---

<HUMAN-WRITING-RULES>
For every user-facing prose artifact produced by this skill, run the full embedded-mode process in `../../references/human-writing.md` before finalizing. Its no-fabrication rule and all 33 pattern checks are mandatory; preserve the intended platform voice and do not alter code, structured data, link targets, quotations, titles, or proper names.
</HUMAN-WRITING-RULES>

<EXTREMELY-IMPORTANT>
1. SELECTHUB IS A BUYER-RESEARCH AND SOFTWARE-SELECTION PLATFORM. It says products are analyst-reviewed and routes
   vendors through a claim/verification process. Do not promise a listing, category position, leaderboard, award,
   buyer leads, recommendation, sales outcome, or editorial control.
2. USE $browse AND EXACTLY FIVE LIVE, COMPARABLE PRODUCT PROFILES IN THE USER'S ACTUAL SELECTHUB CATEGORY. Capture
   category, buyer use case, summary, analyst/features/pricing/deployment evidence, alternatives, rating/review
   context, CTA, and last-updated/verification signals. Do not copy peer content or claim that SelectHub's analysis
   is vendor-authored.
3. CURRENT CLAIM FIELDS WERE OBSERVED ON 2026-07-23: Product Name; Company (required); First Name (required); Last
   Name (required); Title; Email (required); Phone Number for verification (required); Website (required); and submit.
   The page says SelectHub follows up to verify ownership and explain updating/listing. Re-capture before entry.
4. HUMAN APPROVAL REQUIRED. Do not submit the claim, disclose personal contact data, accept terms, buy vendor services,
   contact buyers, or edit a profile without explicit user approval.
</EXTREMELY-IMPORTANT>

# Launch on SelectHub

## Workflow

1. Return `CLAIM READY`, `PROFILE CORRECTION FIRST`, `CATEGORY/BENCHMARK NEEDED`, or `NOT READY`. Confirm the product
   is B2B software, company authority, canonical domain, buyer category, deployment/support/pricing sources, and a
   verification-contact owner.
2. Use `$browse` to benchmark exactly five current profiles in the chosen category. Create an evidence matrix; do not
   turn analyst coverage or peer outcomes into promises.
3. Build `.ulpi/launch/selecthub/` with `OWNERSHIP-AND-ROUTE.md`, `BENCHMARK.md`, `PRODUCT-EVIDENCE-PACKET.md`,
   `CLAIM-FORM-MAP.md`, `BUYER-FACTS.md`, `CHANGE-GOVERNANCE.md`, `analytics.md`, and positioning. Include verified
   product name/domain, category, buyer/problem/outcome, feature evidence, integrations, deployment, security,
   implementation/support, pricing availability, alternatives, media, and source URLs.
4. After authorization, capture the live fields and follow-up verification request. Map every fact to a source; make
   no unverifiable ranking, integration, customer, pricing, or security claim. Present the submission preview for
   approval.
5. After authorized claim/update, verify the public profile, product name, category, link, summary, facts, and change
   status. Correct material errors through the owner route, log each change, and measure qualified referral/context
   only. End `LIVE — SELECTHUB PROFILE RUNBOOK ACTIVE`.
