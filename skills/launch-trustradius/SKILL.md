---
name: launch-trustradius
description: |
  Create, claim, optimize, and operate a TrustRadius B2B technology product profile. Covers eligibility and
  duplicates, vendor signup/claim, mandatory live category and top-five profile research with $browse and
  $browse-stealth fallback, every profile content surface, categories, features, pricing, integrations, security,
  media and demos, conversion copy, authentic long-form review generation, awards, analytics, and ongoing
  maintenance. Writes a paste-ready package under .ulpi/launch/trustradius. Use when a software vendor wants to
  get listed, improve profile completeness, grow trustworthy reviews, or convert in-market TrustRadius buyers.
---

<HUMAN-WRITING-RULES>
For every user-facing prose artifact produced by this skill, run the full embedded-mode process in `../../references/human-writing.md` before finalizing. Its no-fabrication rule and all 33 pattern checks are mandatory; preserve the intended platform voice and do not alter code, structured data, link targets, quotations, titles, or proper names.
</HUMAN-WRITING-RULES>

<EXTREMELY-IMPORTANT>
Treat these rules as blocking:

1. LIST THE RIGHT PRODUCT. TrustRadius profiles represent distinct B2B technology products. Do not create thin
   pages for plans, features, services, editions, or regional variants. Search and claim/correct before creating.
2. REQUIRE AUTHORITY AND AVAILABILITY. The user must represent the vendor and the product must be available to
   real business users. Keep company and product identities, URLs, categories, claims, and pricing accurate.
3. USE $browse AND EXACTLY FIVE LIVE PROFILES. Inspect the current category, exactly five relevant profiles,
   and their vendor sites before final categories or copy. Search snippets do not satisfy this gate.
4. USE $browse-stealth WHEN BLOCKED. On 403/challenge, verify Camoufox, stop the normal server, retry headed,
   stabilize, and inspect the rendered page. If stealth remains blocked by IP reputation, require the permitted
   handoff/proxy and leave the top-five gate blocked. Never fabricate observations.
5. RESPECT THE ORGANIC ORDER. TrustRadius currently states its category lists are based on reviews and profile
   completeness, without paid placement or analyst influence. Record the live promise and ordering. Keep Free
   profile completeness, Premium capabilities, awards, and organic category position separate.
6. COMPLETE EVERY APPLICABLE FIELD. Description, categories/use cases, media, demos, pricing, features,
   integrations, technical/deployment details, security, competitors/alternatives, company data, CTAs, and
   plan-gated content require first-party evidence. Do not publish roadmap or inferred capabilities.
7. NEVER MANIPULATE REVIEWS. Invite a consistently defined genuine-user cohort with neutral language. Do not
   gate, cherry-pick, fabricate, ghostwrite, pressure, or condition invitations on satisfaction or rating.
8. HANDLE INCENTIVES ONLY THROUGH TRUST RADIUS. Public profiles may label reviews Incentivized. Never offer an
   independent incentive. Verify the current TrustRadius-managed campaign, eligibility, disclosure, value,
   country, recipient, and plan rules before any incentive workflow.
9. DO NOT PROMISE SCORES, AWARDS, AI INSIGHTS, OR RANK. These are TrustRadius-controlled outputs. Improve the
   truthful profile, user experience, review coverage, and responsiveness; never guarantee the result.
10. VERIFY LIVE AND PERSIST. Forms, plan entitlements, content limits, award rules, and review policies change.
    Recheck before external action and write the complete package under `.ulpi/launch/trustradius`.
</EXTREMELY-IMPORTANT>

# Launch on TrustRadius

## Goal

Produce:

- `ELIGIBILITY-AND-CLAIM.md` — identity, duplicates, authority, mode, account/claim flow, and verdict
- `SUBMISSION.md` — every live vendor-portal field in exact order with paste-ready values and limits
- `CONTENT-REQUIREMENTS.md` — five-profile-derived baseline, recommended, generated, and plan-gated content
- `CATEGORY-EVIDENCE.md` — primary/additional category and use-case evidence
- `BENCHMARK.md` — dated `$browse` analysis of exactly five relevant organic profiles
- `PROFILE.md` — descriptions, details, pricing, features, integrations, security, media, demos, and CTAs
- `REVIEW-PLAN.md` — fair cohort, neutral templates, campaign method, privacy, QA, and response workflow
- `AWARDS-AND-OPERATIONS.md` — current award criteria, entitlements, owners, maintenance, and 30/60/90-day plan
- `CHECKLIST.md` — blocking gates and final verdict
- `analytics.md` — profile, referral, review, intent, and conversion measurement
- shared `.ulpi/launch/positioning.md` — current product truth

