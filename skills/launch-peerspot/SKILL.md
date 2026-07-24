---
name: launch-peerspot
description: |
  Request, claim, optimize, and operate a PeerSpot enterprise-technology product listing. Covers vendor inquiry,
  duplicate checks, category and product fit, mandatory live top-five research with $browse and $browse-stealth
  fallback, product profile content, reviews, comparisons, buyer-intent positioning, marketplaces, analytics, and
  ongoing maintenance. Writes a paste-ready package under .ulpi/launch/peerspot. Use when an enterprise software
  vendor wants to establish or improve its PeerSpot presence without manipulating reviews or buyer conversations.
---

<HUMAN-WRITING-RULES>
For every user-facing prose artifact produced by this skill, run the full embedded-mode process in `../../references/human-writing.md` before finalizing. Its no-fabrication rule and all 33 pattern checks are mandatory; preserve the intended platform voice and do not alter code, structured data, link targets, quotations, titles, or proper names.
</HUMAN-WRITING-RULES>

<EXTREMELY-IMPORTANT>
Treat these rules as blocking:

1. LIST A REAL ENTERPRISE TECHNOLOGY PRODUCT. Confirm the vendor owns or is authorized to represent the product,
   it has real business users, and it belongs in an active PeerSpot category. Do not list services, modules,
   reseller offers, prototypes, or duplicate editions as independent products.
2. SEARCH BEFORE CONTACTING PEERSPOT. Search product, company, spelling variants, former names, acquired brands,
   category, and comparison URLs. Claim/correct an existing product instead of opening a duplicate.
3. USE $browse AND EXACTLY FIVE LIVE PEERS. Before final category or copy, inspect the live category, exactly five
   comparable products, their public profiles/reviews, comparison pages, and official vendor sites. Snippets do
   not satisfy this gate.
4. USE $browse-stealth WHEN BLOCKED. Normal browse is first. If a 403/challenge occurs, use headed Camoufox.
   If the block remains IP-based, document it, request the permitted handoff/proxy, and leave the benchmark
   `BLOCKED — LIVE TOP-FIVE BROWSE REQUIRED`; do not invent profile observations.
5. BE PRECISE ABOUT PEERSPOT'S REVIEW MODEL. Public pages say reviewers are verified real users within the last
   12 months, reviews are typically long-form and include both pros and cons, and reviewer/company context may be
   visible. Do not promise publication, verification, rankings, comparisons, or buyer-intent outcomes.
6. NEVER MANIPULATE REVIEWS OR COMMUNITY. Do not fabricate, buy, ghostwrite, edit, coordinate, gate, pressure,
   or condition reviews by sentiment, NPS, plan, spend, support outcome, geography, or employee relationship.
   Never pose as an independent user or seed questions/comments deceptively.
7. USE VENDOR-SPONSORED PROGRAMS ONLY. Any review capture, content, demand-generation, intent-data, marketplace,
   or award offer is subject to PeerSpot's current commercial terms. Verify entitlement and program rules; never
   independently offer incentives or claim a sponsored placement is organic.
8. PROTECT CUSTOMER DATA. Use only permitted business contact data, minimize fields, disclose processing as
   needed, honor opt-outs/suppression, retain only what is needed, and never save customer lists or credentials
   in launch artifacts.
9. MAKE EVERY CLAIM CURRENT AND PROVABLE. Product description, pricing, deployment, integrations, security,
   marketplace availability, customers, and media require first-party evidence. Do not publish roadmap claims,
   fake metrics, secret screenshots, or competitor attacks.
10. VERIFY AND PERSIST. Recheck the live form, category, profile, FAQ/policies, and plan before external action;
    write the full package under `.ulpi/launch/peerspot`.
</EXTREMELY-IMPORTANT>

# Launch on PeerSpot

## Goal

Produce:

- `ELIGIBILITY-AND-REQUEST.md` — identity, duplicate search, route, vendor inquiry, and listing verdict
- `SUBMISSION.md` — every live contact/onboarding field in exact order with paste-ready values and limits
- `BENCHMARK.md` — dated `$browse` analysis of exactly five relevant live products
- `CONTENT-REQUIREMENTS.md` — listing-derived baseline, recommended, generated, and plan-gated content
- `CATEGORY-AND-COMPARISONS.md` — category, alternatives, comparison evidence, and positioning
- `PROFILE.md` — buyer-facing product content, claims, assets, and conversion surfaces
- `REVIEW-AND-COMMUNITY-PLAN.md` — fair review program, discussion conduct, privacy, and response playbook
- `OPERATIONS.md`, `CHECKLIST.md`, `analytics.md`, and shared `.ulpi/launch/positioning.md`

## Step 0: Identify product and listing mode

Ask if unclear:

> Which enterprise technology product are you listing on PeerSpot? Send its canonical URL, company name, target
> category, marketplace availability, and any existing PeerSpot product/company URL.

Determine `NEW`, `CLAIM`, `CORRECT`, `OPTIMIZE`, `GROW`, or `MARKETPLACE-EXTEND`. Gather owner authority,
canonical company/product names, public product site, enterprise buyer, category, actual use cases, pricing,
deployment, integrations, security, marketplaces, customer-review owner, and current commercial relationship.

## Step 1: Load references and require live browser research

Read:

- `references/request-and-profile.md` before inquiry, duplicates, onboarding, or profile fields
- `references/benchmark-category-and-copy.md` before top-five/category/comparison/copy work
- `references/reviews-community-and-operations.md` before review sourcing, interactions, entitlements, or analytics
- `references/artifact-templates.md` before writing the final package

