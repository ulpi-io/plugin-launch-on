---
name: launch-alternativeto
description: |
  Prepare, submit, optimize, and operate an AlternativeTo application listing. Covers the seven-day account
  age gate, eligibility and duplicate checks, application name and URLs, English descriptions, platforms,
  cost and license classification, application types, tags versus features, icon and screenshots, accurate
  competitor associations, developer ownership, moderation, organic community participation, approval,
  analytics, and ongoing maintenance. Uses the browse skill to research the live submission form and the top
  five products with the same main task and focus. Writes a paste-ready package under .ulpi/launch/alternativeto.
  Use when a startup wants to add, claim, correct, improve, or grow a product on AlternativeTo.
---

<EXTREMELY-IMPORTANT>
Treat these rules as blocking:

1. WAIT SEVEN DAYS. A new AlternativeTo account cannot submit a new app page until seven full days after
   account creation. Record the creation timestamp and earliest eligible submission date. Never claim the
   package is submit-ready before that gate passes.
2. SEARCH BEFORE SUBMITTING. Never create a duplicate. Search product, company, domain, former names, and
   spelling variants. Claim, edit, or report the existing page instead.
3. PASS ELIGIBILITY. The app must support English. Closed-beta or merely announced products are not accepted;
   an accessible open beta may be considered. AlternativeTo generally rejects hardware and many low-value,
   local, custom-service, basic-tool, clone, wrapper, and oversaturated submissions.
4. CREATE ONE PRODUCT ENTRY. Do not create separate pages for Free, Pro, web, desktop, or other editions that
   share the same main purpose. Use one generic product name and describe editions truthfully.
5. CLASSIFY COST AND LICENSE ACCURATELY. A usable free tier that performs the main purpose can be Freemium.
   A time- or usage-limited trial is Commercial. Open Source requires a real OSI-compatible license and source.
6. ALTERNATIVES REQUIRE THE SAME MAIN TASK AND FOCUS. Shared features, audience, category words, integrations,
   or brand competition alone do not make two products alternatives.
7. USE CLEAN COPY AND URLS. Descriptions must not contain website links, email addresses, phone numbers, or
   physical addresses. Use the dedicated URL fields. AlternativeTo generally does not allow UTM parameters
   in the Official Website URL.
8. USE $browse FOR LIVE RESEARCH. Inspect the current form and the top five relevant AlternativeTo products
   before final copy. If ordinary access is blocked, load and follow `$browse-stealth`, retry in headed Camoufox,
   and stabilize the render. If stealth also fails because of IP reputation, mark live-only fields BLOCKED until
   the user completes the permitted handoff or supplies an approved residential proxy.
9. NEVER MANIPULATE THE COMMUNITY. Do not buy, incentivize, pressure, coordinate, or fabricate likes, votes,
   comments, or reviews. Sharing is allowed only as an invitation to genuinely evaluate the product.
10. VERIFY AND PERSIST. Recheck the live form and official FAQ immediately before submission. Write the full
    Markdown package under .ulpi/launch/alternativeto.
</EXTREMELY-IMPORTANT>

# Launch on AlternativeTo

## Goal

Produce:

- `SUBMISSION.md` — account gate, eligibility, duplicate result, and every paste-ready form field
- `ALTERNATIVE-MAP.md` — primary task/focus and evidence for every proposed association
- `BENCHMARK.md` — dated top-five research and credible profile whitespace
- `PROFILE.md` — final name, descriptions, URLs, platforms, licensing, types, tags, features, and media
- `COMMUNITY-PLAN.md` — ethical announcement, likes, comments, reviews, and moderation rules
- `OPERATIONS.md` — submission, approval, ownership, maintenance, and 30/60/90-day work
- `CHECKLIST.md` — blocking gates and final verdict
- `analytics.md` — clean-link referral attribution and conversion reporting
- shared `.ulpi/launch/positioning.md` — grounded product truth

## Step 0: Identify the product and mode

If not unambiguous, ask:

> Which product or platform are you listing on AlternativeTo? Send its canonical product URL and any existing
> AlternativeTo page.

Determine the mode:

- `NEW` — no page exists
- `CLAIM` — an accurate page exists but the developer lacks admin rights
- `CORRECT` — duplicate or inaccurate page exists
- `OPTIMIZE` — page exists but is incomplete or weak
- `GROW` — page is strong and needs accurate alternatives and organic community activity

