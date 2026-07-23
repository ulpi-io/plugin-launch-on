# Capterra Profile and Category Playbook

Use this reference to turn product truth and live category research into a clear, policy-compliant profile.

## Contents

- Browse research protocol
- Category evidence
- Description rules
- Description workflow
- Profile field coverage
- Logo, screenshots, and video
- Integrations and product details
- Target market and pricing
- Quality scorecard

## Browse research protocol

`$browse` is required. Start with `browse --version`, use one persistent session, and follow the browse skill:

1. `browse goto <category-url>`
2. `browse wait --network-idle`
3. `browse snapshot -i` to see controls, cards, sponsorship labels, and stable refs
4. Use `text` and `links` for concise rendered evidence
5. Refresh the snapshot after navigation or DOM changes
6. Open the top five selected product profiles in the same session
7. Open each vendor-owned site to validate current positioning and public facts
8. Save only minimal evidence needed for the benchmark

Do not use a raw HTTP scraper, bulk crawler, evasion, or CAPTCHA bypass. If a CAPTCHA, MFA, login, or bot
control blocks research, use the browse skill's approved human handoff. Never invent a result.

## Selecting the top five

Record the category URL, category name, date/time zone, region, visible sort, filters, and result order.
Capterra may place sponsored profiles first. Build two lists when relevant:

- Sponsored — visible sponsored cards, recorded for context but not called organic leaders
- Top five organic — first five non-sponsored profiles in the active sort

If the page does not expose a sponsorship label or sort state, say `NOT VISIBLE` rather than infer. If the
category is too broad, choose a buyer-relevant filter first and record it. Do not cherry-pick five products
that support a predetermined narrative.

For each product capture:

- profile and canonical vendor URLs
- visible position and sponsored state
- target buyer and category framing
- short-description structure and overview structure
- named capabilities and differentiators
- pricing, trial, and free-version visibility
- screenshots/video approach
- integrations highlighted
- target market, support, training, and deployment signals
- CTA and missing buyer questions
- a concise synthesis of review themes only when visible; do not copy full review content

The benchmark is research, not a source of copy. Never imitate phrases or make claims from another product.

## Category evidence

For each proposed category, create this map:

| Requirement or buyer expectation | Native capability | Evidence | Status |
|---|---|---|---|
| Exact category criterion or observed table stake | What the product does today | URL, docs, screenshot, demo | PASS/FAIL |

Rules:

- Native product behavior is evidence; audience aspiration is not.
- Integration-provided behavior is not automatically a native capability.
- A roadmap item is not a current feature.
- Marketing language without product proof is weak evidence.
- All primary-category expectations must pass before recommending that category.
- Choose the narrowest accurate primary category and only defensible secondary categories.

The current submission accepts one initial primary category and requires at least seven supported features
from that category's live feature list. Capterra makes the final placement decision. Additional categories
are a post-publication request, not part of the initial submission.

Create a feature-selection table:

| Exact feature label | Product behavior | Evidence | Plan/limits | Type | Select? |
|---|---|---|---|---|---|

`Type` must be Native, Integration, or API-only. Select features that best describe the actual offering, not
every remotely related feature. If the product cannot truthfully meet the seven-feature minimum, fail the
category and research another one with `$browse`.

## Description rules

Current official Profile Guidelines require:

- unique copy that is a true product overview
- product and service names that match the vendor site
- working destination URLs pointing to the vendor's site
- standard English spelling and grammar
- third-person language using the product or company name

Do not include:

- first-person `we`, `our`, or `us`
- superlatives or over-comparative claims such as best, most, or fastest
- CTAs such as `click here` or `start a free trial`
- phone numbers, emails, URLs, or other personally identifiable information
- company suffixes such as Inc., Corporation, or LLC in the company name
- repeated punctuation, excessive capitalization, line breaks, symbols, special characters, or HTML
- offensive, obscene, or defamatory language

Avoid vague claims such as easy, seamless, powerful, revolutionary, all-in-one, or AI-powered unless the next
sentence specifies exactly what the product does and the claim is verifiable.

## Description workflow

Create three independent options:

### Category-led

Start with `[Product] is [accurate category] for [buyer]`. Name the primary workflow, core capabilities, and
credible differentiation. Use when category clarity is the biggest conversion risk.

### Outcome-led

Start with the concrete job or costly problem. Explain how the product changes that workflow and which native
capabilities make it possible. Use only verifiable outcomes; do not invent percentages or guarantees.

### Differentiation-led

Start with the strongest product-specific mechanism or fit. Contrast against category sameness without naming
or disparaging competitors and without claiming superiority.

