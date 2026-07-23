# Stellar G2 profile playbook

Verified against official G2 sources on 2026-07-23. Field availability can vary by plan and G2 release.

## Contents

- Profile strategy
- Product identity and URLs
- Live category benchmark
- Conversion-description workflow
- Core overview
- Visual asset contract
- Packages and pricing
- Features and integrations
- Other profile dimensions
- Conversion QA
- Official sources

## Profile strategy

Build the G2 profile for a buyer comparing products inside a category. A strong profile answers:

1. Is this designed for a company like mine?
2. Does it solve my exact problem?
3. Does it meet the category's expected capabilities?
4. What is different from alternatives?
5. What will it cost and how fast can I evaluate it?
6. Can I trust the vendor, implementation path, and customer experience?

Use unique, category-relevant copy. Do not paste a generic homepage description.

## Product identity and URLs

- Use the exact official product name.
- Use the product's canonical landing page, not the holding-company homepage.
- Use the official vendor domain and current support/documentation links.
- Add consistent UTMs in my.G2. G2 appends its own content parameter based on the source profile page.
- Route each CTA to the most relevant destination: trial, demo, pricing, docs, or contact.
- Verify every URL on desktop and mobile and without an existing login session.

Suggested base convention:

| Field | Value |
|---|---|
| utm_source | g2 |
| utm_medium | software-review-profile |
| utm_campaign | g2-profile |

Preserve an existing organization-wide convention if one already exists.

## Live category benchmark

Use $browse after the main category and target segment are known:

1. Open the current G2 category page and wait for rendered state.
2. Record category, segment, sort order, date, and sponsored placements.
3. Inspect the first five to eight organic profiles under the default G2 Score view.
4. Add one high-satisfaction challenger when it exposes a different positioning strategy.
5. Inspect overview, pricing, screenshots/video, features, CTA, and recent review themes.
6. Save URLs and concise factual observations to BENCHMARK.md.

For each product capture:

| Dimension | Question |
|---|---|
| Category framing | What category words establish relevance immediately? |
| Buyer | Which company segment, role, or workflow is explicit? |
| Problem/outcome | What costly problem and desired result lead the copy? |
| Differentiation | Which claims are specific and which are generic category table stakes? |
| Proof | What verifiable evidence supports trust? |
| Buying path | Is pricing, trial, demo, or implementation clear? |
| Media | What does the first visual prove? |
| Review themes | Which buyer concerns recur across recent reviews? |

Do not copy wording, mimic unverifiable claims, or treat a competitor's review as proof about the user's
product. Use the benchmark to find buyer expectations, saturated messages, and credible whitespace.

## Conversion-description workflow

Draft two assets:

1. Description of Product for the initial submission form—concise and factual within the current live limit.
2. What is Product overview for the claimed profile—normally 120–220 words and never above 500 words under
   the current profile limit.

For each asset create three options:

- Category-led
- Outcome-led
- Differentiation-led

Use this structure:

1. First sentence: category, ideal buyer, and primary value.
2. Buyer problem: specific operational pain or risk.
3. Product mechanism: two to four native capabilities that solve it.
4. Differentiated proof: defensible contrast, time-to-value, result, or implementation fact.
5. Buying next step: clear trial, demo, pricing, or contact path.

Score every option from 1–5:

| Criterion | Test |
|---|---|
| Truth | Every claim is supported by product evidence |
| Clarity | A buyer understands it on one read |
| Category fit | It naturally uses the category's buyer language |
| Differentiation | It avoids generic claims common across the benchmark |
| Proof | It includes concrete, verifiable support |
| Conversion | It makes the next step obvious |

Recommend the highest-scoring option, explain the choice in one sentence, and make that version the final
READY TO PASTE value in SUBMISSION.md and PROFILE.md. Never use keyword stuffing or competitor names merely
to attract comparison traffic.

## Core overview

G2 currently allows up to 500 words in the What is Product section. Aim for 120–220 words unless the product
needs more context:

1. Plain category and ideal customer.
2. Costly problem or workflow.
3. How the product solves it.
4. Three to five native differentiators with proof.
5. Deployment, time-to-value, or support signal.
6. Clear next action.

