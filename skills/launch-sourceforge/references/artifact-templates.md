# SourceForge Artifact Templates

## Contents

1. Package rules
2. Route and eligibility
3. Submission
4. Requirements and benchmark
5. Profile and project releases
6. Reviews, operations, analytics, and checklist

## 1. Package rules

Write to `.ulpi/launch/sourceforge/`. Use ISO dates, timezone, exact source URLs, named owners/roles, and
`READY`, `SELECT`, `UPLOAD`, `ENTER DIRECTLY`, `BLOCKED`, or `NOT APPLICABLE`. Never store credentials, PINs,
verification links, signing keys, customer lists, reviewer PII, or private evidence.

## 2. Route and eligibility

~~~markdown
# SourceForge Route and Eligibility
## Identity
- Product/project:
- Canonical URL:
- Company/author:
- Existing SourceForge URL(s):
- Route: BUSINESS_LISTING | OPEN_SOURCE_PROJECT | BOTH_LINKED
- Mode: NEW | CLAIM | CORRECT | OPTIMIZE | OPERATE
## Duplicate search
| Query | Result | Match | Action |
|---|---|---|---|
## Business eligibility evidence
## Open-source eligibility and license evidence
## Authority
## Verdict
ELIGIBLE — CREATE | ELIGIBLE — CLAIM/OPTIMIZE | BOTH ROUTES ELIGIBLE — KEEP PURPOSES DISTINCT AND CROSS-LINK |
SUPPORT REVIEW REQUIRED | NOT ELIGIBLE
~~~

## 3. Submission

~~~markdown
# SourceForge Submission
## Run context
- Form URL:
- Observed:
- Browse runtime: normal | headed Camoufox | user handoff
## Fields in live order
| Section | Exact label | Required | Control/options | Paste-ready value/status | Count/limit | Evidence |
|---|---|---:|---|---|---|---|
## Assets
| Asset | Source | Dimensions/type/size | Rights | Freshness | Status |
|---|---|---|---|---|---|
## Private verification
## Blockers and next action
~~~

## 4. Requirements and benchmark

~~~markdown
# SourceForge Content Requirements
## Active route and comparison context
## Requirement matrix
| Element | Evidence across five | Class | Applicable | Exact input | Constraint | Buyer/user question | Owner | Status |
|---|---|---|---:|---|---|---|---|---|
## Omissions and reasons
## Drafting gate
READY FOR DRAFTING | BLOCKED — INPUTS OR LIVE RESEARCH MISSING
~~~

~~~markdown
# SourceForge Top-Five Benchmark
## Run context
- Route/category/URL:
- Timestamp/timezone:
- Filters/sort/locale:
- Browse version/runtime/session:
- Normal-browser result:
- Stealth fallback result:
- Paid-placement treatment:
## Exactly five relevant pages
| # | Page/product/project | Position/status | Audience/use case | Content/release strengths | Gap/opportunity |
|---:|---|---|---|---|---|
## Sponsored/Partner/promoted entries (separate)
## Table stakes
## Credible whitespace
## Requirements and copy direction
## Limitations and refresh date
~~~

For `BOTH_LINKED`, create separate five-row business and project tables.

## 5. Profile and project releases

~~~markdown
# SourceForge Profile
## Public identity and audience
## Description options
### Buyer-job led
### Differentiation led
### Proof/reassurance led
## Recommended copy and scoring
## Product/company fields
| Field | Paste-ready value | Evidence | Plan | Status |
|---|---|---|---|---|
## Pricing and CTA
## Categories, features, competitors, integrations, API
## Platforms, support, training, regions, languages, organizations
## Media, captions, video, FAQs, assets, demo
## Desktop/mobile QA
~~~

~~~markdown
# SourceForge Project and Releases
## Project metadata
| Field | Paste-ready value | Evidence | Status |
|---|---|---|---|
## Tools, users, roles, labels, and paths
## Current stable release
| Artifact | OS/arch/type | Version | Size/hash/signature | Clean test | Status |
|---|---|---|---|---|---|
## Release notes and instructions
## Source, license, notices, SBOM
## Default download and clean-environment test
## Security/support/retirement plan
~~~

Use `NOT APPLICABLE — BUSINESS ONLY` for `PROJECT-RELEASES.md` when appropriate.

## 6. Reviews, operations, analytics, and checklist

~~~markdown
# SourceForge Review Plan
## Eligibility, cohort, send event, timing, frequency, suppression
## Current supported method and plan
## Neutral templates
## Privacy and QA
## Incentive decision: NONE | OFFICIAL PROGRAM PENDING VERIFICATION
## Response SLA and escalation
## Prohibited conduct acknowledgement
~~~

~~~markdown
# SourceForge Operations
## Owners and access
## Current entitlement matrix
| Capability | Needed | Available | Limit | Free/Paid/Add-on | Evidence/verified |
|---|---:|---:|---|---|---|
## 0–30 / 31–60 / 61–90 days
## Weekly/monthly/quarterly cadence
## Release, support, review, privacy, and security incidents
## Change log
~~~

~~~markdown
# SourceForge Analytics
## Funnel and UTMs
## Business listing metrics
## Project/download metrics
## Review/support metrics
## Attribution, exclusions, dashboard, and reporting cadence
~~~

~~~markdown
# SourceForge Readiness Checklist
## Route/eligibility and duplicate gate
## Authority and live-form gate
## Normal browse plus stealth-fallback gate
## Exact top-five per active route gate
## Content/category/claims gate
## Media and public QA gate
## Project/release/security gate
## Review/privacy gate
## Plan/analytics/operations gate
## Blockers
## Verdict
READY TO SUBMIT BUSINESS LISTING | READY TO CREATE PROJECT | READY TO SUBMIT BOTH LINKED ROUTES |
LIVE — OPERATIONS ACTIVE | NOT READY — BLOCKERS REMAIN
~~~
