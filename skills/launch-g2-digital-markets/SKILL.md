---
name: launch-g2-digital-markets
description: |
  Prepare, submit, optimize, and operate the shared G2 Digital Markets listing that publishes an eligible
  packaged B2B or B2C software product across Capterra, GetApp, and Software Advice. Covers eligibility,
  duplicate and claim checks, account setup, every listing section, category research, conversion-focused
  descriptions, logo and media, integrations, target market, pricing, compliant reviews, measurement, and
  ongoing profile maintenance. Uses the browse skill to inspect the live category, its top five products, and
  the associated product websites. Writes a durable Markdown package under .ulpi/launch/g2-digital-markets.
  Use when a startup wants to create, claim, improve, or grow listings on any of these three properties.
---

<EXTREMELY-IMPORTANT>
Treat these rules as blocking:

1. PASS ELIGIBILITY FIRST. For the current self-service product route, the submitter must represent a real
   B2B or B2C software product, not a service or consulting offer; it must be packaged/off-the-shelf rather
   than custom-built; and the submitter must directly represent the software vendor.
2. NEVER CHECK A FALSE BOX. Capterra's broader Profile Guidelines can cover some services and vendor-authorized
   resellers, but the current product-request screen has narrower attestations. Escalate exceptions to
   Capterra support instead of misrepresenting eligibility.
3. NEVER CREATE A DUPLICATE. Check for the product, vendor, prior names, and spelling variants. Claim or update
   an existing profile rather than submitting another one.
4. USE ONLY REAL, PUBLICLY AVAILABLE OFFERS. The product must fit an existing category and have a public
   trial, demo, purchase, or information-request CTA. A waitlist-only product is not ready.
5. TELL THE TRUTH. Do not invent capabilities, integrations, pricing, customers, screenshots, review quotes,
   awards, rankings, or support and deployment options.
6. FOLLOW CAPTERRA COPY RULES. Use English, unique third-person copy, standard grammar, and the official
   product name. Avoid first-person language, superlatives, comparative claims, CTAs, contact details, URLs,
   HTML, line breaks, excessive capitalization, and special characters in the description.
7. REVIEWS MUST BE AUTHENTIC AND UNBIASED. Never review-gate, coach answers, ghostwrite, use generative AI for
   a customer's review, target only happy users, pay for sentiment, or ask conflicted reviewers.
8. RESEARCH THE LIVE MARKET. Use $browse to inspect the current Capterra category and the top five relevant
   products before writing final copy. Keep the run narrow, evidence-led, and limited to what is needed for
   this product submission. Do not bulk scrape, copy reviews, evade access controls, or republish page data.
9. VERIFY THE LIVE FORM. Fields, limits, legal entities, and entitlements change. Recheck the visible form and
   official guidelines before submission; record a verification date.
10. PERSIST THE WORK. Write all work under .ulpi/launch/g2-digital-markets so submission does not depend on
    chat history.
</EXTREMELY-IMPORTANT>

# Launch on G2 Digital Markets

## Goal

Create one truthful, conversion-focused package for the shared listing request covering Capterra, GetApp, and
Software Advice:

- `SUBMISSION.md` — eligibility, duplicate result, account setup, and every paste-ready form field
- `CATEGORY-EVIDENCE.md` — category choice, buyer expectations, and native-capability proof
- `BENCHMARK.md` — dated category and competitor analysis with sponsored/organic distinctions
- `PROFILE.md` — final descriptions, product details, media, integrations, target market, and pricing
- `REVIEW-PLAN.md` — compliant review recruitment, outreach, cadence, and responses
- `OPERATIONS.md` — approval tracking, 30/60/90-day work, owners, and maintenance
- `CHECKLIST.md` — blocking readiness and submission gates
- `analytics.md` — UTMs, referral/conversion events, validation, and reporting
- shared `.ulpi/launch/positioning.md` — grounded product truth reused by other launch skills

## Step 0: Identify the product and mode

If the product is not unambiguous, ask:

> Which product or platform are you listing through G2 Digital Markets? Send its canonical product or pricing
> URL and any existing Capterra, GetApp, or Software Advice profile URLs.

Do not infer the product from the repository or company name. Determine the mode:

- `NEW` — no profile exists
- `CLAIM` — an accurate but unclaimed profile exists
- `CORRECT` — duplicate, wrong vendor/name/category, or stale profile
- `OPTIMIZE` — claimed profile is incomplete or weak
- `GROW` — profile is strong and needs reviews and ongoing operations

Gather the product name, vendor name, canonical URL, availability, CTA, representative relationship, target
buyers, deployment, pricing, current customers, and owner. Ask one grouped follow-up only for private or
unknowable facts.

## Step 1: Load the rules and set up research

Read these references as needed:

- `references/eligibility-and-submission.md` before eligibility, account, or form work
- `references/profile-and-category-playbook.md` before category, copy, or asset work
- `references/reviews-and-operations.md` before reviews, ranking, or ongoing operations
- `references/artifact-templates.md` before writing the final package

Use `$browse` to inspect the startup's canonical site, pricing, documentation, product UI, the live Capterra
category and top five relevant Capterra product profiles, and their vendor-owned sites. Check availability
with `browse --version` as directed by the browse skill.

If normal `$browse` receives a 403, challenge, or anti-automation block, load and follow `$browse-stealth`:
verify Camoufox, stop the current server, retry in headed Camoufox, and stabilize before inspection. If stealth
is still blocked by IP reputation, require the permitted user-assisted handoff or residential proxy and keep
the live benchmark blocked. Do not replace the five rendered profiles with snippets.

If `$browse` is unavailable, suggest without installing automatically:

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

If unavailable, stop before final copy, mark `BENCHMARK.md` as `BLOCKED — BROWSE REQUIRED`, and list the
installation commands. Do not claim to have researched the category or recommend a final description without
the live top-five evidence. Never copy full reviews or collect personal reviewer information.

## Step 2: Ground the product

Reuse `.ulpi/launch/positioning.md` only if current. Otherwise inspect the product site and repository, then
write or refresh it with:

- official product and vendor names
- one-sentence positioning and primary buyer problem
- ideal users, roles, industries, and company sizes
- current native capabilities and defensible differentiators
- deployment, devices, languages, regions, security, support, and training
- public pricing, trial/free-version status, and billing units
- verified integrations and evidence URLs
- canonical page, public CTA, and current availability
- competitors/alternatives and last-verified dates

Every claim in the profile must trace to this brief or an explicit user confirmation.

## Step 3: Pass eligibility and duplicate gates

Apply `references/eligibility-and-submission.md`. For the self-service entry screen, record PASS/FAIL and
evidence for these exact attestations:

1. `I am submitting a B2B or B2C software product, not a service or consulting offer.`
2. `My product is an off-the-shelf software, not a custom built solution.`
3. `I am a direct representative of the software vendor, not a reseller.`

Also verify category fit, public availability, a real CTA, official name/domain consistency, and excluded
product types. Search for an existing listing manually in a normal browser. Issue one verdict:

- `ELIGIBLE — NEW LISTING`
- `ELIGIBLE — CLAIM OR UPDATE EXISTING`
- `ELIGIBLE — SUPPORT REVIEW REQUIRED`
- `NOT READY`
- `INELIGIBLE`

Stop the submission path on NOT READY or INELIGIBLE, but document remediation. Never attest on the user's
behalf or click the final legal/submission control without explicit authorization.

## Step 4: Build the exact account worksheet

The account setup observed July 23, 2026 contains:

- Company/product name and website, prefilled when available
- Select Company Size
- Country
- Enter First Name
- Enter Last Name
- Select Department
- Select Job Level
- Business Phone country code and Enter Phone Number
- Select Time Zone
- New Password
- Verify New Password

Write these in `SUBMISSION.md` in visible order. Public values may be populated. Mark personal contact fields
`PRIVATE — ENTER DIRECTLY`; do not store a raw phone number without explicit user instruction. Mark both
password fields `SECRET — ENTER DIRECTLY`; never request, generate, echo, or persist the password. Tell the
user to use a password manager. Do not guess company size, department, job level, country, or time zone.

## Step 5: Build the initial listing request

Map the current entry screen exactly:

- Business Email `required` — `PRIVATE — ENTER DIRECTLY`
- Product Name `required` — paste-ready official product name
- Product Website `required` — canonical public URL
- `I want to be contacted to learn about brand building and lead generation` — optional marketing consent;
  default to unchecked unless the user chooses it
- privacy-policy acknowledgement — link the policy and require user review

Then map the current Product Listing Request sections:

1. Product description
2. Product details
3. Media
4. Integrations
5. Category
6. Target market
7. Product pricing
8. Submit for review

Use the visible form as final truth for fields not yet documented here. Capture field labels, required state,
help text, allowed values, limits, and section order into `SUBMISSION.md`; do not invent missing controls.

## Step 6: Prove category fit and benchmark the market

Use `$browse` on the live category page. After `goto`, wait for network idle and use `snapshot -i`, `text`,
and `links` to inspect the rendered result. Record the category URL, date, region, filters, sort order, and
which cards appear sponsored. Sponsored profiles can appear first and must not be described as organic
category leaders.

Research exactly five relevant category leaders. Prefer the first five organic results in the active default
or buyer-relevant sort; if sponsored cards interrupt the list, record them separately and continue until five
organic profiles are covered. When the default sort cannot be established, say so and use the visible order.
Open each profile in the same persistent browse session and capture concise observations: buyer, problem,
overview structure, core capabilities, pricing visibility, media, integrations, target market, CTA, and
recurring buyer questions. Do not reproduce full reviews or competitor descriptions.

