# Capterra Eligibility and Submission Reference

Use this reference before preparing or submitting a Capterra listing. The live form and current official
guidelines remain the final source of truth.

## Contents

- Eligibility gate
- Duplicate and ownership gate
- Account setup
- Initial listing request
- Product Listing Request sections
- Product Details fields
- Sensitive-data handling
- Submission and approval states

## Eligibility gate

The self-service entry screen observed July 23, 2026 requires the submitter to confirm all three statements:

1. `I am submitting a B2B or B2C software product, not a service or consulting offer.`
2. `My product is an off-the-shelf software, not a custom built solution.`
3. `I am a direct representative of the software vendor, not a reseller.`

Treat each as an independent PASS/FAIL gate. Link evidence for the product type and public offer; require the
user to confirm their relationship. Never check an inaccurate statement.

Capterra's broader Profile Guidelines currently say eligible profiles may include B2B or B2C products or
services and that an authorized reseller can sometimes create a listing. That broader policy does not make a
false self-service attestation acceptable. Ask Capterra support which route applies when the offer is an
eligible service or the submitter is an authorized reseller.

Additional profile criteria:

- The offer is packaged, pre-built, and publicly available.
- It fits at least one existing Capterra category at Capterra's discretion.
- The public site has a trial, demo, purchase, or request-information CTA.
- The only public CTA is not a waitlist or equivalent.
- Product name on the submission matches the vendor's site.
- Destination URLs work and point to the vendor's site.

Current exclusions include marketplaces or database websites, personal productivity solutions, product
clones, personal apps, and custom-made/bespoke software. When fit is ambiguous, use `SUPPORT REVIEW REQUIRED`.

For beta products, do not assume acceptance. Confirm the product is usable, publicly offered, backed by a
working site and CTA, and able to earn at least one authentic review during its first calendar year. Verify
the current beta language in the live rules before relying on it.

## Duplicate and ownership gate

Before creating anything, use `$browse` to search Capterra for:

- official product name
- vendor name
- former product and company names
- common abbreviations and spelling variants
- canonical domain

Record query, date, and result URLs. If a matching profile exists:

- do not submit another profile
- record whether it is claimed
- compare name, vendor, URL, category, copy, pricing, integrations, and status
- use the claim or correction route
- document any duplicate or ownership dispute for support

Do not assume a profile is absent because one query returned no result. Search Capterra and a normal search
engine using the domain and product name.

## Account setup

The account completion screen observed July 23, 2026 shows:

| Field | Handling |
|---|---|
| Company/product name | Confirm prefilled value; use the current official name |
| Website | Confirm canonical public product URL |
| Select Company Size | User-confirmed; never infer from vague marketing copy |
| Country | User-confirmed company/account country |
| Enter First Name | `PRIVATE — ENTER DIRECTLY` |
| Enter Last Name | `PRIVATE — ENTER DIRECTLY` |
| Select Department | User-confirmed submitter department |
| Select Job Level | User-confirmed submitter level |
| Business Phone country code | `PRIVATE — ENTER DIRECTLY` |
| Enter Phone Number | `PRIVATE — ENTER DIRECTLY` |
| Select Time Zone | User-confirmed operating time zone |
| New Password | `SECRET — ENTER DIRECTLY WITH PASSWORD MANAGER` |
| Verify New Password | `SECRET — ENTER DIRECTLY WITH PASSWORD MANAGER` |

Never ask the user to paste passwords into chat or Markdown. Do not store phone numbers, personal email
addresses, or names unless the user explicitly wants them persisted and understands the repository exposure.

## Initial listing request

The first request screen observed July 23, 2026 contains:

| Field | Required | Output rule |
|---|:---:|---|
| Business Email | Yes | `PRIVATE — ENTER DIRECTLY`; must be a real business address |
| Product Name | Yes | Official product name, matching the product site |
| Product Website | Yes | Canonical public product or pricing URL |
| Contact me about brand building and lead generation | No | Default unchecked; user decides marketing consent |
| Privacy policy acceptance | On submit | Link current policy and require user review |

Do not opt the user into marketing by default. Do not claim to accept a privacy policy or other terms for the
user unless they explicitly authorize the action after review.

## Product Listing Request sections

The visible workflow order is:

1. Product description
2. Product details
3. Media
4. Integrations
5. Category
6. Target market
7. Product pricing
8. Submit for review

The interface says submission becomes available only after all mandatory fields are complete. For each page,
capture exact field labels, required markers, UI help, option values, limits, and any AI-generated prefill.
The form can change; the current render outranks this reference.

## Product description

Observed requirements:

- English content
- clear, high-level overview of core capabilities
- product logo: PNG, JPG, JPEG, or WebP under 5 MB
- short description: maximum 135 characters
- overview: minimum 400 and maximum 1,000 characters

