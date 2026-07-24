---
name: launch-g2
description: |
  Prepare, submit, optimize, and operate a G2 product listing for a real B2B software product or service.
  Covers the eligibility gate, duplicate-profile search, category evidence, product-submission worksheet,
  live category and top-product benchmarking with the browse skill, conversion-focused profile copy and
  assets, packages and pricing, features, integrations, UTMs, authentic review campaigns, review responses,
  Grid and badge readiness, and ongoing measurement. Writes a durable launch package under .ulpi/launch/g2.
  Use when a startup wants to get listed on G2, claim or improve an existing G2 profile, collect compliant
  customer reviews, qualify for G2 reports, or turn G2 into a sustained buyer-trust channel.
---

<HUMAN-WRITING-RULES>
For every user-facing prose artifact produced by this skill, run the full embedded-mode process in `../../references/human-writing.md` before finalizing. Its no-fabrication rule and all 33 pattern checks are mandatory; preserve the intended platform voice and do not alter code, structured data, link targets, quotations, titles, or proper names.
</HUMAN-WRITING-RULES>

<EXTREMELY-IMPORTANT>
This skill prepares a G2 listing and growth program. Treat these rules as blocking:

1. PASS ELIGIBILITY FIRST. G2 does not list B2C-only products or products still in alpha or beta. Do not
   submit until the offer is a real, available B2B product or eligible service tied to a real vendor.
2. NEVER CREATE A DUPLICATE. Search G2 by product and vendor name before preparing a new submission. If a
   profile exists, claim or correct it.
3. CATEGORIES FOLLOW NATIVE FUNCTIONALITY. A product must meet every inclusion criterion for a requested
   category. Audience, aspirational use cases, competitors, and integrations are not proof of native features.
4. TELL THE TRUTH. Use the official product name, canonical URL, actual pricing, supported deployment model,
   real integrations, current screenshots, and verifiable evidence. Never invent features, customers, awards,
   rankings, or reviews.
5. REVIEWS MUST BE AUTHENTIC AND UNBIASED. Never review-gate, target only happy users, ghostwrite reviews,
   ask employees or direct competitors to review, suppress criticism, or condition an incentive on sentiment.
6. DO NOT PROMISE RANK. G2 scores are relative and algorithmic. Set controllable goals around completeness,
   category fit, review quality and recency, buyer engagement, referral traffic, and qualified pipeline.
7. VERIFY LIVE REQUIREMENTS. G2 changes forms, plan entitlements, report deadlines, and profile fields. Recheck
   official G2 documentation and the live form immediately before submission.
8. PERSIST THE WORK. Write the full package under .ulpi/launch/g2 so the user can review, submit, and maintain
   it without reconstructing decisions from chat.
9. BENCHMARK THE LIVE CATEGORY. Use the browse skill to inspect the current leading G2 profiles in the exact
   category and buyer segment before finalizing description copy. Never copy competitor language or claims.
</EXTREMELY-IMPORTANT>

# Launch on G2

## Goal

Produce a truthful, conversion-focused G2 launch package and an ongoing operating plan:

- SUBMISSION.md — eligibility verdict, existing-profile result, submission worksheet, and claim route
- CATEGORY-EVIDENCE.md — requested categories, every inclusion criterion, and proof for each
- BENCHMARK.md — dated live analysis of leading products, buyer expectations, and competitive whitespace
- PROFILE.md — paste-ready profile copy, pricing, feature, integration, media, and UTM specifications
- REVIEW-PLAN.md — compliant audience, invitations, cadence, moderation expectations, and response playbook
- OPERATIONS.md — 30/60/90-day plan, quarterly upkeep, metrics, targets, and owners
- CHECKLIST.md — blocking pre-submit, profile-quality, compliance, and launch-readiness gates
- analytics.md — UTM map, referral/conversion instrumentation, validation, and read-out plan
- positioning.md — shared grounded product brief at .ulpi/launch/positioning.md, created or reused

## Step 0: Ask which product or platform is being listed

If the user has not already identified it unambiguously, ask this before research:

Which product or platform are you listing on G2? Send its canonical product or pricing URL and any existing
G2 profile URL.