Use `$browse` on each product's vendor-owned public site to validate current claims and identify:

- category table stakes
- overused or unsupported language
- credible differentiation and whitespace
- missing buyer questions the profile can answer
- proof patterns and pricing/media expectations

Write `BENCHMARK.md` with all five profile URLs, vendor URLs, source dates, the selection method, and a compact
comparison table. Write `CATEGORY-EVIDENCE.md` mapping each category expectation to a native capability and
proof. For login, CAPTCHA, or MFA that needs a human, follow the browse skill's handoff protocol. For an
anti-automation block, use `$browse-stealth` first as required above; never fabricate the benchmark.

## Step 7: Craft the product descriptions

Use `launch-copy` when available. Draft three truthful options:

- category-led — establishes the category, buyer, and core capability immediately
- outcome-led — starts with the costly problem and a verifiable outcome
- differentiation-led — leads with the strongest defensible distinction

The currently observed form requires:

- Short description: maximum 135 characters
- Product overview: English, minimum 400 and maximum 1,000 characters

Count Unicode characters exactly, including spaces and punctuation. For each option, write both lengths and
score truth, clarity, category relevance, differentiation, buyer usefulness, and policy compliance. Recommend
one version. Keep the final copy in `PROFILE.md` and duplicate the exact paste-ready values in `SUBMISSION.md`.

Apply all copy rules in `references/profile-and-category-playbook.md`. Do not reuse website boilerplate
verbatim: Capterra requires a unique overview and may edit final profile copy.

## Step 8: Complete every profile section

Populate all fields revealed by the live form. At minimum, `PROFILE.md` must cover:

- official product and suffix-free company names
- canonical product URL and verified public CTA
- short description and 400–1,000-character overview
- product details and use cases
- logo and real-interface media inventory
- verified integrations, each with evidence
- proposed primary and secondary categories with proof
- target roles, industries, regions, and company sizes
- deployment, devices, languages, support, and training
- pricing model, starting price, billing unit/frequency, currency, free trial, and free version
- source, owner, and last-verified date for every mutable field

Logo requirement observed July 23, 2026: PNG, JPG, JPEG, or WebP under 5 MB. The current Media page requires
at least one screenshot and allows at most five. Each screenshot requires a caption. Screenshot formats are
PNG, WebP, JPEG, or JPG and every image must be under 5 MB. Never use stock imagery or marketing slogans as
screenshots. Video is optional; accepted URL providers are Vimeo, Wistia, and YouTube, with YouTube preferred.
Videos must be in English and about the product.

For every live field, `SUBMISSION.md` must have:

- exact field label
- required/optional status
- visible instructions and allowed values
- a `READY TO PASTE` block or safe `ENTER DIRECTLY` instruction
- character count when limited
- evidence/source and last-verified date
- `BLOCKED` plus one precise question if required data is missing

Finish with an ordered click-through checklist matching the live section order.

The Product Details page observed July 23, 2026 requires these exact groups:

- `Which languages is your product available in?` — required multi-select; current UI shows 47 options
- `Which countries is your product available in?` — required multi-select; current UI shows 88 options
- `Support Options` — required; visible values: Email/Help Desk, FAQs/Forum, Knowledge Base, Phone Support,
  24/7 (Live Rep), and Chat
- `Training Options` — required; visible values: In Person, Live Online, Webinars, Documentation, and Videos
- `Deployment Options` — required; visible values grouped as Web: Cloud, SaaS, Web-based; Desktop: Mac,
  Windows, Linux, Chromebook; On-Premise: Windows, Linux; Mobile: Android, iPhone, iPad

The page may prefill these fields with AI-fetched website information. Review every selection against current
product truth; never accept a prefill merely because it appeared automatically.

The Integrations page observed July 23, 2026 requires:

- `Do you offer an Open API?` — required Yes/No; answer Yes only when a real customer/developer API is
  currently offered and provide documentation evidence
- `Add Integrations` — searchable selector for current integrations
- `Added Integrations` — review the resulting chips before saving

Do not claim an Open API because the application uses internal endpoints. Do not add integrations that are
planned, one-way manual exports, or merely possible through an undocumented API.

The Category page observed July 23, 2026 requires:

- one initial primary category
- at least seven features selected from the chosen category's feature list
- a review of all selected features before saving

Capterra makes the final category placement decision. Additional relevant categories can be requested only
after the product is published. Use the live category's exact feature list and map every selected feature to
current product evidence. Never select a feature merely to reach the minimum. If fewer than seven supported
features exist, mark the category `FAIL` and research a better-fitting category.