Use `$browse`; run `browse --version`. If normal browsing is blocked, load `$browse-stealth`, verify Camoufox,
stop normal browse, and retry in headed Camoufox. If still blocked, do not replace rendered peer analysis with
search snippets: require the permitted user handoff/residential proxy and mark the live gate blocked.

## Step 2: Ground product and vendor truth

Browse the product site, feature/use-case pages, pricing, documentation, integration directory, support,
security/trust center, legal pages, marketplace listings, and brand assets. Record sources/verification dates for:

- exact vendor/product identity, buyer, job, workflow, deployment, and differentiators
- pricing/trial/demo/contact path, target company sizes/industries, regions, and support
- feature and technical claims, integrations/API, security/compliance, and marketplace status
- approved logo/screenshots/video/demo, asset rights, freshness, and public-safe captions

Reuse shared positioning only when current. Never infer enterprise fit or capability from a competitor page.

## Step 3: Search duplicates, categories, and comparisons

With `$browse`, search exact/variant product and company names, former/acquired names, existing category pages,
product pages, vendor pages, and comparison URLs. Record candidate URLs and issue:

- `NEW — REQUEST LISTING`
- `EXISTING — CLAIM/REQUEST ACCESS`
- `CORRECTION OR MERGE — PEERSPOT REVIEW`
- `CATEGORY FIT UNCERTAIN — REQUEST GUIDANCE`
- `NOT READY — BLOCKER`

Choose the narrowest accurate category. Competitors must solve the same primary job for a similar buyer. Never
inject a product into comparisons merely to capture branded search traffic.

## Step 4: Capture the vendor request

The observed July 23, 2026 PeerSpot vendor contact form at `company.peerspot.com/about-us/contact` shows:

- First Name, Last Name, Email, Company Name
- AWS Marketplace status and Google Cloud Marketplace status checkboxes
- Area of Interest: Content marketing, Customer advocacy, Demand generation, Product marketing, Listing my
  product/company, LLM Influence, AWS Marketplace, peerspot.ai, Google Marketplace, or Report a bug
- Message and Get in touch

For a new listing select `Listing my product/company`; report marketplace status truthfully. Capture all fields
revealed after submission and any PeerSpot response in exact live order. Use `READY TO PASTE`, `SELECT`,
`ENTER DIRECTLY`, `BLOCKED`, or `NOT APPLICABLE`; record visible constraints. Do not store authentication,
verification details, contract terms, or private contacts beyond role/owner.

## Step 5: Benchmark exactly five live products

Open the target category and capture timestamp/timezone, filters, sort/order, category definition, product count,
and selection rule. Read exactly five comparable product profiles and official vendor sites. Also inspect one or
more relevant comparison pages. Capture:

- displayed rank/order, product/vendor URL, rating/review count, review recency, reviewer role/company context
- overview, benefits, limitations, features, integrations, deployment, pricing, and vendor details when present
- long-form review patterns: use case, pros, cons, ROI, comparison/alternatives, and buyer objections
- community questions/discussions only as themes; never use them as vendor-authored content
- profile completeness, media, category fit, comparison positioning, and vendor-site consistency

Create `CONTENT-REQUIREMENTS.md` before draft copy. Classify `REQUIRED/BASELINE`, `RECOMMENDED`,
`PEERSPOT-GENERATED`, `VENDOR-PROGRAM/PLAN-GATED`, or `NOT RELEVANT`; attach exact input, constraint, evidence,
buyer question, and owner. Summarize—do not copy reviewers' prose.

## Step 6: Build profile, category, and comparison package

Prepare every available, truthful profile surface: product/company identity, concise and full description, category,
features/use cases, pricing/contact state, deployment, integrations/API, security/trust proof, screenshots/video,
documentation, support, marketplaces, approved alternatives, and conversion destination.

Draft three angles: buyer-job, technical/workflow, and proof/reassurance. Score factuality, category fit,
specificity, buyer objections, scanability, and difference from the exact five. Recommend one with source links.
For media, list source, rights, dimensions, caption, crop/safe area, PII/secret check, owner, and freshness.

## Step 7: Design fair review and community operations

Define a universal post-use eligibility rule, full eligible cohort, send event/delay, frequency cap, reminder,
suppression, privacy basis, permitted PeerSpot method, owner, and audit evidence. Use neutral invitations asking
for an honest, detailed experience. Do not ask for a rating, five stars, or a specific answer.

Public PeerSpot material says reviews are verified from real users of the past 12 months and include pros/cons.
Respect that: never generate answers, alter feedback, or turn a review request into sales outreach. If PeerSpot
offers gift cards or campaigns, use only its current documented/administered program. Vendor/community answers
must identify affiliation, be factual/helpful, protect PII, and never attack competitors or manipulate votes.

## Step 8: Operate, measure, and validate

Separate current profile/listing basics from paid/vendor-program capabilities such as content marketing, customer
advocacy, demand generation, product marketing, buyer intelligence, marketplace programs, LLM influence, custom
content, or awards. Verify entitlements in writing before recommending them.

Measure profile/category referrals, comparison referrals, CTA/demo/trial conversion, review invites/starts/
approvals/recency, response SLA, community participation, marketplace referrals, and downstream conversion using
privacy-safe UTMs and first-party events. Do not scrape reviewer identities.

Write all artifacts, confirm exactly-five evidence and browser fallback, public claim truth, category/comparison
fit, private-data exclusion, and final verdict: `READY TO REQUEST LISTING`, `READY TO CLAIM/UPDATE PROFILE`,
`READY TO ENABLE REVIEW PROGRAM`, `LIVE — OPERATIONS ACTIVE`, or `NOT READY — BLOCKERS REMAIN`.

Never submit, publish, contact PeerSpot, start a review campaign, purchase a program, or contact customers
without explicit user approval.
