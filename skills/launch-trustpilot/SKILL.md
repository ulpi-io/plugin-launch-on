---
name: launch-trustpilot
description: |
  Claim, create, optimize, and operate a Trustpilot business profile and a compliant customer-review program.
  Covers domain and duplicate checks, the four-step business-account flow, profile details, categories,
  locations, top-five live category research with the browse skill, conversion-focused profile copy, supported
  review invitations, neutral outreach, replies, flagging, TrustScore and category-rank interpretation,
  analytics, and ongoing reputation operations. Writes a paste-ready package under .ulpi/launch/trustpilot.
  Use when a startup wants to establish, correct, improve, or grow its company or product-brand presence on
  Trustpilot without review gating, incentives, fake reviews, or other reputation manipulation.
---

<HUMAN-WRITING-RULES>
For every user-facing prose artifact produced by this skill, run the full embedded-mode process in `../../references/human-writing.md` before finalizing. Its no-fabrication rule and all 33 pattern checks are mandatory; preserve the intended platform voice and do not alter code, structured data, link targets, quotations, titles, or proper names.
</HUMAN-WRITING-RULES>

<EXTREMELY-IMPORTANT>
Treat these rules as blocking:

1. LIST THE RIGHT BUSINESS AND DOMAIN. Trustpilot profiles represent a business/domain. Confirm whether the
   product brand has its own customer relationship and canonical domain or belongs on the parent-company
   profile. Do not create fragmented profiles for plans, features, apps, or editions.
2. SEARCH BEFORE SIGNUP OR CLAIMING. Search the canonical domain, brand, legal/trading name, former domains,
   country variants, and spelling variants. Claim, correct, or request an eligible merge instead of creating a
   duplicate. A business may already have an unclaimed profile because a consumer reviewed it.
3. USE AUTHORIZED, ACCURATE DETAILS. The user must be an authorized representative. Business name, domain,
   category, locations, contacts, services, guarantees, and claims must be current, relevant, and not misleading.
4. USE $browse AND RESEARCH THE TOP FIVE. Before final profile copy or category recommendations, inspect the
   live Trustpilot category, exactly five relevant leading organic profiles, and their vendor sites. Record the
   market, filters, ordering, date, URLs, and any sponsored placements separately. Search snippets alone do not
   satisfy this gate.
5. INVITE FAIRLY. Invite all eligible customers at the same defined experience point using fair, neutral,
   unbiased language and a Trustpilot-supported method. Never cherry-pick happy customers or gate invitations
   behind satisfaction, NPS, support outcomes, refunds, plan, spend, geography, or predicted sentiment.
6. NEVER INCENTIVIZE OR FABRICATE. Do not offer discounts, money, points, gifts, coupons, refunds, contest
   entries, referral benefits, or any value for a review. Never buy, write, ghostwrite, generate, coordinate,
   pressure, or ask users to edit/delete reviews. Owners, employees, close family, shareholders, competitors,
   and others with conflicts of interest must not review.
7. PROTECT CUSTOMER DATA. Use only data the business may lawfully process for this purpose, disclose the
   processor/workflow as required, minimize fields, honor opt-outs, set retention, and never persist customer
   lists, passwords, activation links, one-time codes, or private reviewer data in launch artifacts.
8. RESPOND AND FLAG HONESTLY. Reply professionally without disclosing personal information. Flag only a real
   guideline breach with evidence; disagreement, criticism, or a low star rating is not a valid flagging reason.
9. DO NOT PROMISE A SCORE OR RANK. TrustScore is not a simple average and category positions change. Separate
   controllable customer-experience and operational work from outcomes. Separate Free-plan capabilities from
   paid or add-on features and verify current entitlements before recommending them.
10. VERIFY AND PERSIST. Recheck the live form, public profile, plan, and official legal guidance immediately
    before external action. Write the complete Markdown package under `.ulpi/launch/trustpilot`.
</EXTREMELY-IMPORTANT>

# Launch on Trustpilot

## Goal

Produce:

