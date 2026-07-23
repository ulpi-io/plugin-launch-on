# TrustRadius Artifact Templates

Write under `.ulpi/launch/trustradius/`. Use ISO dates/timezone, source URLs, owners, exact limits, and statuses.
Never store credentials, MFA, customer lists, reviewer PII, or private evidence.

## ELIGIBILITY-AND-CLAIM.md

~~~markdown
# TrustRadius Eligibility and Claim
## Product/company identity and mode
## Duplicate search
| Query | Result URL | Match | Action |
|---|---|---|---|
## Authority and eligibility
## Existing access/profile state
## Verdict
NEW PROFILE — VENDOR SIGNUP | EXISTING PROFILE — CLAIM | REQUEST ACCESS |
CORRECTION/MERGE — SUPPORT REVIEW | NOT ELIGIBLE OR AMBIGUOUS — BLOCKED
~~~

## SUBMISSION.md

~~~markdown
# TrustRadius Submission
## Run context and browser runtime
## Signup/claim fields in live order
## Product Listing fields in live order
## Company Listing fields in live order
| Section | Exact label | Required | Control/options | Value/status | Count/limit | Evidence |
|---|---|---:|---|---|---|---|
## Assets and private verification
## Blockers and next action
~~~

## CONTENT-REQUIREMENTS.md and BENCHMARK.md

~~~markdown
# TrustRadius Content Requirements
| Element | Evidence across five | Class | Applicable | Exact input | Constraint | Buyer question | Owner | Status |
|---|---|---|---:|---|---|---|---|---|
## Drafting gate
READY FOR DRAFTING | BLOCKED — INPUTS OR LIVE RESEARCH MISSING
~~~

~~~markdown
# TrustRadius Top-Five Benchmark
## Category, filters/order, timestamp/timezone, locale
## Browse version/runtime; normal result; stealth result
## TrustRadius ordering/no-paid-placement statement
| # | Product/profile | Score/reviews/badges | Content strengths | Review/buyer evidence | Gap/opportunity |
|---:|---|---|---|---|---|
## Table stakes, whitespace, copy/category direction, limitations
~~~

## CATEGORY-EVIDENCE.md and PROFILE.md

~~~markdown
# TrustRadius Category Evidence
| Category/use case | URL | Product evidence | Buyer intent | Peer evidence | Verdict |
|---|---|---|---|---|---|
## Primary and additional recommendation
~~~

~~~markdown
# TrustRadius Profile
## Identity and description options
## Recommended copy and scoring
## Categories/use cases
## Media, captions, videos, demos
## Pricing, features, integrations/API
## Security and technical/deployment details
## Competitors, company, FAQs, support
## CTA and Free/Premium entitlement
## Desktop/mobile QA
~~~

## REVIEW-PLAN.md, AWARDS-AND-OPERATIONS.md, analytics.md, CHECKLIST.md

~~~markdown
# TrustRadius Review Plan
## Cohort, eligibility, event, timing, frequency, suppression
## Supported method and privacy
## Neutral invitation templates
## Incentive: NONE | TRUSTRADIUS-MANAGED PENDING LIVE VERIFICATION
## QA, responses, escalation, prohibited conduct
~~~

~~~markdown
# TrustRadius Awards and Operations
## Current award rules and generated-content boundaries
## Free/Premium entitlement matrix
## Owners and 30/60/90-day plan
## Weekly/monthly/quarterly cadence and incidents
~~~

~~~markdown
# TrustRadius Analytics
## Funnel, UTMs, profile/category, review, CTA/conversion, award, intent/lead metrics
## Attribution, exclusions, dashboard, cadence
~~~

~~~markdown
# TrustRadius Readiness Checklist
## Identity/duplicate/authority
## Live form and exact five profiles
## Browse plus stealth fallback
## Content/category/claim/media QA
## Review/privacy/incentive rules
## Plan/award/analytics/operations
## Blockers
## Verdict
READY TO CLAIM | READY TO SUBMIT NEW PRODUCT | READY TO PUBLISH/UPDATE PROFILE |
READY TO ENABLE REVIEW CAMPAIGN | LIVE — OPERATIONS ACTIVE | NOT READY — BLOCKERS REMAIN
~~~