For `Employee Recognition`, use the exact 37-feature taxonomy recorded in
`references/eligibility-and-submission.md`. Do not apply that taxonomy to another category.

The Target Market page observed July 23, 2026 requires:

- a Target Market description with a maximum of 200 characters
- target industries through `Add industries`
- `Target Company Size`
- `Target Number of Users`

Use the current live option values. Recommend only industries, company sizes, and user-count bands supported
by product evidence or confirmed customer fit. Never default to every segment or claim universal fit. Mark
each selection `USER CONFIRMATION REQUIRED` when public evidence cannot establish actual served clients.

For the Target Market description, count every character, including spaces and punctuation, before presenting
the value. Never estimate the count. Reject or rewrite any draft over 200 characters. Output the exact final
value in a `READY TO PASTE — N/200` block. Keep it in third person and name buyer roles, organization fit, and
relevant operating context without unsupported industries.

The Product Pricing page observed July 23, 2026 allows up to six pricing plans through `Add Pricing Plan`.
For every plan, capture the exact plan name, description, numeric price, currency, billing unit, billing period,
and any minimum user or commitment. Also capture every current option under `Do you provide these options?`
from the live form. Do not infer option labels that are not visible.

The page may prefill pricing with AI-fetched website data. Compare every plan against the canonical pricing
page. Resolve monthly versus annual display, per-user versus flat pricing, and annual-billing discounts before
marking it ready. Never paste a bare amount such as `$1.00` without confirming what it is per and how often it
is billed. Record changes in `SUBMISSION.md` and use no more than six current plans.

The final page observed July 23, 2026 shows `Your product listing is ready to be reviewed`, offers `Back` for
final changes, and presents `Submit for review` under `Ready to get listed?`. Before submission, compare the
rendered review against `SUBMISSION.md`, resolve every blocker, and have the user review the listing, privacy
terms, and legal attestations. Treat `Submit for review` as the external state-changing action: do not click it
without explicit user authorization. After clicking, record evidence and change status to `SUBMITTED FOR
REVIEW`, not `APPROVED` or `PUBLIC`.

## Step 9: Build the review program

Read `references/reviews-and-operations.md` and write `REVIEW-PLAN.md`. Segment a broad, representative set of
actual users. Exclude vendor affiliates, direct competitors, financially interested people, public-sector
users from incentive programs, sanctioned parties, and anyone prohibited by employer policy.

Invitations must ask for honest first-hand feedback without suggesting a rating or wording. Never generate,
edit, submit, or preview a customer's review for them. Use Capterra's approved Vendor Portal collection link.
Any incentive must be nominal, lawful, equally available regardless of sentiment, disclosed, and administered
through the approved workflow. Include the mandatory disclosures from the current Community Guidelines.

Create a neutral initial cohort, an always-on cadence, moderation expectations, response templates, and a
process for routing product feedback. Vendor responses must use portal tools and remain respectful.

## Step 10: Plan approval and sustained success

Write `OPERATIONS.md` with these separate states:

- account created
- listing sections complete
- submitted for review
- changes requested
- approved
- publicly visible
- profile claimed/admin access confirmed
- categories confirmed
- review link active
- analytics validated

Do not call the listing complete from a submission receipt alone. Plan:

- Days 0–30: approval, completeness, first media, pricing, integrations, analytics, representative reviews
- Days 31–60: improve weak sections from buyer questions, refresh media, continue broad review cadence
- Days 61–90: analyze referral quality, respond to reviews, update evidence, and assess category fit
- Quarterly: verify pricing, capabilities, integrations, screenshots, target market, links, and policy changes

Do not promise category rank, badges, Shortlist inclusion, traffic, or leads. Separate sponsored placement from
objective research. Optimize controllable inputs: accuracy, completeness, review quality/recency, buyer fit,
referral conversion, and profile upkeep.

## Step 11: Instrument and validate

Use `launch-analytics` when available. Write `analytics.md` with distinct `utm_source` values for `capterra`,
`getapp`, and `software_advice`, plus a shared campaign convention, landing page, events, owners, dashboard,
and test procedure. Track profile visits when available, referral sessions, demo/trial/purchase conversions,
qualified pipeline, review invitations, published reviews, response time, category status, and completeness.

Validate every artifact against `references/artifact-templates.md`. Final readiness requires:

- eligibility PASS and duplicate route resolved
- no unsupported required field
- descriptions within current limits
- logo valid and at least one real product media asset ready
- category and integration claims have evidence
- private data and passwords excluded from Markdown
- review plan complies with current rules
- user has reviewed legal attestations and privacy terms
- final external submission remains user-controlled unless explicitly authorized

Report the verdict as `READY TO SUBMIT`, `READY TO CLAIM/UPDATE`, or `BLOCKED`, followed by only the blocking
items. All output must be Markdown.