Gather product name, canonical URL, public availability, English support, main task/focus, supported platforms,
cost/license, source repository when applicable, creator/company, app-store URLs, existing page, and account
creation date. Ask one grouped follow-up only for private or unknowable facts.

## Step 1: Load references and require browse

Read:

- `references/eligibility-and-submission.md` before the account, eligibility, duplicate, or form stages
- `references/profile-and-alternatives.md` before benchmarking, description, taxonomy, or association work
- `references/community-and-operations.md` before likes, reviews, ownership, approval, or maintenance
- `references/artifact-templates.md` before writing the final package

Use `$browse` and start with `browse --version`. If it is missing, suggest without installing automatically:

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

Use one persistent session. After navigation, wait for network idle and inspect with `snapshot -i`, `text`,
and `links`. If the site returns an access block, load `$browse-stealth`, verify Camoufox, stop the current
server, and retry with headed Camoufox. If stealth remains blocked, use the permitted handoff/proxy path;
official indexed sources may guide URLs but unobserved live fields and the top-five gate remain `BLOCKED`.

## Step 2: Ground product truth

Reuse `.ulpi/launch/positioning.md` only when current. Otherwise inspect the canonical site, pricing, docs,
app-store pages, repository, and actual UI. Record:

- official generic product name and creator
- one primary task and focus
- intended users and use cases
- native capabilities and differentiators
- supported platforms and delivery modes
- current pricing/free tier/trial and license
- English support and public-access state
- canonical clean URLs and stores
- source, owner, and last-verified date for every claim

Do not use roadmap items or marketing implications as current capability.

## Step 3: Run account and eligibility gates

Apply `references/eligibility-and-submission.md`. Calculate:

`earliest submission = account created timestamp + 7 full days`

Issue one account verdict:

- `ACCOUNT ELIGIBLE`
- `ACCOUNT AGING — ELIGIBLE YYYY-MM-DD HH:MM TZ`
- `ACCOUNT DATE UNKNOWN — BLOCKED`

Then issue one product verdict:

- `ELIGIBLE — NEW`
- `ELIGIBLE — CLAIM/EDIT EXISTING`
- `ELIGIBLE — ADMIN REVIEW DISCRETION`
- `NOT READY`
- `INELIGIBLE`

Stop the external submission on any blocked gate, but keep preparing the package during the seven-day wait.

## Step 4: Search duplicates and resolve ownership

Use `$browse` or indexed search to query product name, creator, canonical domain, prior names, and variants.
Record every query and result URL in `SUBMISSION.md`.

If a page exists:

- use `Contribute to this page` → `Edit / Update Information` for factual changes
- use `Report something wrong` for bad URL, platform, price, discontinued/dangerous status, or other errors
- for developer admin rights, create an account and email `support@alternativeto.net` with the username, app,
  and ownership proof; a message from the product's domain is suitable evidence
- do not submit a new application

If another product shares the same name, use a concise functional qualifier only when needed to distinguish it.

## Step 5: Research the live market and top five

First define the product's primary task and focus in one sentence. Search AlternativeTo for the closest known
product and relevant application type/tag. Inspect exactly five leading products that a real user would
consider for that same job. Record selection method, active platform/cost filters, visible ordering, date, and
profile URLs.

For each profile capture:

- one-line positioning and description structure
- cost/license, platforms, application types, tags, and features
- official/store/source links
- icon and screenshot strategy
- number and quality of listed alternatives
- likes, reviews/comments, and update freshness only as contextual signals
- buyer questions answered and missing

Open each vendor-owned site with `$browse` to validate current facts. Never copy profile text. Write
`BENCHMARK.md` with table stakes, overused claims, taxonomy patterns, and credible whitespace.

## Step 6: Build the alternative map

Write `ALTERNATIVE-MAP.md`. For each candidate association ask:

1. What is the other product's main task and focus?
2. What is this product's main task and focus?
3. Would a person searching for `alternatives to X` reasonably want this product for the same primary job?
4. Which meaningful differences should be disclosed: platform, cost, hosting, audience, or workflow?

Mark each `PASS`, `FAIL`, or `BORDERLINE — USER/ADMIN JUDGMENT`. Shared secondary features are insufficient.
Prefer a small set of strong associations over a large spam-like list.

After the app exists, suggest associations through the target app page: `Contribute to this page` → `Suggest
Alternatives`. For an unlisted app, the live flow may offer `Add a new application as a new alternative`.
Every association is subject to moderation.