For each option produce:

- short description, at most 135 characters
- product overview, 400–1,000 characters
- exact character count for each
- evidence links for every substantive claim
- score from 1–5 on truth, clarity, category relevance, differentiation, buyer usefulness, and compliance

Recommend the highest-scoring version only after the live top-five benchmark is complete. Do not pad the
overview to reach 400 characters. Add decision-useful product information.

## Profile field coverage

Create a field inventory for:

- product and company names
- canonical URL and public CTA
- short description and overview
- core capabilities and use cases
- languages and countries
- support and training
- deployment and devices
- logo, screenshots, and product video
- integrations
- primary and secondary categories
- target roles, industries, company sizes, and regions
- pricing model, starting price, billing unit, frequency, currency, trial, and free version

Each mutable field needs a source, owner, and `last verified` date. Never let repository copy silently replace
the live product truth.

## Logo, screenshots, and video

Observed logo input: PNG, JPG, JPEG, or WebP, less than 5 MB. Use a current, legible, product-specific logo.
Check transparent backgrounds and contrast where practical. Do not use a customer logo without rights.

The current Media page requires one to five screenshots, each with a mandatory caption. Accepted formats are
PNG, WebP, JPEG, and JPG, and every file must be under 5 MB. Screenshots must show the real product interface.
Use screenshots that help a buyer understand the workflow:

1. primary job-to-be-done
2. result or output
3. setup/admin experience
4. reporting or analytics
5. integration or collaboration flow

Remove personal data, secrets, internal URLs, unreleased features, and unrelated browser chrome. Avoid stock
images and marketing slogans. Use current UI and only assets the vendor has rights to submit.

Videos are optional and must be in English, describe the product or service, and use a Vimeo, Wistia, or
YouTube link; the current form marks YouTube preferred. Prefer a short product walkthrough with truthful
narration over a generic brand reel.

## Integrations and product details

For every integration record:

- exact integration name
- direction and data/workflow exchanged
- native, marketplace, API, webhook, or third-party connector status
- availability by plan
- setup requirements
- public evidence URL

Do not list an integration because both products expose APIs. Do not describe a planned connector as live.
The current form also requires a Yes/No answer to `Do you offer an Open API?`; answer from documented,
customer-accessible capability, not internal implementation details.

For languages, countries, support, training, and deployment, use the exact current live form options. Require
proof for native apps and 24/7 human support. Review any AI-fetched prefill against current product truth.

## Target market and pricing

Describe target market as a concrete fit:

- buyer roles and end users
- company sizes actually supported
- industries with real product fit or customers
- countries and languages genuinely available
- use cases and deployment constraints

The current Target Market page requires a description capped at 200 characters, industries, company size, and
number of users. Count the description exactly, including spaces and punctuation, and show `N/200`. Use the
exact live option labels. For each selected item keep a concise reason and evidence source, then ask the user
to confirm the final set because served-client truth may not be public.

Avoid saying `businesses of all sizes` unless product, onboarding, pricing, permissions, security, and support
really cover each segment.

Pricing must match the public pricing page or a user-confirmed sales model. Capture:

- free or paid model
- starting amount and currency
- billing unit and period
- minimum seats/commitment
- free trial and duration
- free version and limits
- contact-sales conditions
- plan names and current verification date

The current pricing workflow permits at most six plans. For each one, keep plan name, description, amount,
currency, unit, billing period, billing cadence, minimum commitment, and limits together. Inspect the current
`Do you provide these options?` controls with `$browse` and use their exact labels.

Treat AI-fetched pricing as an untrusted draft. Reconcile monthly and annual prices, per-user and flat units,
discounted annual billing, free tiers, and contact-sales conditions against the canonical pricing page before
marking the section ready.

Never fabricate an attractive starting price. If pricing is not public, use the exact live option such as
`Contact vendor for pricing` when available and truthful.

## Quality scorecard

A stellar profile should pass:

| Dimension | Passing standard |
|---|---|
| Truth | Every claim is current and evidenced |
| Category clarity | Buyer understands the category and job immediately |
| Specificity | Copy names real workflows and capabilities |
| Differentiation | Distinction is defensible, not generic hype |
| Buyer usefulness | Pricing, fit, deployment, support, and media answer evaluation questions |
| Compliance | Copy and assets follow current guidelines |
| Completeness | Every applicable field is populated accurately |
| Consistency | Site, profile, pricing, and integrations agree |
| Conversion | Canonical destination and next step are clear outside the description |
| Maintainability | Owners, evidence, and verification dates are recorded |