- `SUBMISSION.md` — mode, duplicate evidence, account flow, ownership, and every current setup field
- `PROFILE.md` — paste-ready public profile copy, categories, contact details, services, guarantees, and media
- `CONTENT-REQUIREMENTS.md` — listing-derived matrix of required, recommended, plan-gated, and generated content
- `CATEGORY-EVIDENCE.md` — category choice, market/country context, and evidence for every category
- `BENCHMARK.md` — dated `$browse` analysis of exactly five relevant organic profiles
- `REVIEW-PLAN.md` — eligible audience, supported invitation method, neutral templates, cadence, and privacy
- `RESPONSE-PLAYBOOK.md` — response SLAs, safe templates, escalation, recovery, and legitimate flagging
- `OPERATIONS.md` — plan entitlements, owners, 30/60/90-day work, maintenance, and incident handling
- `CHECKLIST.md` — blocking gates and one final readiness verdict
- `analytics.md` — profile/referral, invitation, review, response, and downstream-conversion measurement
- shared `.ulpi/launch/positioning.md` — grounded product and business truth

## Step 0: Identify the business profile and mode

If not unambiguous, ask:

> Which business or product brand are you listing on Trustpilot? Send its canonical business domain, primary
> country/market, and any existing Trustpilot profile URL.

Do not infer the target from the repository name. Determine one mode:

- `NEW` — no profile exists and signup is appropriate
- `CLAIM` — an accurate unclaimed profile already exists
- `CORRECT` — the page has a wrong name, domain, country, category, or other material fact
- `MERGE` — multiple profiles represent the same eligible business/domain history
- `OPTIMIZE` — claimed profile is incomplete or weak
- `GROW` — profile is accurate and needs a compliant review and response system

Gather canonical domain, business and trading names, country, customer relationship, owner authority, existing
profile(s), former domains/names, locations, primary buyer category, customer lifecycle, review volume, current
invitation method, CRM/commerce/support stack, privacy owner, and Trustpilot plan. Ask one grouped follow-up only
for private or unknowable facts.

## Step 1: Load references and require browse

Read:

- `references/account-and-profile.md` before signup, claim, correction, merge, or profile work
- `references/benchmarking-and-copy.md` before category research, top-five analysis, or public copy
- `references/reviews-and-compliance.md` before invitations, replies, flags, or reviewer outreach
- `references/trustscore-and-operations.md` before score/rank interpretation, analytics, or ongoing work
- `references/artifact-templates.md` before writing the final package

Use `$browse`; start with `browse --version`. If it is unavailable, suggest without installing automatically:

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

CLI:

~~~bash
npm install -g @ulpi/browse
browse --version
~~~

Use one persistent session. Inspect live renders with `goto`, `wait --load networkidle`, `snapshot -i`, `text`,
and `links`. Try the exact category slug rather than relying only on the categories index. If ordinary access is
blocked, load and follow `$browse-stealth`: verify Camoufox, stop the current server, retry in headed Camoufox,
and wait for stability. If stealth remains blocked by IP reputation, require the permitted user-assisted handoff
or residential proxy. Mark `BENCHMARK.md` `BLOCKED — LIVE TOP-FIVE BROWSE REQUIRED` and do not recommend final
category/copy until five profiles are read.

## Step 2: Ground business and product truth

Reuse `.ulpi/launch/positioning.md` only when current. Otherwise browse the canonical site, pricing, product,
help center, legal pages, and relevant app stores, then record:

- exact customer-facing brand, legal/trading entity, domain, country, and contact details
- what is sold, to whom, the primary job, and the customer experience Trustpilot reviewers would evaluate
- current capabilities, service promises, differentiators, and credible guarantees
- availability, regions, locations, languages, pricing, trial/free status, and support channels
- customer lifecycle events that qualify as genuine experiences
- current CRM, billing, commerce, support, and email systems
- evidence URL, owner, and last-verified date for every public claim

Do not publish roadmap features, unsupported guarantees, invented numbers, or vague superlatives. Decide whether
the product brand deserves its own domain profile or should remain on the parent-company profile.

## Step 3: Search profiles and resolve ownership

With `$browse`, search Trustpilot and the public web for:

- exact canonical domain with and without `www`
- business, trading, and product-brand names
- former names and domains
- country/localized variants and common misspellings

Record every query and candidate URL in `SUBMISSION.md`. Compare domain, name, locations, reviews, and Company
activity. Issue one verdict:

- `NEW PROFILE — SIGNUP PATH`
- `EXISTING UNCLAIMED PROFILE — CLAIM`
- `EXISTING CLAIMED PROFILE — REQUEST ACCESS`
- `CORRECTION REQUIRED`
- `POTENTIAL MERGE — SUPPORT REVIEW REQUIRED`
- `AMBIGUOUS — BLOCKED`

Never create a duplicate to escape old reviews or a low TrustScore. Never promise deletion: once a business is
reviewed, its profile and reviewer-owned content generally remain unless content breaches platform rules.

## Step 4: Complete the account and claim worksheet