## Step 7: Build the submission worksheet

Use the live `Suggest a new application` flow as final truth. The observed form contains these sections:

1. Main info — Name, Short Description, Website, Full Description, Supported Languages, Pricing, Is Opensource?
2. Tags — required Tags that drive categories and Application Type, plus relevant Features
3. Platforms — required Platforms
4. Author / Social Media — required Company / Author, X username, Facebook URL
5. Icon & Screenshots — required Application Icon, Screenshots, Videos
6. Meta — optional Note about your changes
7. `Submit the application`

Read `references/eligibility-and-submission.md` for the exact current help text and media contract. Capture
every visible option and character limit that appears at execution time.

`SUBMISSION.md` must contain, in live order:

- exact field label and required/optional state
- `READY TO PASTE` value or safe `ENTER DIRECTLY`
- deterministic character count for every limited field
- evidence and last-verified date
- `BLOCKED` plus one precise question for missing required data
- final `Submit the application` checklist

Never persist passwords. Treat username and email as private unless the user explicitly wants them recorded.
The current signup screen says the username cannot be changed and an email/password signup requires at least
eight password characters; have the user review the live terms/privacy notice.

## Step 8: Create the buyer-facing profile

Use `launch-copy` when available and `references/profile-and-alternatives.md`. Draft three description angles:

- task-led — names the job and user immediately
- differentiation-led — names a defensible mechanism or fit
- migration-led — explains why someone replacing a known product should consider it

Keep all copy English, factual, unique, and useful. Do not include any URLs, addresses, email, or phone details
in descriptions. Score truth, task clarity, taxonomy fit, differentiation, alternative relevance, and policy
compliance. Recommend one after the benchmark.

Populate:

- generic application name, creator, clean Official Website, Creator Website, store/social/source URLs
- current Platforms, Cost/License, and detailed open-source license where applicable
- description(s), application type(s), Tags, and Features
- square icon and real screenshots
- initial strong alternative associations

The live form accepts JPEG, PNG, SVG, or WebP icons and suggests a transparent square at least 128×128. Prefer
280×280 or larger when available for quality. The icon is required. Screenshots accept JPEG, PNG, or WebP and
must be at most 3 MB each; animated screenshots are unsupported. Add current screenshots because missing
screenshots may cause denial. AlternativeTo currently supports YouTube video URLs only. Remove PII, secrets,
internal URLs, and unreleased functionality from media.

## Step 9: Plan approval and organic community participation

Read `references/community-and-operations.md`. The official FAQ says approval usually takes a couple of days
to one week. Track submitted, changes requested, approved, public, ownership confirmed, and associations
approved as separate states.

Sharing the published page is allowed, but ask people to evaluate it honestly. Never reward, pressure, script,
or fake likes/reviews. Do not use the personal profile or public Lists as promotional spam. Comments and reviews
are moderated; do not ghostwrite user feedback.

Write neutral announcement copy, a monitoring cadence, factual response guidance, and correction routes.
Do not promise ranking: likes matter, but AlternativeTo uses undisclosed additional factors and organic quality.

## Step 10: Measure and maintain

Use `launch-analytics` when available. AlternativeTo generally requires a clean Official Website URL without
UTM parameters, so use server/analytics referrer data for `alternativeto.net` and downstream conversion events.
Do not add tracking parameters unless the current platform explicitly permits them.

Track public status, profile freshness, approved alternatives, qualified referral sessions, activation and
conversion, organic likes/comments, factual correction time, and assisted pipeline. Recheck links, platforms,
pricing/license, description, tags/features, screenshots, and availability quarterly.

## Step 11: Validate and hand off

Apply `references/artifact-templates.md`. Final readiness requires:

- account is at least seven full days old
- email/account access works and user reviewed terms
- eligibility and duplicate gates pass
- English support and public availability are evidenced
- clean official URL and accurate cost/license/platforms
- no contact details or URLs in descriptions
- icon and screenshots are current and owned
- every proposed alternative passes the main-task-and-focus test
- every live field is captured and required values are complete
- community plan prohibits manipulation
- final external submission remains user-controlled unless explicitly authorized

Report `READY TO SUBMIT`, `READY TO CLAIM/EDIT`, `ACCOUNT AGING`, or `BLOCKED`, followed only by remaining
blockers. Keep all artifacts in Markdown.
