# Trustpilot Benchmarking and Profile Copy

## Contents

1. Mandatory browse gate
2. Category and comparison-set selection
3. Top-five capture schema
4. Evidence and interpretation rules
5. Profile copy workflow
6. Category evidence workflow
7. Benchmark deliverable
8. Listing-derived content requirements

## 1. Mandatory browse gate

The final category and profile-copy recommendation requires `$browse` research against the current rendered
Trustpilot site. Start with `browse --version` and keep one persistent session.

Recommended sequence:

~~~bash
browse --session trustpilot goto "https://www.trustpilot.com/categories/<category-slug>"
browse --session trustpilot wait --load networkidle
browse --session trustpilot snapshot -i
browse --session trustpilot text
browse --session trustpilot links
~~~

Open each selected public profile and its canonical vendor site in the same session. A categories index can be
blocked while a direct category slug works, so try the exact category URL discovered through the public site.

Do not substitute generic web-search snippets for the five rendered profiles. If access remains blocked, stop
the final recommendation and request a safe user-assisted handoff. Record `BLOCKED — LIVE TOP-FIVE BROWSE
REQUIRED`. Do not use stealth or evade access controls without explicit permission and applicable policy.

## 2. Category and comparison-set selection

Start from one sentence:

> Customers choose this business/product to [primary job] in [market/context].

Select the narrowest accurate Trustpilot category. Use the relevant country/market because category ordering and
availability can differ. Record the active URL, filters, visible ordering, and timestamp.

Choose exactly five organic profiles that are:

- visible leaders in the relevant category/order, or
- the closest realistic alternatives when the visible category leaders serve materially different buyers

Explain the method. Separate promoted/sponsored entries from the organic set. Do not quietly choose only weak
profiles. If fewer than five relevant profiles exist, record the shortage and use the nearest defensible peers
with a clear limitation.

## 3. Top-five capture schema

For each profile capture:

| Dimension | What to record |
|---|---|
| Identity | Business name, profile URL, domain, country, claimed/unclaimed |
| Placement | Visible position, order/filter, sponsored status |
| Reputation | TrustScore, star label, review count, distribution/recency if visible |
| Activity | Review sources/labels, reply behavior, flagging/merge signals |
| Taxonomy | Primary and additional categories |
| Profile | Logo/header, description, services, guarantees, contacts, locations, promotion |
| Responses | Coverage, tone, specificity, public/private resolution path, apparent SLA |
| Review themes | Repeated buyer praise, objections, and service failures in paraphrase only |
| Vendor site | Positioning, proof, pricing/CTA, consistency, trust placement |
| Opportunity | Table stakes, credible whitespace, claim to avoid |

Never store reviewer usernames, avatars, order references, contact information, or verbatim review bodies. Use
aggregate/paraphrased themes only.

## 4. Evidence and interpretation rules

TrustScore and category order are observations at a timestamp, not permanent achievements. Do not infer cause
from correlation. A paid plan, profile design, reply rate, review volume, or invitation source must not be
described as causing organic ranking unless Trustpilot explicitly documents that relationship.

Distinguish:

- public fact: directly visible on Trustpilot/vendor site
- business claim: present on the profile/site but not independently verified
- inference: analyst interpretation, labeled as such
- plan feature: available only when the live pricing/account confirms it

Do not reuse competitor wording, logos, reviews, screenshots, or proprietary internal benchmark data.

## 5. Profile copy workflow

Create three original options:

1. Buyer-job led: who, job, and product/service immediately
2. Differentiation led: specific defensible mechanism or fit
3. Trust/reassurance led: scope, support, guarantees, or transparency that reduces risk

Each option should answer:

- What is it?
- Who is it for?
- What experience will reviewers be evaluating?
- Which specific current capabilities or service qualities matter?
- Why should a buyer trust the claim?

Score 1–5 on truth, clarity, category fit, specificity, differentiation, objection handling, scanability, and
site consistency. Reject any version with unsupported superlatives, results, customer counts, review statistics,
security/compliance claims, guarantees, or competitor comparisons.

Count characters against the current visible limit. If no limit appears, do not invent one. Keep a complete
version plus a shorter fallback only when the live form needs it.

## 6. Category evidence workflow

For each category, write:

~~~text
Category:
Public URL:
Country/market:
What buyers expect:
Native offering evidence:
Closest peers:
Why this is/is not the primary category:
Verdict: PASS | BORDERLINE — TRUSTPILOT REVIEW | FAIL
Verified:
~~~

Do not choose categories solely because a competitor uses them. A competitor category is a hypothesis; the
business's real offer is the proof. Keep secondary categories limited to meaningful customer intent.

## 7. Benchmark deliverable

`BENCHMARK.md` must include:

- run timestamp/timezone, locale/country, category, URL, filters/order, and browse session method
- selection methodology and sponsored-placement treatment
- exactly five comparison rows with source links
- table stakes buyers expect
- repeated/overused claims to avoid
- credible positioning whitespace grounded in the product
- profile completeness patterns
- response and recovery patterns
- category recommendation and uncertainty
- three copy options, scores, and one recommended version
- limitations and next refresh date

The benchmark is stale after a material category redesign, competitor change, rebrand, or 90 days. Refresh it
immediately before major copy/category decisions even when less than 90 days old.

## 8. Listing-derived content requirements

Do not infer the listing contract from Trustpilot help text alone. Read the five live profiles and compare the
rendered `Summary`, `About`, `Reviews`, `Company details`, `Contact info`, and Company activity areas.

The July 23, 2026 Software Company sample (Jersey Watch, Unlockerplus, SiteGround, LifeLock, and SquadLocker)
showed this recurring public surface:

| Surface | Observed content | Control class |
|---|---|---|
| Header | Logo, business name, domain, claimed date, subscription label, website/review CTAs | Mixed |
| Reputation | TrustScore, star label, review count, last-12-month volume, rating distribution | Trustpilot-generated |
| Taxonomy | Breadcrumbs, category assignments, category positions | Mixed/generated |
| Summary | AI review summary, recurring topics, representative-review cards | Trustpilot-generated |
| Company details | Business-authored or externally sourced overview | Business/external |
| Rich profile | Additional "Why" message, images, feature/service bullets, service links, support or sales CTA | Often plan-gated |
| Contact | Country/address, phone, email, website as applicable | Business-controlled |
| Activity | Invitation statement, negative-review reply rate/time, AI-reply disclosure, merge history | Generated from operations |
| Reviews | Verified/invited/unprompted labels, responses, filters, topics | User/platform plus business replies |

The five profiles also showed that a minimal listing can contain a short overview plus contact details, while a
richer paid profile may add branded images, a second buyer-facing message, service links, guarantees/benefits,
support/sales CTAs, and structured bullets. Do not assume rich fields are free or available.

Create `CONTENT-REQUIREMENTS.md` with:

| Element | Live evidence across five | Class | Applicable | Exact input needed | Constraint | Buyer question | Owner | Status |
|---|---|---|---:|---|---|---|---|---|

Required evaluation rows:

- business name, canonical domain, logo, location/country, and public website CTA
- primary/additional categories and category-market evidence
- company description/About content
- specific products/services/capabilities and audience/use cases
- truthful benefits, proof, guarantees, and customer-support expectations
- address, phone, email, hours, locations, and support/sales links when applicable
- header/rich images, service links, promotion, and custom CTA with entitlement
- invitation-source statement, reply coverage/time, merge state, and response owner
- generated score, distribution, summary/topics, ranking, and review labels as non-editable outcomes

Use the category-specific five, not this generic sample, for the actual launch. The sample defines the method,
not the user's final requirements.