Use the live form as final truth. The observed July 23, 2026 signup flow has four stages:

1. `Business details` — Business location, Business name, Business website
2. `Additional details` — capture every live label and required state at execution time
3. `Personal details` — First name, Last name, Phone number with selected country code
4. `Activate account` — let the user complete private email/account verification directly

The business-name control may surface Dun & Bradstreet data. Select only the correct entity; do not force a
near match. In `SUBMISSION.md`, put fields in live order with `READY TO PASTE`, `SELECT`, `ENTER DIRECTLY`, or
`BLOCKED`. Include exact visible limits and deterministic character counts. Do not store passwords, verification
links/codes, or unrequested private contact data. Record the current privacy/marketing notice for user review.

For an existing page, follow the claim/access flow instead of signup. Keep proof of authority minimal and share
it only through Trustpilot's official channel. Do not falsely claim affiliation.

## Step 5: Research the live category and top five

Define the primary customer job and candidate Trustpilot category. Open the relevant country/category page with
`$browse` and inspect exactly five leading organic profiles a buyer would reasonably compare. If the page shows
promoted/sponsored placements, record them separately and do not count them as organic top five unless the user
explicitly asks for an advertising analysis.

For every profile capture:

- displayed position, profile URL, claimed status, business domain, country, and categories
- TrustScore, star label, total review count, visible review recency, and rating distribution when shown
- Company activity: invitation sources, reply behavior, flagging transparency, and merge history when visible
- profile completeness: logo/header, description, services, guarantees, contacts, locations, and promotions
- response coverage, tone, apparent SLA, and whether critical reviews receive useful answers
- buyer questions answered, trust objections handled, and credible whitespace
- vendor-site positioning, proof, contact/checkout flow, and consistency with the Trustpilot profile

Before drafting, compare all five profiles and write `CONTENT-REQUIREMENTS.md`. Classify every observed element:

- `REQUIRED/BASELINE` — necessary to identify the business and avoid a thin or ambiguous profile
- `RECOMMENDED` — repeatedly used by strong relevant profiles and useful to buyers
- `PLAN-GATED` — visible on paid profiles or the live account only; verify entitlement
- `TRUSTPILOT-GENERATED` — score, AI summary, top mentions, ranking, distribution, review labels, and activity
- `NOT RELEVANT` — present on a peer but not truthful/useful for this business

For each business-controlled item record the exact live field/surface, source input, character/file constraints,
buyer question answered, evidence required, and owner. For platform-generated content, record the operational
inputs the business can ethically improve, but never write or promise the output. Do not begin profile copy until
this matrix exists.

Do not collect reviewer personal data or copy review text. Summarize themes. Record category URL, country/filter,
sort/order, timestamp/timezone, access method, and the reason each company belongs in the comparison set.

## Step 6: Select categories with evidence

Use `references/benchmarking-and-copy.md`. Choose the narrowest accurate primary category matching what customers
buy, not the largest category. Add only supported secondary categories. The current official profile guidance
has described one primary and up to five additional categories, but verify the live limit before writing.

For each category, record:

- exact current label and URL
- native offer/capability evidence
- buyer intent and benchmark peers
- country availability and category-page eligibility
- `PASS`, `BORDERLINE — TRUSTPILOT REVIEW`, or `FAIL`

Do not category-stuff. Trustpilot makes the final display/ranking decisions and may use its own classification.

## Step 7: Build the public profile

Use the live `Settings > Public profile settings` surface and `references/account-and-profile.md`. Populate all
available fields that are accurate for the user's plan:

- business name and canonical domain
- square logo and plan-eligible header image
- company description
- primary and additional categories
- services/customer-service highlights and real guarantees
- website, business email/phone/address/hours when appropriate
- locations/branches only when real and operational
- promotion banner only when current, truthful, and plan-eligible

Treat `CONTENT-REQUIREMENTS.md` as the drafting contract. A field may be omitted only with a documented reason,
not because a benchmark peer omitted it. Keep business-authored copy separate from descriptions imported from
external sources and from Trustpilot-generated review summaries/topics.

Draft three description angles: buyer-job led, differentiation led, and trust/reassurance led. Score factuality,
clarity, category fit, differentiation, buyer objections, scanability, and consistency with the site. Recommend
one using the top-five evidence. Never copy competitors or reviews. Keep claims specific and verifiable.

For each media asset specify source file, dimensions, crop/safe area, alt/context note, owner, and freshness.
Remove PII, test data, secrets, internal URLs, and unreleased features. Preview desktop and mobile before publish.

