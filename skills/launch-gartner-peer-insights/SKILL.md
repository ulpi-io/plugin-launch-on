---
name: launch-gartner-peer-insights
description: |
  Qualify, request, build, and operate a Gartner Peer Insights vendor and product listing. Covers enterprise
  eligibility, market-capability mapping, suite-level naming, duplicates and acquisitions, Vendor Portal fields,
  mandatory live market and top-five product research with $browse and $browse-stealth fallback, Gartner-safe
  third-person profile copy, pricing and screenshots, compliant review sourcing, Customers' Choice and Voice of
  the Customer readiness, analytics, and maintenance. Writes a paste-ready package under
  .ulpi/launch/gartner-peer-insights. Use when a technology vendor wants to list or improve an enterprise product.
---

<HUMAN-WRITING-RULES>
For every user-facing prose artifact produced by this skill, run the full embedded-mode process in `../../references/human-writing.md` before finalizing. Its no-fabrication rule and all 33 pattern checks are mandatory; preserve the intended platform voice and do not alter code, structured data, link targets, quotations, titles, or proper names.
</HUMAN-WRITING-RULES>

<EXTREMELY-IMPORTANT>
Blocking rules:

1. ENTERPRISE ELIGIBILITY FIRST. The product must be sold to mid-to-large enterprise clients. Gartner Peer
   Insights excludes small-business-only and consumer IT solutions.
2. PASS THE MARKET TEST. Meet every mandatory capability and at least 50% of the other published capabilities
   for the selected active market. Map each capability to public first-party evidence. Gartner decides fit.
3. LIST THE OWNED SELLABLE SUITE. Only the owning vendor may list. No reseller, integrator, or partner page.
   List the independently sellable suite/highest service level, not modules/components. Mark beta and legacy
   exactly as Gartner requires.
4. SEARCH BEFORE REQUESTING. Resolve duplicates, prior names, acquisitions/divestitures, legacy products, and
   existing access. Do not create a new listing to avoid reviews/history.
5. USE $browse AND EXACTLY FIVE. Inspect the live market, exactly five relevant leading product listings, their
   details/reviews, and vendor sites before final content.
6. USE $browse-stealth ON BLOCK. On 403/challenge, verify Camoufox, stop normal browse, retry headed, stabilize,
   and inspect. If IP reputation still blocks it, require the permitted handoff/proxy; never invent evidence.
7. OBEY PROFILE COPY RULES. English, third person, factual, publicly verifiable, standard grammar, relevant to
   the approved vendor/product. No first person, superlatives, competitor mentions, awards, CTA, links, PII,
   line breaks, special characters, HTML, offensive/defamatory text, or marketing screenshots.
8. REVIEWS MUST BE PERSONAL AND INDEPENDENT. Never fabricate, ghostwrite, gate, alter, pressure, or solicit
   employees of the vendor/competitor or people at exclusive partners, resellers, integrators, or consultants.
9. INCENTIVES ONLY THROUGH GARTNER. The Vendor Portal may offer complimentary Gartner-administered gift cards.
   Never offer an independent incentive. Verify current campaign, cohort, country, value, disclosure, and rules.
10. DO NOT PROMISE CLASSIFICATION, REVIEWS, CUSTOMERS' CHOICE, VOC, OR RESEARCH COVERAGE. Gartner controls all
    editorial decisions. Recheck live rules and persist under `.ulpi/launch/gartner-peer-insights`.
</EXTREMELY-IMPORTANT>

# Launch on Gartner Peer Insights

## Outputs

- `ELIGIBILITY.md` — enterprise, ownership, suite-level, duplicate, and market verdict
- `MARKET-CAPABILITIES.md` — mandatory and other capability evidence with computed coverage
- `SUBMISSION.md` — account/request and every Vendor/Product Profile field in live order
- `BENCHMARK.md` — dated exactly-five live product analysis
- `CONTENT-REQUIREMENTS.md` — benchmark-derived and Gartner-rule-derived field matrix
- `VENDOR-PROFILE.md` — company description and reusable vendor facts
- `PRODUCT-PROFILE.md` — compliant product description, pricing, screenshots, and per-market content
- `REVIEW-PLAN.md` — eligible cohort, Gartner campaign, neutral templates, privacy, and QA
- `VOC-AND-OPERATIONS.md` — freeze periods, awards/VoC, maintenance, escalations, and cadence
- `CHECKLIST.md`, `analytics.md`, and shared `.ulpi/launch/positioning.md`

## Step 0: Identify product and target market

Ask when unclear:

> Which enterprise product are you listing on Gartner Peer Insights? Send its canonical product URL, target
> Gartner market, typical customer size, and any current Gartner Peer Insights product/vendor URLs.

Determine `NEW`, `CLAIM/ACCESS`, `CORRECT`, `RENAME/M&A`, `OPTIMIZE`, or `GROW`. Gather owning vendor, exact
sellable suite, enterprise customer evidence, existing profiles/reviews, target market, product owner, review
owner, public capabilities, pricing, current Vendor Portal access, and timing.

## Step 1: Load references and browse

Read:

- `references/eligibility-market-and-submission.md`
- `references/profile-benchmark-and-copy.md`
- `references/reviews-voc-and-operations.md`
- `references/artifact-templates.md`

Use `$browse` normally first. Gartner returned 403 in normal browse during the July 23, 2026 research run and
loaded in headed Camoufox. Apply `$browse-stealth` exactly on a block. Do not finalize from snippets.

