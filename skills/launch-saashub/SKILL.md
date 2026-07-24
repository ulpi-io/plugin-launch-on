---
name: launch-saashub
description: |
  Submit, verify, optimize, and operate a SaaSHub product listing. Covers eligibility, duplicate prevention,
  mandatory live five-peer category research, exact submission-field capture, categories, competitors, pricing,
  screenshots, product verification, reviews/comments, comparisons, analytics, and ongoing accuracy. Use when a
  released software vendor wants persistent SaaSHub discovery and competitor-intent visibility.
---

<HUMAN-WRITING-RULES>
For every user-facing prose artifact produced by this skill, run the full embedded-mode process in `../../references/human-writing.md` before finalizing. Its no-fabrication rule and all 33 pattern checks are mandatory; preserve the intended platform voice and do not alter code, structured data, link targets, quotations, titles, or proper names.
</HUMAN-WRITING-RULES>

<EXTREMELY-IMPORTANT>
Treat these rules as blocking:

1. SUBMIT ONLY AN ELIGIBLE, RELEASED PRODUCT. SaaSHub’s current submission guidance rejects software-development
   agencies, waitlist-only landing pages, unreleased products, free-subdomain products, and products not in English.
   Confirm a real, accessible product website on its own domain before submission.
2. SEARCH BEFORE SUBMITTING. Use `$browse` to find exact/variant names, former names, vendor names, domain, existing
   product, category, alternatives, and comparison pages. Verify/correct an existing profile instead of adding a
   duplicate.
3. BROWSE EXACTLY FIVE LIVE COMPARABLES. Before category, competitor, pricing, feature, or copy decisions, inspect
   the relevant SaaSHub category and exactly five comparable live listings, their official sites, and a relevant
   alternatives or comparison page. Search snippets do not satisfy this gate.
4. USE `$browse-stealth` WHEN BLOCKED. Normal browse comes first. On a block, retry headed Camoufox using
   `browse-stealth`. If an IP block remains, document it and require the permitted handoff/proxy; write
   `BLOCKED — LIVE TOP-FIVE BROWSE REQUIRED`, not invented observations.
5. LIST REAL CATEGORIES AND COMPETITORS. SaaSHub asks submitters to add relevant categories and listed competitors;
   it warns that submissions without listed competitors are slowed and put at the bottom of the queue. Competitors
   must solve the same primary job for a similar buyer—not merely be popular brands or targets for traffic capture.
6. VERIFY ONLY AS THE VENDOR. SaaSHub supports verification with a company-domain email, HTML snippet, or current
   support path. Never use a non-authoritative email, add an ownership snippet without consent, or store credentials.
7. NEVER MANIPULATE REVIEWS, COMMENTS, OR SIGNALS. Do not fabricate, buy, ghostwrite, gate, pressure, or condition
   reviews/comments, alternatives, votes, or comparisons. Never pose as a customer or independent community member.
8. KEEP EVERY CLAIM PROVABLE. Product description, pricing, feature/specs, screenshots, videos, platforms, release
   status, categories, integration/alternative claims, and badges need current first-party evidence. No invented
   pricing, roadmap, ratings, rankings, or competitor attacks.
9. HUMAN APPROVAL IS REQUIRED. Do not create an account, submit/verify/edit a product, add a snippet, post a
   comment/review, purchase a featured listing, invite customers, or contact SaaSHub without explicit user approval.
</EXTREMELY-IMPORTANT>

# Launch on SaaSHub

## Goal

Write `.ulpi/launch/saashub/` with `ELIGIBILITY-AND-ROUTE.md`, `SUBMISSION.md`, `BENCHMARK.md`,
`CONTENT-REQUIREMENTS.md`, `PROFILE.md`, `CATEGORIES-AND-COMPETITORS.md`, `VERIFICATION.md`,
`COMMUNITY-AND-OPERATIONS.md`, `CHECKLIST.md`, `analytics.md`, and shared `.ulpi/launch/positioning.md`.

## Step 0: Identify the product and listing state

Ask if unclear:

> Which released product are you listing on SaaSHub? Send its canonical URL, company/product name, target buyer and
> primary job, intended category, pricing URL, official domain email availability, and any existing SaaSHub URL.

Determine `NEW`, `VERIFY/CLAIM`, `CORRECT`, `OPTIMIZE`, or `NOT READY`. Gather owner authority, release/access proof,
English public site, canonical domain, buyer/job, pricing, platform, features, integrations, alternatives, logo,
screenshots/video, status page, support, legal proof, and customer-feedback owner.