Do not guess from the current repository name, parent company, or prior conversation. Confirm whether the
listing is for a standalone product, platform, API, plugin, service, or suite.

Then determine which operating mode applies:

- New listing: no G2 product profile exists.
- Claim: a correct but unclaimed profile exists.
- Correct: a duplicate, wrong vendor, wrong product name, or inaccurate category/profile exists.
- Optimize: the profile is claimed but incomplete, weak, or stale.
- Grow: the profile is strong and needs a compliant review and category-performance program.

Gather the product name, vendor/legal entity, canonical URL, launch state, B2B use case, deployment model,
pricing, target segments, existing customers, current G2 URL if any, and the owner who can access my.G2.
Ask only for facts that cannot be verified from the site or repository.

## Step 1: Require the browse workflow for live research

Use the $browse skill for the product-site, G2 category, and competitor-profile research in this workflow.
Check its availability and run browse --version as directed by that skill.

If $browse is not installed, tell the user that live category benchmarking needs it and suggest:

Claude Code:

~~~text
/plugin marketplace add ulpi-io/marketplace
/plugin install browse@ulpi
~~~

Codex:

~~~bash
codex plugin marketplace add ulpi-io/marketplace
codex plugin add browse@ulpi
~~~

The browse plugin also requires its CLI:

~~~bash
npm install -g @ulpi/browse
browse --version
~~~

Do not install anything automatically. If normal `$browse` receives a 403, challenge, or anti-automation block,
load and follow `$browse-stealth`: verify Camoufox, stop the current server, retry in headed Camoufox, and wait
for the rendered page to stabilize. If stealth remains blocked by IP reputation, require the permitted
user-assisted handoff or residential proxy, mark `BENCHMARK.md` `BLOCKED — LIVE TOP-FIVE BROWSE REQUIRED`, and
keep description copy provisional. Never claim to have inspected current top G2 products without live evidence.

## Step 2: Ground the product

Reuse .ulpi/launch/positioning.md if it is current. Otherwise inspect the live site with the browse skill
when available, plus README, documentation, pricing, security, integrations, and product UI. Record:

- official product and vendor names
- one-sentence positioning and buyer problem
- ideal customer profile and company segment
- native capabilities and differentiators
- deployment, languages, regions, pricing, and trial status
- evidence URLs and current screenshots
- real competitors and alternatives

Save the brief to .ulpi/launch/positioning.md. Never infer eligibility or category fit from marketing copy
alone.

## Step 3: Run the eligibility and duplicate gate

Load references/eligibility-and-categories.md. Search G2 for the product name, vendor, prior names, and common
spelling variants. Then issue one verdict:

- ELIGIBLE — proceed.
- ELIGIBLE, CLAIM EXISTING — do not submit a new product.
- ELIGIBLE WITH CATEGORY EVIDENCE REQUIRED — proceed only after Step 4 passes.
- NOT READY — product is alpha/beta or lacks a public, purchasable B2B offer.
- INELIGIBLE — B2C-only or otherwise outside G2's listing methodology.
- NEEDS G2 RESEARCH DECISION — ambiguous product, API, extension, plugin, or mixed software/service offer.

Write the evidence and verdict to SUBMISSION.md. Stop the submission workflow on NOT READY or INELIGIBLE,
but leave a concrete remediation path.

## Step 4: Prove category fit

For every proposed category:

1. Open the current G2 category page.
2. Read the full category definition and all inclusion criteria.
3. Map every criterion to a native product capability.
4. Link proof: product page, documentation, current screenshot, recorded demo, or release note.
5. Mark any unsupported criterion as FAIL; do not stretch positioning to hide it.
6. Select the strongest existing category as the proposed main category.

Write CATEGORY-EVIDENCE.md using references/eligibility-and-categories.md. Request only child categories that
the product fully satisfies. Treat integration-provided functionality as integration evidence, not native
functionality. If no defined category fits, document the closest Other category or a research request.

## Step 5: Benchmark leading products in the live category

After category fit is proven, use $browse to inspect the live main-category page and leading product profiles.
Write BENCHMARK.md:

1. Record the category URL, segment filter, sort order, date, and whether any result is sponsored.
2. Inspect the first five to eight organic products under the default G2 Score view, plus a relevant
   high-satisfaction challenger when useful.