## Step 2: Ground product truth

Browse the official product, capabilities, enterprise customers, pricing/sales, docs, integrations, security,
support, legal, lifecycle/EOL, acquisition/rebrand, and media pages. Record public URL and verified date for
every claim. Reuse shared positioning only when current.

## Step 3: Search profiles and test structural eligibility

Search exact/former vendor and product names, suite/modules, domains, acquisitions, legacy names, and Gartner
vendor/product pages. Confirm:

- owning vendor and authorized contact
- independently sellable suite/highest service level
- real mid-to-large enterprise customers
- public product URL and current sale state
- correct beta, acquisition, divestiture, rebrand, or legacy treatment

Issue `ELIGIBLE — CONTINUE`, `EXISTING — CLAIM/CORRECT`, `RENAME/M&A EVIDENCE REQUIRED`, `LEGACY REVIEW`, or
`INELIGIBLE/BLOCKED`.

## Step 4: Map the market definition

Open the current target market and `How Categories and Markets Are Defined`. Capture exact definition,
mandatory capabilities, other capabilities, transition/retirement status, active/open state, related markets,
and publication/freeze timing. In `MARKET-CAPABILITIES.md`, map every capability to a public product page or
downloadable public datasheet. Pass only if all mandatory rows pass and at least 50% of other rows pass.
Internal documents created for the application do not qualify as contest evidence.

## Step 5: Capture registration and listing request

Use the Technology Provider Tool/Vendor Portal live form. Current official listing guidance requires:

- contact name, job title/role, and email
- company name
- product name
- website URL describing the product
- requested Gartner Peer Insights market
- explanation of how the product provides solutions within that market

Capture all dynamically rendered identity, account, company, product, market, evidence, verification, and
consent fields in exact order. Mark `READY TO PASTE`, `SELECT`, `UPLOAD`, `ENTER DIRECTLY`, or `BLOCKED`, with
visible limits/counts. Never persist password, hCaptcha/MFA, verification codes, or customer lists.

## Step 6: Benchmark exactly five live products

Open the live target market using its default buyer-facing sort; record date/timezone, filters, sort, market
transition, and product count. Inspect exactly five relevant leading products and official sites. Capture:

- product/vendor, displayed order, rating/count, Customers' Choice/other platform labels
- overview and alternatives, market positioning and details
- review distribution/recency, willingness to recommend, company-size/region/industry segments
- integration/deployment and other market dimensions
- description structure, pricing presence, screenshots, company/vendor information
- comparison patterns, table stakes, buyer objections, and credible whitespace

Example only: the July 23, 2026 Employee Recognition and Reward Systems market, sorted `Number of Ratings,
High to Low`, began Vantage Circle, Achievers Platform, Workhuman Social Recognition, Assembly, and Awardco
Platform. Re-run live for the user's actual market. Summarize; never copy reviews or proprietary Gartner content.

## Step 7: Build requirements and compliant profiles

Create `CONTENT-REQUIREMENTS.md` before drafting. Classify `REQUIRED`, `RECOMMENDED`, `GARTNER-GENERATED`,
`PER-MARKET`, or `NOT APPLICABLE`. Then prepare:

- Vendor Profile: company description plus portal fields such as revenue/employees when available
- Product Profile per market: third-person description, pricing, actual product screenshots, and all live fields
- source URL, evidence, owner, live constraint, and verification date for each value

Write three compliant third-person options: enterprise-job, capability/workflow, and deployment/reassurance.
Strip all prohibited content listed in the blocking rules. Product information is completed separately for every
product in every approved market; vendor information is reusable across the vendor's products.

## Step 8: Build compliant review sourcing

Define genuine users with direct personal experience. Exclude vendor/competitor employees and people at
exclusive partners, resellers, system integrators, and consultants. Use a neutral Gartner-generated campaign
link and identical eligibility/timing. Do not supply answers or alter feedback.

Default to Gartner's current Vendor Portal review-sourcing flow. If complimentary gift cards are offered, use
only the Gartner-administered program after verifying current rules. Apply privacy minimization, lawful basis,
opt-out/suppression, frequency caps, and secure deletion. Reviewers must comply with employer confidentiality.

## Step 9: VoC, distinctions, operations, and analytics

Record current Voice of the Customer and Customers' Choice methodology, eligibility windows, market-specific
minimums, review recency, distribution/coverage, freeze period, and licensing. Reviews submitted during a freeze
may roll to the next cycle. Never promise research inclusion.

Maintain quarterly capability/market fit, public evidence, profile copy, pricing/screenshots, lifecycle, names,
reviews, access, privacy, and escalation contacts. Gartner may reclassify/remove products during audits.

Track profile/market referral traffic, campaign invites/starts/completions, approved review volume/recency,
distribution by allowed segments, public rating/willingness-to-recommend, and downstream conversions without
scraping reviewer identities or Gartner content.

## Step 10: Validate

Require all eligibility gates, 100% mandatory and >=50% other capabilities, exact five live profiles, stealth
fallback evidence, every live field, compliant third-person copy, authentic review cohort, privacy, and current
VoC/freeze facts. Final verdict: `READY TO REQUEST LISTING`, `READY TO PUBLISH PROFILE`,
`READY TO SOURCE REVIEWS`, `LIVE — OPERATIONS ACTIVE`, or `NOT READY — BLOCKERS REMAIN`.

Never submit, publish, source reviews, or contact Gartner/customers without explicit user approval.