## Step 8: Design the compliant review program

Use `references/reviews-and-compliance.md`. Define a universal eligibility rule based on a genuine completed
experience, not predicted satisfaction. Map the full eligible population, exclusions required by law/policy,
send event, delay, frequency cap, opt-out/suppression, method, owner, and audit evidence.

Select only a currently supported Trustpilot method visible in the business account, such as a plan-eligible
automatic invitation, approved integration, manual platform upload/send, or supported business-generated link.
Verify entitlement and limits live; do not assume. The current public pricing page advertises 50 automated
invitations/month on Free, but record the live plan truth because allowances change.

Create neutral email/SMS/in-app variants that:

- ask for an honest review, not a positive or five-star review
- state why the recipient is receiving it and identify the business
- contain the official Trustpilot destination generated by a supported method
- do not offer value or condition support/refunds on review action
- include required privacy/opt-out information
- use the same wording and timing for the full eligible cohort

Do not generate review text for customers. Test delivery, identity/reference mapping, duplicates, suppression,
mobile rendering, and failure handling with internal non-review test accounts before enabling production sends.

## Step 9: Build the response and recovery playbook

Set owners, coverage, and risk-based SLAs. Reply to positive and critical reviews without demanding a change.
Each response should acknowledge the experience, address what can be addressed publicly, protect personal data,
offer a private resolution path where useful, and close with accountability. Do not paste repetitive SEO copy.

For a possible violation, preserve the profile URL, review ID, visible text, dates, transaction lookup result,
and exact guideline ground. Flag only through Trustpilot's supported flow. Do not flag merely because a review is
negative, unfair in the business's view, or disputed. Never disclose the evidence publicly.

Convert recurring review themes into product/service work with owner, severity, frequency, action, due date,
and a feedback-to-fix closure check. Ask for an updated review only if Trustpilot's current rules allow neutral
follow-up; never pressure, bargain, or link resolution to editing/deletion.

## Step 10: Interpret score, rank, and progress correctly

Use `references/trustscore-and-operations.md`. Explain that TrustScore considers time span, frequency, and a
Bayesian average; it is not a raw arithmetic mean. Category position and labels are dynamic. Never calculate a
guaranteed number or claim payment changes organic score/rank.

Report controllable leading indicators separately from outcomes:

- eligible experiences, invite coverage, delivery, opt-outs, and review conversion
- review volume/recency, rating distribution, reply coverage/time, unresolved critical themes
- profile views and website referrals where available
- TrustScore, star label, category position, branded search, and downstream conversion

Annotate plan-gated metrics. Use Trustpilot dashboard data only within its permitted scope; do not republish
restricted competitor analytics or use a benchmark for unsupported comparative advertising.

## Step 11: Validate, hand off, and maintain

Write every artifact from `references/artifact-templates.md`. Then verify:

- the public URL resolves to the intended domain/profile and no duplicate remains unresolved
- the claimed label, name, domain, category, contacts, copy, locations, and assets render correctly
- the top-five benchmark is live, dated, and contains exactly five relevant organic profiles
- listing-derived content requirements are classified and every applicable controlled field is complete
- invitation cohort, wording, supported method, privacy, suppression, and limits pass compliance review
- replies/flags have owners and evidence standards
- free/paid entitlements are current and clearly separated
- analytics record a baseline and do not expose customer or reviewer data

Issue exactly one verdict in `CHECKLIST.md`:

- `READY TO CLAIM/CREATE`
- `READY TO PUBLISH PROFILE`
- `READY TO ENABLE INVITATIONS`
- `LIVE — OPERATIONS ACTIVE`
- `NOT READY — BLOCKERS REMAIN`

Do not perform final signup, claim, publish, invitation activation, paid upgrade, or bulk customer upload without
explicit user approval at that action. After launch, run weekly review/response checks, monthly profile and
entitlement checks, quarterly category/benchmark refreshes, and immediate incident review for warnings, unusual
review patterns, delivery failures, privacy issues, rebrands, acquisitions, or domain changes.

## Completion contract

Do not call the work complete until:

- the right business/domain and mode are explicit
- duplicates and ownership are resolved or clearly blocked
- `$browse` produced a live, dated five-profile category benchmark
- five listings were compared into a complete content-requirements matrix before drafting
- all live account/profile fields are paste-ready or safely marked for direct entry
- profile copy and categories trace to evidence
- review invitations are neutral, universal, supported, private, and tested
- response, flagging, recovery, analytics, owners, and cadence are documented
- the public profile and current plan entitlements have been reverified
