# Trustpilot Account and Profile Reference

## Contents

1. Source-of-truth hierarchy
2. Profile model and mode decisions
3. Signup and claim flow
4. Duplicate, access, correction, and merge handling
5. Public profile field inventory
6. Category and location rules
7. Asset and copy standards
8. Final profile QA

## 1. Source-of-truth hierarchy

Use sources in this order:

1. The live Trustpilot Business form and the user's signed-in Business account
2. Trustpilot's current legal Guidelines for Businesses
3. Trustpilot Help Center articles and current Business pricing/features pages
4. The public Trustpilot profile/category pages
5. The business's canonical website, legal pages, and product UI
6. User confirmation for private facts

Record URLs and verification dates. Treat old screenshots and help articles as orientation only when the live
surface differs. Never turn a search snippet into a confirmed field value.

Useful official entry points:

- Signup: `https://business.trustpilot.com/signup`
- Current pricing: `https://business.trustpilot.com/pricing`
- Business guidelines: `https://legal.trustpilot.com/for-reviewers/guidelines-for-businesses`
- Public categories: `https://www.trustpilot.com/categories`
- Public profile overview: `https://trustpilot.zendesk.com/hc/en-us/articles/360013930439-Your-business-profile-page`
- Profile customization: `https://trustpilot.zendesk.com/hc/en-us/articles/202616716-Customize-your-business-profile`

## 2. Profile model and mode decisions

A Trustpilot profile is anchored to a business/domain, not a plan or feature. A consumer review can cause a
profile to exist before the business claims it. Search first.

Use the product brand's domain when it is the public seller/service the customer experienced. Use the parent
company when products do not have distinct customer relationships/domains. Document the decision; do not split
reviews merely for better presentation.

Modes:

- `NEW`: no matching page; start the business-account flow
- `CLAIM`: matching unclaimed page; follow the claim route
- `REQUEST ACCESS`: claimed page but authorized user lacks access
- `CORRECT`: material facts are wrong
- `MERGE`: multiple profiles may qualify for consolidation
- `OPTIMIZE`: accurate claimed profile needs completion
- `GROW`: profile is complete and requires sustainable review operations

## 3. Signup and claim flow

The live signup observed on July 23, 2026 presents:

1. Business details
2. Additional details
3. Personal details
4. Activate account

Observed Business details fields:

- Business location
- Business name
- Business website

The business name may be assisted by Dun & Bradstreet. Match the real entity; do not select a similarly named
company. If no exact result exists, follow the live correction/manual-entry route.

Observed Personal details fields:

- First name
- Last name
- Phone number with a country-code selector, such as `+971` for UAE

Capture Additional details from the live session because questions may vary by country/business. Let the user
enter contact details and complete activation directly. Never save passwords, one-time codes, private activation
links, or sensitive identity evidence in `.ulpi/launch`.

For every field record:

| Field | Required | Value/status | Evidence | Verified |
|---|---:|---|---|---|
| Exact live label | Yes/No | `READY TO PASTE`, `SELECT`, `ENTER DIRECTLY`, or `BLOCKED` | Source | ISO date |

Reproduce every live character/file limit and count the prepared value deterministically. Do not assume limits
from a different marketplace.

## 4. Duplicate, access, correction, and merge handling

Search:

- domain with/without `www`, protocol, and localized country domain
- official, trading, former, and product names
- old/rebranded domains
- spelling, spacing, punctuation, and legal-suffix variants

Compare the candidate page's linked site, category, country, locations, review subjects, and Company activity.

If unclaimed, claim it. If claimed, use the official access/support route and provide minimum ownership proof.
If wrong, request a factual correction with evidence. If multiple profiles represent eligible identical domains,
a rebrand, merger, or another supported case, request Trustpilot review for merging. Do not assume all pages can
be merged. Merged reviews can recalculate the main profile's TrustScore.

Never create a replacement profile to avoid reviews. Trustpilot generally does not delete a profile after a
business has been reviewed because the reviewer owns the content, subject to guideline enforcement.

## 5. Public profile field inventory

Inspect `Settings > Public profile settings > Profile page` and record current plan availability. Common public
elements include:

- business name and domain
- logo and header image
- TrustScore/star label and review count
- Company activity information
- company description
- categories
- service/customer-service highlights
- truthful customer guarantees
- website and contact information
- promotion banner
- locations/branches
- reviews, reply/flagging activity, and related/similar businesses

Some customization is plan-gated. Never present header, promotions, competitor-display control, colors, custom
HTML, widgets, or similar features as available until the live account confirms entitlement.

The public profile may dynamically show sections based on review count or behavior. For example, Trustpilot has
documented a highlighted-review section after more than 20 reviews. Treat such display logic as platform-owned,
not a promised outcome.

## 6. Category and location rules

Choose categories by what the business actually sells and what customers evaluate. The official customization
guidance has described one primary category and up to five additional categories, but verify the live limit.

For each category, store:

- exact label and public category URL
- country/market context
- offer evidence and buyer intent
- closest five organic profiles
- pass/borderline/fail decision

Trustpilot may make or revise the final category classification. Do not use irrelevant categories for exposure.

Use locations only for real, active branches or stores. Confirm name, address, contact, hours, URL, ownership,
and whether location reviews are operationally supported. Do not create virtual locations to expand reach.

## 7. Asset and copy standards

Business name must match customer-facing branding. The description should state:

1. what the business/product is
2. who it is for
3. the primary job or outcome
4. specific current capabilities/service scope
5. a credible differentiator or reassurance

Avoid keyword stuffing, unverifiable leadership claims, ratings claims, guarantees not backed by policy, review
quotes copied without rights, and contact details duplicated into prose. Keep public details consistent with the
canonical website.

For every image record source, dimensions, file type/size, crop, rights, owner, and review date. Use sharp,
current brand assets. Remove customer PII, test tenants, internal paths, secrets, and unreleased features.

## 8. Final profile QA

- Correct profile and domain, with no unresolved duplicate
- Authorized owner and activation complete
- Claimed state visible
- Name/domain/logo/category/details consistent with canonical site
- Contacts and locations tested
- Description factual, specific, readable, and benchmark-informed
- Services and guarantees backed by public policy
- No stale promotion
- Desktop and mobile preview checked
- Plan-gated features labeled correctly
- Public link captured after publish
- Baseline TrustScore, review count, category position, and date recorded without promises