Count characters including spaces and punctuation. Validate using the same Unicode string that will be pasted.
See `profile-and-category-playbook.md` for copy rules.

## Product Details fields

Observed July 23, 2026:

### Which languages is your product available in?

- Required multi-select
- UI showed 47 available options
- Select only languages with a real localized product experience or supported language offering
- Do not treat a browser's automatic translation as product availability

### Which countries is your product available in?

- Required multi-select
- UI showed 88 available options
- Select where the product is actually sold/supported and legally available
- Do not equate website reach with supported availability

### Support Options

Visible options:

- Email/Help Desk
- FAQs/Forum
- Knowledge Base
- Phone Support
- 24/7 (Live Rep)
- Chat

Select only operated channels. `24/7 (Live Rep)` requires real round-the-clock human availability, not an
automated bot or an unanswered inbox.

### Training Options

Visible options:

- In Person
- Live Online
- Webinars
- Documentation
- Videos

Select only training customers can currently access. A marketing demo does not automatically count as
training.

### Deployment Options

Visible values:

- Web: Cloud, SaaS, Web-based
- Desktop: Mac, Windows, Linux, Chromebook
- On-Premise: Windows, Linux
- Mobile: Android, iPhone, iPad

Differentiate native application support from access through a web browser. A responsive website does not
prove native Android, iPhone, iPad, Mac, Windows, Linux, or Chromebook deployment. Require a store link,
download page, documentation, or product proof for each checked platform.

The page warns that information may be fetched from the website with AI. Review every preselected value.
Treat AI prefill as a draft, not evidence.

## Media fields

The Media page observed July 23, 2026 requires at least one screenshot and permits at most five.

Screenshot contract:

- Supported formats: PNG, WebP, JPEG, or JPG
- Each file must be less than 5 MB
- Each screenshot must include a mandatory caption describing its content
- Use a real product interface, not stock imagery or a marketing slide

Record the local asset path, file format, byte size, dimensions, current UI version, caption, rights owner,
and privacy review for each screenshot. Remove secrets, PII, customer data, internal-only domains, and
unreleased features.

Video is optional. The visible form accepts Vimeo, Wistia, and YouTube URLs and marks YouTube as preferred.
The official profile rules require an English video about the product. Verify the URL is public and playable.

## Integrations fields

The Integrations page observed July 23, 2026 contains:

- `Do you offer an Open API?` — required Yes/No radio group
- `Add Integrations` — searchable selector
- `Added Integrations` — selected integration chips

Answer Open API `Yes` only when a public or customer-accessible documented API exists. Internal endpoints or
future plans do not qualify. For every added integration, record evidence, direction, availability, setup,
and plan restrictions. Review AI-fetched or preselected integrations rather than accepting them automatically.

## Category fields

The Category page observed July 23, 2026 says:

- Select the product's primary category and features.
- The product is initially listed in one category.
- Additional relevant categories can be requested after publication.
- Capterra's team makes the final category placement decision.
- Select at least seven features that best describe the product offering.

Do not treat the selected category as approved until Capterra confirms placement. Build the initial submission
around one strongest category. Keep secondary-category evidence ready for a post-publication request.

For the `Employee Recognition` category, the observed form displayed 37 options:

1. eCards
2. Reminders
3. Social Recognition
4. Customizable Branding
5. Alerts/Notifications
6. Chat/Messaging
7. Recognition Tracking
8. Engagement Tracking
9. Gamification
10. Peer-to-Peer Recognition
11. Rewards Catalog
12. Customizable Reports
13. Nominations
14. Employee Profiles
15. Single Sign On
16. Manager-to-Employee Recognition
17. API
18. Surveys & Feedback
19. Goal Management
20. Employee Reward Programs
21. Third-Party Integrations
22. Commenting/Notes
23. Budget Control
24. Mobile Access
25. Multi-Language
26. Awards Management
27. AI/Machine Learning
28. Workflow Automation
29. Leaderboards
30. Reporting/Analytics
31. 360 Degree Feedback
32. Customizable Dashboard
33. Customizable Templates
34. Incentive Management
35. Ongoing Performance Tracking
36. Generative AI
37. AI Copilot

Feature options are category-specific and may change. When the selected category is not Employee Recognition,
use `$browse` to capture its current exact list rather than reusing these options.

For every selected feature record:

- exact form label
- current product behavior
- public documentation, screenshot, demo, or repository evidence
- availability by plan
- whether it is native, integration-provided, or API-only
- PASS/FAIL and last-verified date

Select at least seven only when seven or more genuinely pass. Do not use roadmap items, loose synonyms,
integration-provided behavior presented as native, or unverified AI claims to satisfy the minimum.

## Target Market fields

The Target Market page observed July 23, 2026 asks the vendor to specify the clients served, focusing on
industry and roles. Its visible mandatory controls are:

- Target Market description — maximum 200 characters
- `Add industries` — target industries; required
- `Target Company Size` — selection required
- `Target Number of Users` — selection required

The exact selectable values were not visible in the supplied screen. Use `$browse` on the live form to record
the option labels before producing paste-ready selections. Do not invent bands or normalize the platform's
wording.

Build the recommendation from:

- customer industries and active use cases
- product permissions, administration, onboarding, and reporting depth
- pricing minimums and sales motion
- security, compliance, procurement, support, and service capacity
- proven deployment sizes and documented technical limits
- the intended buyer roles and actual end-user population

For each selection record `evidence`, `reason`, and `user confirmation`. Website positioning can support a
recommendation, but it does not prove the vendor currently serves every claimed segment. Avoid selecting all
industries or all company/user sizes to maximize exposure; broad targeting weakens buyer fit and can make the
profile inaccurate.

Count the Target Market description deterministically; do not estimate by eye. Count spaces and punctuation,
rewrite anything above 200 characters, and label the final value `READY TO PASTE — N/200`.

Verified example for Team Toast, 179 characters:

~~~text
Team Toast serves HR and People teams at growing organizations seeking employee recognition, feedback, surveys, and engagement tools within Slack, Microsoft Teams, or Google Chat.
~~~

## Product Pricing fields

The Product Pricing page observed July 23, 2026 contains:

- `Add Pricing Plan`
- `Pricing plans`
- a maximum of six plans
- currency selection, observed as `$ (USD)` in the supplied form
- `Do you provide these options?` followed by live selectable options

The option labels under `Do you provide these options?` were not present in the supplied text. Use `$browse`
on the rendered form and record the exact labels before preparing the final worksheet; do not guess them.

For every plan capture:

- exact plan name
- concise plan description
- displayed numeric price
- currency
- price unit, such as per user, workspace, or organization
- billing period, such as month or year
- billing cadence and whether annual prepayment is required
- minimum seats/users or commitment
- included limits relevant to the price
- public pricing-page evidence and last-verified date

The page can be populated with AI-fetched website information. Review every value. A numeric amount is
incomplete without its unit and period. When the public page shows both monthly and annual choices, preserve
their exact relationship rather than converting, rounding, or mixing them silently.

For the supplied Team Toast example, verify these source facts before saving:

| Plan | Stated fit | Pricing facts to reconcile |
|---|---|---|
| Free | Up to 25 users; no card; no time limit | $0 |
| Growth | 26–50 users | $1 per user/month or $10 per user/year billed annually |
| Scale | 51+ users | $3 per user/month or $30 per user/year billed annually |

Do not let the form's bare `$1.00` or `$3.00` obscure the per-user/month unit or the annual option. If the form
supports only one price, select the canonical starting price and explain the alternative cadence in the plan
description without exceeding any live limit.

## Submit for review screen

The final page observed July 23, 2026 contains:

- `Your product listing is ready to be reviewed.`
- `Need to make some final changes?`
- `Back`
- `Ready to get listed?`
- `Submit for review`

The readiness message proves only that mandatory form validation passed. It does not prove factual accuracy,
policy compliance, approval, public visibility, category placement, or admin ownership.

Before clicking:

1. Compare every rendered section with the verified submission package.
2. Recheck character limits, assets, feature evidence, target market, and pricing units.
3. Confirm private data and credentials were not persisted in Markdown.
4. Have the user review current privacy terms and legal attestations.
5. Resolve all `BLOCKED`, `PROVISIONAL`, and `USER CONFIRMATION REQUIRED` items.
6. Use `Back` for any correction.
7. Require explicit user authorization for `Submit for review`.

After clicking, capture the visible receipt or confirmation and record the time, submitting account, and next
expected state. Set status to `SUBMITTED FOR REVIEW`; wait for separate evidence before marking approved,
publicly visible, claimed, or category-confirmed.

## Sensitive-data handling

Safe artifact labels:

- `READY TO PASTE` for public, verified copy
- `PRIVATE — ENTER DIRECTLY` for contact information
- `SECRET — ENTER DIRECTLY` for passwords or credentials
- `BLOCKED` for required unknowns
- `OPTIONAL — USER DECISION` for marketing consent or nonessential fields

Never place passwords, session tokens, customer emails, unreleased pricing, or customer PII in the launch
package. Prefer a secure password manager and the Vendor Portal's own review-invitation workflow.

## Submission and approval states

Track these separately:

1. Account created
2. Initial product request started
3. Required listing sections completed
4. User reviewed attestations, privacy policy, and terms
5. Submitted for review
6. Capterra requested changes
7. Changes resubmitted
8. Profile approved
9. Profile publicly visible
10. Profile claimed/admin access confirmed
11. Categories confirmed
12. Review link and analytics validated

An on-screen receipt or completed form is not approval. Approval is not necessarily evidence that the public
profile, final categories, ownership, and analytics are all ready.