## Step 0: Identify product and mode

If not unambiguous, ask:

> Which B2B technology product are you listing on TrustRadius? Send its canonical product URL, company name,
> primary category/buyer, and any existing TrustRadius product URL.

Do not infer from the repository name. Determine `NEW`, `CLAIM`, `REQUEST ACCESS`, `CORRECT`, `OPTIMIZE`, or
`GROW`. Gather product/company names, canonical URL, availability, buyer, owner authority, existing profiles,
former names/domains, pricing, categories, integrations, deployment, security, review owner, plan, and analytics.

## Step 1: Load references and browser capabilities

Read:

- `references/eligibility-claim-and-fields.md` before signup, claim, duplicate, or form work
- `references/profile-benchmark-and-copy.md` before top-five research, categories, content, or assets
- `references/reviews-awards-and-operations.md` before invitations, incentives, awards, plans, or analytics
- `references/artifact-templates.md` before writing final artifacts

Use `$browse`; start with `browse --version`. If missing, suggest the browse plugin for Claude Code or Codex
without installing automatically. Use one persistent session. On 403/challenge, load `$browse-stealth`, run
Camoufox doctor, stop the normal server, and retry with headed Camoufox. If still blocked, use the permitted
handoff/proxy path and mark the live research blocked.

## Step 2: Ground product truth

Browse the canonical homepage, product/features, pricing, docs, integrations, security/trust center, support,
legal, demo/trial, and company pages. Record evidence and verification date for:

- exact product and company identity, URLs, audience, job, problem, workflow, and differentiators
- current capabilities, category use cases, deployment, OS/mobile, organization size, geography, and departments
- pricing tiers/units/periods, contact-sales state, free option/trial, demo, and CTAs
- named integrations and API status
- security/compliance claims and evidence
- approved logo, screenshots/captions, videos/demos, customer proof, and rights

Reuse shared positioning only if current. Never convert roadmap, review claims, or assumptions into vendor facts.

## Step 3: Search duplicates and prove eligibility

With `$browse`, search TrustRadius and the web for product/company names, canonical/former domains, spellings,
editions, acquisitions, and existing profiles. Compare name, URL, description, categories, reviews, and company.
Record each query and issue:

- `NEW PROFILE — VENDOR SIGNUP`
- `EXISTING PROFILE — CLAIM`
- `EXISTING CLAIMED PROFILE — REQUEST ACCESS`
- `CORRECTION/MERGE — SUPPORT REVIEW`
- `NOT ELIGIBLE OR AMBIGUOUS — BLOCKED`

Never create a duplicate to escape reviews, old positioning, or access friction.

## Step 4: Capture vendor signup and claim

Use the live claim entry at `https://solutions.trustradius.com/claim-your-profile/` and the Vendor Portal as
final truth. The public claim path currently offers Free and Premium profile routes and sends Free claims to a
vendor login/signup flow. Capture every rendered signup, identity, company, product search/selection, authority,
claim, verification, and access field in exact order.

After access, inventory every `Product Listing` and `Company Listing` field. Mark each `READY TO PASTE`,
`SELECT`, `UPLOAD`, `ENTER DIRECTLY`, `NOT APPLICABLE`, or `BLOCKED`; record live limits and deterministic
counts. Do not store passwords, MFA, verification links/codes, private contacts, or customer lists.

## Step 5: Research category and exactly five profiles

Define the primary buyer job and open the narrow live category with `$browse`. Record category URL, date/timezone,
locale, filters, order, profile-completeness promise, and displayed positions. Inspect exactly five leading
relevant profiles and their first-party sites.

For every profile capture:

- position, product URL, score/review count, badges, pricing/trial/demo labels, and CTA
- product description structure and Categories & Use Cases
- logo and Media gallery count, screenshot/video captions, demos
- pricing detail, integrations, features, security, technical/deployment/mobile details
- competitors/alternatives, awards, company information, and FAQs
- generated buyer/usage data, AI insights, review themes, review recency, incentive labels, and vendor responses
- vendor-site consistency, table stakes, objection handling, and credible whitespace

Do not copy prose or review text. Write `CONTENT-REQUIREMENTS.md` first and classify each element as
`REQUIRED/BASELINE`, `RECOMMENDED`, `FREE`, `PREMIUM/PLAN-GATED`, `TRUSTRADIUS-GENERATED`, or `NOT RELEVANT`,
with exact input, constraint, evidence, buyer question, and owner.

## Step 6: Select categories and use cases

Choose the narrowest category matching the product's core purchased job. Add only categories/use cases with
current native capability. For each candidate record exact label/URL, product evidence, buyer intent, benchmark
peers, category definition/feature expectations, and `PASS`, `BORDERLINE — EDITORIAL REVIEW`, or `FAIL`.
TrustRadius makes final taxonomy decisions. Do not category-stuff.

## Step 7: Build the complete product profile

Using the live Vendor Portal and requirements matrix, prepare all applicable surfaces:

- product/company name, logo, canonical website, short and full description
- Categories & Use Cases
- screenshots with specific captions, videos and product demos
- pricing plans/details, starting price, unit/period, free option/trial, contact-sales state
- category features/capabilities and descriptions
- named integrations and API evidence
- deployment type, OS/mobile applications, supported users/markets, technical details
- security/compliance information with evidence and expiry/owner
- competitors/alternatives, company details, FAQs, and support
- Free or plan-eligible website/demo/contact/lead CTAs
- Premium narrative/custom content only when the live plan allows it

Draft buyer-job, differentiation, and proof/reassurance descriptions. Score factuality, category fit, clarity,
specificity, objection coverage, scanability, and five-profile differentiation; recommend one. Remove PII,
secrets, internal URLs, test data, and unreleased features from assets. Preview desktop and mobile.

## Step 8: Build the authentic review program

Define a universal genuine-use rule, eligible population, permitted exclusions, send event/delay, frequency,
reminder, suppression/opt-out, privacy basis, supported TrustRadius method, owner, and audit evidence. Use the
same neutral invitation for the full cohort. Ask for an honest detailed review, never a positive rating.

Never generate reviewer answers. If TrustRadius asks structured questions, tell users to answer from their own
experience. For incentives, default `NONE`; if explicitly requested, verify and use only a TrustRadius-managed,
properly disclosed campaign. Build response SLAs that protect PII and never pressure reviewers to edit/delete.

## Step 9: Awards, plans, analytics, and operations

Record current award eligibility and date windows from official live rules; do not promise qualification.
Separate Free profile fields from Premium capabilities such as enhanced narrative/content, review/refresh
campaigns, custom questions, content licensing/TrustQuotes, reference management, intent data, lead capture,
competitive analytics, and integrations. Verify plan and contract.

Create a 30/60/90-day plan and weekly/monthly/quarterly cadence for profile completeness, field freshness,
pricing/features/integrations/security, assets, broken CTAs, review coverage/recency, responses, categories,
awards, access, and privacy.

Measure profile/category views where exposed, referral sessions, CTA/demo/trial/contact conversion, review
starts/completions/recency, response SLA, category position, award state, and Premium intent/leads only when
entitled. Use privacy-safe UTMs and first-party events.

## Step 10: Validate and hand off

Write every artifact from the templates and verify duplicate/authority, live form, exact five profiles, normal
browse plus stealth fallback, category evidence, complete truthful fields, asset QA, review fairness, privacy,
plan entitlements, and public display. Final verdict:

- `READY TO CLAIM`
- `READY TO SUBMIT NEW PRODUCT`
- `READY TO PUBLISH/UPDATE PROFILE`
- `READY TO ENABLE REVIEW CAMPAIGN`
- `LIVE — OPERATIONS ACTIVE`
- `NOT READY — BLOCKERS REMAIN`

Never submit, publish, invite reviewers, purchase a plan, or contact customers without explicit user approval.