3. Capture each product's overview structure, buyer, problem, outcomes, proof, differentiators, CTA, pricing
   transparency, media strategy, and recurring review themes.
4. Separate category table stakes from genuinely differentiated positioning.
5. Identify overused claims, missing buyer questions, underserved segments, and credible whitespace.
6. Link every observed profile and quote no competitor copy beyond a few necessary words.

Do not choose a description by imitating the category leader. Use the benchmark to understand buyer
expectations, then ground every claim in the user's real product and positioning.md.

## Step 6: Build the submission and claim package

Complete the worksheet in SUBMISSION.md using the live Product Submission Form as the final source of truth.
Populate every field with a final paste-ready value in the same order as the live form:

- Product or pricing page URL
- official Product Name with no marketing suffix
- Vendor Domain and Vendor Name
- LinkedIn Company Page URL
- Description of Product
- submission logo, with SVG preferred by the current live form
- current product screenshots, each with a Title and Description
- whether the submitter works at the company that develops the product
- whether the submitter wants to serve as profile admin
- up to three eligible customer reviewer contacts, only when privacy/compliance checks pass
- launch state and proof the product is generally available
- requested categories with links to CATEGORY-EVIDENCE.md
- pricing/trial model, deployment, languages, and target business users
- submitter identity and company relationship
- supporting demo, documentation, and screenshots

Discover public facts with $browse and the product site. Then ask one grouped follow-up containing only the
private or genuinely unknowable fields, such as company relationship, admin preference, and optional reviewer
contacts. Do not ask the user to retype public data.

SUBMISSION.md must:

- use the exact live field labels as headings
- put the final value immediately below each heading in a clearly marked READY TO PASTE block
- include word/character counts when the live field has a hard limit
- provide local asset paths and source URLs for logo and every screenshot
- give every screenshot a final Title and Description
- mark missing required information BLOCKED with one precise question
- contain no generic placeholders when the ready verdict is issued
- finish with a short, ordered click-through checklist matching the form

If an eligible profile exists, record the claim URL and owner. G2 says claim approval typically takes one to
three business days. Do not create accounts, accept terms, or make the final external submission unless the
user explicitly asks and reviews the prepared data. Do not write raw customer email addresses into repository
artifacts; have the user enter them directly into G2 or use an approved secure system.

Track approval as separate states: submitted, conditionally approved, profile approved, publicly visible,
categories assigned, direct profile URL received, and claimed/admin access confirmed. A profile approval
message is not evidence that category assignment is complete.

## Step 7: Build a stellar buyer-facing profile

Load references/profile-playbook.md. Use launch-copy when available to create profile copy from positioning.md,
BENCHMARK.md, and the current category contract. Draft three distinct descriptions:

- category-led: immediately establishes category fit and buyer
- outcome-led: leads with the costly problem and measurable or verifiable outcome
- differentiation-led: leads with the strongest defensible contrast against category sameness

Show word counts, score each against truth, clarity, category relevance, differentiation, proof, and CTA
strength, then recommend one. Write both the concise submission Description of Product and the fuller G2
profile overview. Never exceed a live hard limit; the current profile overview limit is 500 words.

Then apply the rest of the G2 profile contract. PROFILE.md must contain:

- three buyer-first description options, their scorecard, and one recommended final version
- category-specific problem, outcomes, native capabilities, differentiators, and proof
- profile logo, Grid logo, banner, video, screenshot, and download asset specifications
- packages, prices, billing units, trial details, CTAs, and package-level features
- languages, deployment model, product features, integrations, AI disclosures, and values/ethics fields
- canonical product and company URLs with a consistent G2 UTM scheme
- a field owner and last-verified date for every mutable section

Design the profile as a conversion page for an in-market software buyer, not as a backlink placeholder.
Separate verified free-profile capabilities from subscription-gated features; never tell the user a paid
feature is available without checking their current plan.

## Step 8: Build the compliant review engine

Load references/reviews-and-compliance.md and write REVIEW-PLAN.md:

- invite a broad, representative set of real users; never select only promoters
- exclude vendor employees and employees of direct competitors
- use neutral invitations asking for honest feedback, not a rating
- explain identity and moderation requirements without coaching answers
- use G2-managed or properly disclosed incentives only; never tie rewards to positivity
- plan an initial cohort and an always-on cadence that maintains recency
- include small-business, mid-market, enterprise, role, use-case, and geography mixes that reflect reality
- respond publicly to positive and negative reviews with substance
- route valid product feedback into the roadmap and report only genuine guideline violations

Use the user's actual customer base. If there are not enough eligible users, state that plainly and create a
customer-success plan rather than fabricating a campaign.

## Step 9: Plan for profile and category success

Load references/success-operations.md. Write OPERATIONS.md with:

- day 0–30: approval/claim, full profile, accurate category placement, first unbiased review cohort
- day 31–60: close content gaps, respond to every review, measure G2 referral and conversion behavior
- day 61–90: establish a recurring review cadence, refresh weak assets, and prepare for report deadlines
- quarterly: verify fields, pricing, evidence, categories, competitors, assets, reviews, and report dates

Set staged goals. Ten category-attributed reviews is an important report and feature-data threshold, but only
approved reviews relevant to that category count. Twenty reviews with a 4.0+ average can earn Users Love Us
under G2's current rules; treat it as an earned outcome, never a manipulated target.

Track profile completion, claim/approval status, category acceptance, approved/rejected/pending reviews,
review recency and segment mix, response time, profile views, referral sessions, assisted conversions,
qualified leads, and influenced pipeline. Use launch-analytics with channel g2 and utm_source g2 when
available; otherwise write the same minimal plan directly to .ulpi/launch/g2/analytics.md.

## Step 10: Run the blocking gate

Load references/artifact-templates.md and complete CHECKLIST.md. Do not mark the G2 launch ready unless:

- eligibility passed and no duplicate submission is being created
- every requested category criterion has evidence
- the live category benchmark is complete or explicitly marked BLOCKED
- the recommended description is grounded in product truth and competitive whitespace
- product and vendor identity match public truth
- profile copy, assets, pricing, deployment, features, integrations, and URLs are current
- review invitations are neutral, representative, and policy-compliant
- incentive handling and badge/report claims comply with current G2 rules and plan entitlements
- ownership, response SLA, metrics, and quarterly maintenance are assigned
- the user has reviewed any data that will be submitted externally

## Guardrails

- Never bypass G2 moderation, account controls, or plan restrictions.
- Never contact an anonymous reviewer to pressure or identify them.
- Never copy reviews from another site or submit on a customer's behalf.
- Never hide pricing that the user wants public; if pricing is custom, explain the buyer path clearly.
- Never claim Grid placement, rankings, awards, badges, star ratings, or category membership before verified.
- Never optimize for volume at the expense of review authenticity, detail, relevance, or recency.
- Never treat a high-authority G2 URL as proof of SEO value; measure actual discovery and conversion.
- Never leave a submission field as a template placeholder while reporting the package ready.

## When to load references

- references/eligibility-and-categories.md — listing eligibility, product identity, duplicate checks, and
  evidence-based category selection in Steps 3–6.
- references/profile-playbook.md — profile fields, asset specifications, pricing, features, integrations,
  live category benchmarking, buyer-facing copy, and conversion QA in Steps 5 and 7.
- references/reviews-and-compliance.md — reviewer eligibility, moderation, invitations, incentives, review
  gating prohibitions, responses, and campaign design in Step 8.
- references/success-operations.md — G2 scoring, report thresholds, badges, KPIs, and the 30/60/90 plus
  quarterly operating rhythm in Step 9.
- references/artifact-templates.md — required file structures and the blocking checklist in Step 10.

## Output contract

Write and return:

1. .ulpi/launch/positioning.md
2. .ulpi/launch/g2/SUBMISSION.md
3. .ulpi/launch/g2/CATEGORY-EVIDENCE.md
4. .ulpi/launch/g2/BENCHMARK.md
5. .ulpi/launch/g2/PROFILE.md
6. .ulpi/launch/g2/REVIEW-PLAN.md
7. .ulpi/launch/g2/OPERATIONS.md
8. .ulpi/launch/g2/CHECKLIST.md
9. .ulpi/launch/g2/analytics.md
10. an eligibility verdict, ready/not-ready verdict, unresolved G2 decisions, and exact next action