## Step 1: Load references and research live

Read:

- `references/eligibility-submission-and-verification.md`
- `references/benchmark-profile-and-competitors.md`
- `references/community-operations-and-templates.md`

Use `$browse` to inspect the product site and the live SaaSHub submit, category, product, alternatives, comparison,
and verification pages. Record source URL, access date/timezone, exact visible fields/help text/limits, and evidence.
Recheck the live form immediately before an approved human submission.

## Step 2: Pass eligibility and duplicate gates

Record why the product is released, publicly reachable, English, and uses its own appropriate domain. Check each
disqualifier from the current submit page. Search duplicates and choose `CREATE`, `VERIFY/EDIT EXISTING`,
`CORRECT/MERGE`, or `NOT READY`. Do not treat “approval” as guaranteed.

## Step 3: Benchmark exactly five live peers

Open the intended category, record its definition, filters/order, and product count if shown. Choose exactly five
products that solve the same buyer job. Browse each listing and official site plus a relevant alternatives/comparison
page. Capture:

- URL, category tags, description, website/CTA, pricing type/amount/period where shown, platforms, release details
- screenshots/images/video, feature/specs, reviews/comments, questions, badges, and visible freshness/verification
- alternatives, verified alternatives, popular comparisons, related categories, and competitor framing
- profile completeness, factual specificity, visual patterns, buyer objections, and vendor-controlled vs generated
  content

Write `CONTENT-REQUIREMENTS.md` before copy. Mark each surface `REQUIRED/LIVE-FORM`, `CATEGORY BASELINE`,
`RECOMMENDED`, `SAASHUB/COMMUNITY-GENERATED`, `FEATURED/PAID`, `NOT AVAILABLE`, or `NOT APPLICABLE`; include
constraint, source, buyer question, and owner. Summarize peers—never reproduce their prose.

## Step 4: Build the submission and profile package

The current public Submit a Product page starts with Website URL and advises relevant categories, listed competitors,
and product verification; all submissions undergo approval. Capture every subsequent actual field in exact live order
and state `READY TO PASTE`, `SELECT`, `UPLOAD`, `NOT APPLICABLE`, `NEEDS OWNER`, or `BLOCKED`, with visible limits.

Prepare source-backed copy for identity, canonical website/CTA, concise and full description, categories, approved
competitors/alternatives, pricing model/plans/official pricing URL, supported platforms, release date where provable,
features/specs, screenshots/images/video, status/support, and real integration/compatibility proof. Draft three
angles—buyer job, workflow/capability, and proof/reassurance—then recommend the most concrete and distinctive one.

Public SaaSHub pages commonly surface Website, Pricing, Platforms, Release Date, Categories, screenshots/images,
Features & Specs, reviews, comments/discussion, alternatives, verified alternatives, popular comparisons, and
badges. These are content requirements to verify in the current UI, not a claim that every product/editor can set
every field. Never use AI-generated generic “features” as a vendor claim without first-party support.

## Step 5: Verify the product and operate responsibly

SaaSHub says product verification is free and helps vendors control/update listing details. Its documented routes are
the product page’s `Verify <product>` flow using a company email or HTML snippet, or a support-requested verification
link; after access, review the Verification tab and use the current verify action. It also says verified listings
receive a badge and quarterly prompts to reconfirm data. Make the exact current route a human handoff; no secret or
snippet is stored in artifacts.

Treat featured promotion separately from free listing/verification and verify scope, cost, placement, duration,
labels, and metrics before purchase. Request only neutral, honest user feedback under one universal eligibility rule;
do not solicit a star rating or positive comment. Answer public comments with vendor attribution, facts, source links,
and no PII or competitor attacks.

## Step 6: Measure, refresh, and validate

Track SaaSHub profile/category/comparison referrals, CTA-to-trial/demo/docs conversion, verified status, profile
freshness, review/comment volume and response SLA, and downstream activation through privacy-safe UTMs and
first-party events. Revalidate after material product, price, feature, integration, status, legal, or brand changes;
complete quarterly verification prompts truthfully.

Before external action, confirm exactly-five evidence, eligibility, duplicate decision, live field/limit capture,
category/competitor fit, source-backed claims, media rights, verified-owner route, private-data exclusion, and human
approval. End with `READY TO SUBMIT`, `READY TO VERIFY/UPDATE`, `LIVE — OPERATIONS ACTIVE`, or
`NOT READY — BLOCKERS REMAIN`.