Avoid:

- unverifiable superlatives
- keyword stuffing
- invented market leadership
- vague AI claims
- feature dumps without outcomes
- competitor attacks
- claims that conflict with pricing or documentation

## Visual asset contract

The initial Add your product form and the claimed my.G2 profile expose different asset controls. For initial
submission, the live form recommends SVG for the uploaded logo and accepts a file or web URL. After claiming,
follow the current my.G2 field-specific formats below.

### Profile logo

- Product-specific JPG, PNG, or GIF.
- At least 400 pixels.
- Use adequate whitespace and test at small sizes.

### Grid logo

- SVG smaller than 5 MB.
- Prefer an image mark rather than text because it renders small.

### Profile banner

- JPG, PNG, or GIF smaller than 5 MB.
- Preferred dimensions: 1260 × 240 pixels.
- If rendering is poor, G2 recommends 2500 × 476 pixels at a minimum of 72 PPI.
- Communicate one buyer outcome, one product visual, and restrained branding.
- Keep important content away from edges and test the public render.

### Banner video

G2 currently supports Vimeo, Vidyard, Wistia, and YouTube Universal Links. Use a short product walkthrough:

1. buyer problem
2. actual UI and core workflow
3. differentiated outcome
4. realistic proof
5. next step

### Screenshots and multimedia

- Use current production UI, readable at G2's displayed size.
- Show one workflow or proof point per image.
- Add clear captions tied to buyer outcomes.
- Remove customer PII, secrets, internal environments, and misleading sample data.
- Order assets from core value to setup, differentiated workflows, analytics, and administration.
- Verify live file-type, size, count, and dimension rules in my.G2 before upload.

## Packages and pricing

Complete pricing even when sales-assisted:

- edition/package name
- concise edition description
- price or custom-quote state
- currency
- billing cadence
- billing unit such as user, seat, workspace, or usage
- number of units included
- trial or free-plan details
- package CTA
- up to 12 truthful package-specific features under G2's current limit

Standardize package structure so buyers can compare editions. Match the canonical pricing page exactly. If
pricing is custom, explain what controls price and what the buyer should prepare before requesting a quote.

## Feature data

Select category-specific features truthfully:

- Native — product supplies the capability itself.
- Third Party — capability is available through an integration or external application.
- Not Available — product does not currently supply it.

Feature selections drive reviewer questions. G2 currently requires at least ten responses to feature-related
questions before the public Features tab appears. Do not mark roadmap features as available.

## Integrations

G2 can infer integrations from approved review responses and refresh the data periodically. Some plans allow
direct integration-list editing. For each integration record:

- integration product name
- native/partner/connector method
- supported workflows and objects
- setup requirements
- public documentation
- maintenance owner

Never list an integration that is only planned, customer-specific, or unsupported.

## Other profile dimensions

Complete every available relevant field:

- hosted/cloud, on-premises, or both
- supported languages
- company and product details
- values and ethics information
- target markets and category attributes
- security, privacy, compliance, and support facts
- AI disclosure/trust fields only when the product genuinely qualifies
- trial, demo, implementation, and support paths

The All-in-One or Best-of-Breed classification is algorithmic, currently applies at 25+ reviews, and does not
affect G2 Score. Do not claim or force it in profile copy.

## Conversion QA

Before publishing:

- Read every field as a skeptical buyer in the selected main category.
- Check copy against current product docs and pricing.
- Test every CTA with UTMs.
- Confirm screenshots are legible and ordered.
- Confirm the first asset and first paragraph communicate the same promise.
- Confirm free-versus-paid G2 capabilities and do not promise unavailable plan features.
- Confirm mobile rendering.
- Assign a field owner and a last-verified date.

## Official sources

- [Product Information](https://documentation.g2.com/g2/docs/product-information/)
- [Packages and Pricing](https://documentation.g2.com/docs/packages-pricing)
- [Features](https://documentation.g2.com/docs/features)
- [Get started with G2](https://documentation.g2.com/docs/get-started-with-g2)
- [G2 integrations overview](https://documentation.g2.com/docs/integrations)
