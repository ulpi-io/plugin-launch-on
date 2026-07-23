# Trustpilot Artifact Templates

## Contents

1. Package rules
2. SUBMISSION.md
3. PROFILE.md
4. CONTENT-REQUIREMENTS.md
5. CATEGORY-EVIDENCE.md
6. BENCHMARK.md
7. REVIEW-PLAN.md
8. RESPONSE-PLAYBOOK.md
9. OPERATIONS.md
10. CHECKLIST.md
11. analytics.md

## 1. Package rules

Write to `.ulpi/launch/trustpilot/`. Use ISO dates, explicit timezone, named owners/roles, source URLs, and
`READY`, `ENTER DIRECTLY`, `SELECT`, `BLOCKED`, or `NOT APPLICABLE` statuses. Never store passwords, activation
codes/links, customer lists, reviewer PII, or private transaction evidence.

## 2. SUBMISSION.md

~~~markdown
# Trustpilot Submission

## Identity and mode
- Business/product brand:
- Canonical domain:
- Country/market:
- Profile mode: NEW | CLAIM | REQUEST ACCESS | CORRECT | MERGE | OPTIMIZE | GROW
- Authorized owner:
- Existing profile URL(s):
- Verified:

## Duplicate search
| Query | Result URL | Match assessment | Action |
|---|---|---|---|

## Verdict
NEW PROFILE — SIGNUP PATH | EXISTING UNCLAIMED PROFILE — CLAIM | EXISTING CLAIMED PROFILE — REQUEST ACCESS |
CORRECTION REQUIRED | POTENTIAL MERGE — SUPPORT REVIEW REQUIRED | AMBIGUOUS — BLOCKED

## Account/claim fields in live order
| Stage | Exact label | Required | Value/status | Count/limit | Evidence |
|---|---|---:|---|---|---|

## Authority and activation
- Proof route:
- Private fields completed directly:
- Activation status:
- Privacy/marketing notice reviewed:

## Blockers and next action
~~~

## 3. PROFILE.md

~~~markdown
# Trustpilot Profile

## Public identity
- Business name:
- Domain:
- Public profile URL:
- Country:

## Description options
### Buyer-job led
Copy:
Character count:
Score:

### Differentiation led
Copy:
Character count:
Score:

### Trust/reassurance led
Copy:
Character count:
Score:

## Recommendation
- Selected copy:
- Why the benchmark supports it:
- Claim evidence:

## Public fields
| Field | Paste-ready value | Plan entitlement | Evidence | Status |
|---|---|---|---|---|

## Assets
| Asset | Source | Dimensions/type/size | Rights/owner | Freshness | Status |
|---|---|---|---|---|---|

## Desktop/mobile QA
~~~

## 4. CONTENT-REQUIREMENTS.md

~~~markdown
# Trustpilot Content Requirements

## Live comparison context
- Category/market:
- Five profile URLs:
- Observed:

## Requirement matrix
| Element | Evidence across five | Class | Applicable | Exact input needed | Live constraint | Buyer question | Owner | Status |
|---|---|---|---:|---|---|---|---|---|

## Business-controlled baseline
## Recommended conversion content
## Plan-gated enhancements
## Trustpilot-generated sections and ethical operational inputs
## Omissions with reasons
## Drafting gate
READY FOR PROFILE DRAFTING | BLOCKED — CONTENT INPUTS MISSING
~~~

Do not mark ready until all applicable baseline rows have evidence or one precise owner/question.

## 5. CATEGORY-EVIDENCE.md

~~~markdown
# Trustpilot Category Evidence

## Primary customer job

## Candidate categories
| Category | URL/market | Offer evidence | Buyer intent | Peer evidence | Verdict |
|---|---|---|---|---|---|

## Recommendation
- Primary:
- Additional:
- Live limit:
- Trustpilot review uncertainty:
- Verified:
~~~

## 6. BENCHMARK.md

~~~markdown
# Trustpilot Top-Five Benchmark

## Run context
- Timestamp/timezone:
- Country/locale:
- Category URL:
- Filters/order:
- Browse version/session method:
- Sponsored-placement treatment:
- Selection method:

## Five organic profiles
| # | Profile/domain | Score/reviews observed | Categories/activity | Profile/response strengths | Gap/opportunity |
|---:|---|---|---|---|---|

## Table stakes
## Claims to avoid
## Credible whitespace
## Profile and response patterns
## Recommended category and copy direction
## Limitations and refresh date
~~~

Exactly five organic profiles are required. Put promoted entries in a separate optional table.

## 7. REVIEW-PLAN.md

~~~markdown
# Trustpilot Review Plan

## Policy owner and approval
## Genuine-experience eligibility rule
## Full eligible population and permitted exclusions
## Send event, delay, frequency, reminder, and suppression
## Supported method and live plan entitlement
## Data/privacy assessment

## Neutral templates
### Email
### SMS
### In-app

## QA evidence
| Test | Expected | Result | Owner | Date |
|---|---|---|---|---|

## Rollout and reconciliation
## Prohibited conduct acknowledgement
~~~

## 8. RESPONSE-PLAYBOOK.md

~~~markdown
# Trustpilot Response Playbook

## Owners, coverage, and SLA
| Severity/rating | Owner | Target | Escalation |
|---|---|---|---|

## Response principles
## Positive response scaffolds
## Neutral/mixed response scaffolds
## Critical response scaffolds
## Private resolution handoff
## PII and legal-risk rules

## Flagging decision
| Current guideline ground | Evidence required | Not a valid reason | Owner |
|---|---|---|---|

## Warning/incident response
## Feedback-to-fix loop
~~~

## 9. OPERATIONS.md

~~~markdown
# Trustpilot Operations

## Current plan entitlements
| Capability | Needed | Available | Limit | Free/Paid/Add-on | Verified |
|---|---:|---:|---|---|---|

## Baseline
## 0–30 days
## 31–60 days
## 61–90 days
## Weekly/monthly/quarterly cadence
## Access, integration, and data-retention owners
## Incident triggers and escalation
## Change log
~~~

## 10. CHECKLIST.md

~~~markdown
# Trustpilot Readiness Checklist

## Business/domain and duplicate gate
## Authority/account gate
## Live top-five browse gate
## Profile/category/copy gate
## Review fairness and supported-method gate
## Privacy/security gate
## Response/flagging gate
## Entitlement/analytics gate
## Public QA gate

## Blockers

## Verdict
READY TO CLAIM/CREATE | READY TO PUBLISH PROFILE | READY TO ENABLE INVITATIONS |
LIVE — OPERATIONS ACTIVE | NOT READY — BLOCKERS REMAIN
~~~

Use one verdict only and list evidence directly above it.

## 11. analytics.md

~~~markdown
# Trustpilot Analytics

## Baseline timestamp
## Funnel definitions
| Stage | Definition | Source | Owner | Privacy classification |
|---|---|---|---|---|

## Invitation metrics
- Eligible experiences:
- Fair invite coverage:
- Sent/delivered/bounced/opted out:
- Reviews received and conversion:

## Reputation and operations
- TrustScore/star label/review count:
- Review recency/distribution:
- Reply coverage and response time:
- Critical themes and closure:
- Category/market position:

## Referral and conversion
- Profile views if entitled:
- Trustpilot referral sessions:
- Qualified conversions/revenue definition:
- Attribution caveats:

## Reporting cadence and owners
## Data minimization and retention
~~~

Use referrer data or approved tracking allowed by the profile/link surface. Do not assume custom UTMs are
accepted. Test the final public link and keep reviewer/customer identity out of analytics artifacts.
