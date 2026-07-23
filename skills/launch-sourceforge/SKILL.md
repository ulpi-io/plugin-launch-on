---
name: launch-sourceforge
description: |
  Create, claim, optimize, and operate either a SourceForge business-software listing, a hosted open-source
  project, or a legitimate linked presence using both routes. Covers eligibility and duplicate checks, exact
  submission fields, mandatory live top-five research with $browse and $browse-stealth fallback, categories,
  conversion copy, media, pricing, features, integrations, project metadata, releases and downloads, reviews,
  analytics, and ongoing maintenance. Writes a paste-ready package under .ulpi/launch/sourceforge. Use when a
  startup, software vendor, or open-source maintainer wants to get listed, improve an existing SourceForge page,
  or operate SourceForge as a durable discovery and download channel.
---

<EXTREMELY-IMPORTANT>
Treat these rules as blocking:

1. CHOOSE THE RIGHT ROUTE. A commercial business-software listing and a hosted open-source project are different
   products with different eligibility, forms, fields, and success mechanics. Do not draft until the route is
   `BUSINESS_LISTING`, `OPEN_SOURCE_PROJECT`, or genuinely `BOTH_LINKED`.
2. PASS ELIGIBILITY. A business listing must be publicly and commercially available to businesses, submitted by
   the vendor or an authorized representative, and fit a current SourceForge category. An open-source project
   must publish source under a license compliant with the Open Source Definition. A source-available, freeware,
   consulting, reseller, custom-development, or unreleased offer must not be mislabeled.
3. SEARCH BEFORE CREATING. Search names, domains, former names, product editions, and project URL names. Claim,
   correct, or request support instead of creating duplicates or using a second page to escape reviews/history.
4. USE $browse AND RESEARCH EXACTLY FIVE. Inspect the live form, category/directory, exactly five relevant
   same-route profiles, and their official sites or repositories before final copy. For `BOTH_LINKED`, benchmark
   five business listings and five open-source projects separately. Search snippets alone do not satisfy this.
5. USE STEALTH WHEN BLOCKED. If normal `$browse` receives 403, a challenge, or anti-automation block, load and
   use `$browse-stealth`: verify Camoufox, stop the current server, then retry in headed Camoufox and stabilize the
   page. If stealth is still blocked by IP reputation, record the exact evidence and require a user-assisted
   browser handoff or residential proxy. Never invent the missing top-five observations or finalize copy.
6. SEPARATE ORGANIC FROM PAID. Record Sponsored, Partner, promoted, and plan-enhanced placements separately.
   Never call paid visibility an organic ranking signal or imply that payment is required for a base listing.
7. CLAIMS MUST BE TRUE. Categories, features, pricing, free trial/version, deployment, platforms, API,
   integrations, support, training, regions, languages, audience, license, source, releases, and security claims
   require current first-party evidence. SourceForge makes final category and approval decisions.
8. SHIP SAFE RELEASES. For hosted projects, publish the correct source/license, clean binaries, release notes,
   version/platform labels, checksums and signatures where practical, documentation, and support paths. Do not
   upload malware, bundled unwanted software, misleading download buttons, secrets, or abandoned builds as new.
9. KEEP REVIEWS AUTHENTIC. Never fabricate, gate, condition, pressure, or write reviews. Default to neutral,
   non-incentivized invitations. Any incentive must run only through SourceForge's current official Vendor
   Reviews Program, with an eligible upgraded plan and all current limits; never independently offer incentives.
10. VERIFY LIVE AND PERSIST. Forms, plans, policies, sort order, and limits change. Recheck immediately before
    external action and write the complete Markdown package under `.ulpi/launch/sourceforge`.
</EXTREMELY-IMPORTANT>

# Launch on SourceForge

## Goal

Produce:

- `ROUTE-AND-ELIGIBILITY.md` — route, duplicate search, eligibility evidence, and verdict
- `SUBMISSION.md` — every current field in live order with paste-ready values and exact limits
- `CONTENT-REQUIREMENTS.md` — five-listing-derived baseline, recommended, generated, and plan-gated content
- `CATEGORY-EVIDENCE.md` — primary/additional category, features, competitors, and evidence
- `BENCHMARK.md` — dated `$browse` top-five analysis, with paid placements separated
- `PROFILE.md` — conversion-focused copy, details, media, FAQs, and CTAs
- `PROJECT-RELEASES.md` — open-source project metadata, tools, files, release, and security plan
- `REVIEW-PLAN.md` — authentic invitation, response, and current program-policy workflow
- `OPERATIONS.md` — owners, plan entitlements, maintenance, support, and 30/60/90-day work
- `CHECKLIST.md` — blocking gates and final readiness verdict
- `analytics.md` — listing, referral, download, review, and downstream-conversion measurement
- shared `.ulpi/launch/positioning.md` — grounded product truth

## Step 0: Identify software and route

If not unambiguous, ask:

> Which software are you listing on SourceForge? Send the canonical product URL, whether it is commercial
> business software, open-source software, or both, and any existing SourceForge product/project URLs.

Determine one route:

- `BUSINESS_LISTING` — commercial B2B software/service that fits the vendor directory
- `OPEN_SOURCE_PROJECT` — source and downloads hosted or mirrored as an eligible open-source project
- `BOTH_LINKED` — a real open-source project plus a distinct commercial offering from the same vendor

Then determine mode: `NEW`, `CLAIM`, `CORRECT`, `OPTIMIZE`, or `OPERATE`. Gather canonical name/domain,
company/maintainer, authority, product availability, license/repository, pricing, buyer/user audience, current
SourceForge URLs, desired categories, release owner, review owner, plan, and analytics owner.

## Step 1: Load references and browser capabilities

Read the relevant references before acting:

- `references/routes-eligibility-and-submission.md` for route, eligibility, duplicates, and forms
- `references/business-profile-and-benchmark.md` for commercial profiles and top-five research
- `references/open-source-project-and-releases.md` for projects, tools, downloads, and releases
- `references/reviews-plans-and-operations.md` for reviews, paid plans, analytics, and maintenance
- `references/artifact-templates.md` before writing final artifacts

Use `$browse`; start with `browse --version`. If unavailable, suggest installing the browse plugin without doing
so automatically. For Claude Code use `/plugin marketplace add ulpi-io/marketplace` then
`/plugin install browse@ulpi`. For Codex use `codex plugin marketplace add ulpi-io/marketplace` then
`codex plugin add browse@ulpi`.

Use one persistent normal browser session. On 403/challenge/block, explicitly load `$browse-stealth`, run
`browse --runtime camoufox doctor`, stop the current server, retry with
`browse --runtime camoufox --headed goto <url>`, wait for stability, then inspect with text, links, or a fresh
interactive snapshot. Follow the stealth skill exactly. If the page remains blocked, do not substitute snippets
for live evidence: mark the benchmark `BLOCKED — LIVE TOP-FIVE BROWSE REQUIRED` and request the permitted
handoff/proxy path.

## Step 2: Ground product truth

Browse the canonical homepage, product/features, pricing, documentation, support, legal/license, repository,
releases, integrations, and security pages. Record evidence URLs and verification dates for:

- exact product/project and company/author identity
- primary audience, job, problem, workflows, differentiators, and current capabilities
- pricing units, billing periods, tiers, free trial/version, and CTA destination
- platforms/deployment, regions, languages, organization types/sizes, support, and training
- API and named integrations
- license, repository, current stable version, supported OS/architectures, checksums/signatures, and support path
- approved logo, cover image, screenshots, video, captions, rights, and freshness

Reuse `.ulpi/launch/positioning.md` only when current. Never convert roadmap claims into listing facts.

## Step 3: Search duplicates and prove eligibility

With `$browse`, search SourceForge and the public web for exact name, domain, vendor/author, former names, common
spellings, project URL-name candidates, and editions. Record every result in `ROUTE-AND-ELIGIBILITY.md`.

For business software prove public commercial B2B availability, vendor authorization, website/pricing or sales
path, and category fit. For open source prove the public source location, exact license text/identifier, license
compatibility, maintained download/release intent, and project ownership. Issue one verdict:

- `ELIGIBLE — CREATE`
- `ELIGIBLE — CLAIM/OPTIMIZE`
- `BOTH ROUTES ELIGIBLE — KEEP PURPOSES DISTINCT AND CROSS-LINK`
- `SUPPORT REVIEW REQUIRED`
- `NOT ELIGIBLE`

## Step 4: Capture the live submission flow

Use the current form as final truth. For a business listing, the observed July 23, 2026 initial request includes:

- Your Name, Email Address, Company, Your Title, Website, Phone, Company Founded, Company Location
- Software Title, Logo, Product Description, Audience
- consent to current terms, privacy policy, and communications

The live form may load more fields dynamically; browse the full form and capture them. Logo guidance currently
prefers a square, high-resolution JPG, GIF, or PNG. For an open-source project, the observed registration asks
for Project Name, URL name, and selected services/tools; the URL name is 3–30 letters, numbers, or dashes and a
later rename requires support. A first project may require private phone/PIN verification.

After creation, capture every edit surface. Put fields in exact live order with `READY TO PASTE`, `SELECT`,
`UPLOAD`, `ENTER DIRECTLY`, `NOT APPLICABLE`, or `BLOCKED`; include visible character/file limits and computed
counts. Never store passwords, PINs, verification links, customer lists, or private credentials.

## Step 5: Run the live top-five benchmark

Choose the narrowest relevant category and buyer/user intent. Inspect exactly five leading same-route pages in
the active live ordering. Record timestamp/timezone, URL, locale, category, filters, sorting, rank/position, and
why each is comparable. Separate ads, Sponsored, Partner, and other promoted placements from organic results.

For business listings compare identity, audience, description structure, pricing, CTAs, categories/features,
platforms, support/training, integrations/API, screenshots/video/captions, FAQs, proof, reviews/responses, and
vendor-site consistency. For open-source projects compare summary, description, features, samples, categories,
license, platforms, languages, intended audience, UI, programming languages, files/releases, recency, download
path, documentation/support, activity, reviews, and official-site/repository consistency.

Create `CONTENT-REQUIREMENTS.md` before writing copy. Classify every observed element as `REQUIRED/BASELINE`,
`RECOMMENDED`, `PLAN-GATED/PAID`, `SOURCEFORGE-GENERATED`, or `NOT RELEVANT`, with exact input, constraint,
evidence, buyer/user question, and owner. Do not copy competitors or review text; summarize patterns.

## Step 6: Select category, features, and comparisons

Choose the narrowest accurate primary category supported by the product's core job. Record current label/URL,
offer evidence, benchmark peers, search intent, and `PASS`, `BORDERLINE`, or `FAIL`. Add extra categories only
when native capability supports them and the user's plan or project UI permits them.

For business listings, map truthful category-specific descriptions, features, integrations, API, competitors,
deployment, audience, organization types/sizes, regions, and languages. For projects, map categories, OS,
languages, intended audience, user interface, programming languages, and license. Do not category/tag stuff.

## Step 7: Build the business profile

For `BUSINESS_LISTING` or the business half of `BOTH_LINKED`, prepare:

- logo, 1300x200 cover image where available, company information, homepage and social URLs
- audience, concise positioning, full product description, and category-specific descriptions
- starting price, pricing details, billing unit/period, free trial/version, and CTA
- platforms/deployment, support, training, API, integrations, regions, languages, organization types/sizes
- categories, features, competitors/alternatives, up to six screenshots with useful captions, and YouTube video
- default FAQ accuracy plus custom FAQs only when the current plan supports them
- plan-eligible case studies, articles, gated assets, interactive demo, and visitor/intent analytics

Draft three description angles—buyer-job led, differentiation led, and proof/reassurance led—score them against
the five-profile benchmark, and recommend one. Every claim must link to first-party evidence.

## Step 8: Build the project and release system

For `OPEN_SOURCE_PROJECT` or the project half of `BOTH_LINKED`, prepare project Name, Unixname/URL name, Home
Page, YouTube video, one-to-two-sentence Short Summary, Full Description, Support Page, X handle, Facebook page,
logo, status, categories, license, features, screenshots/samples, OS, languages, intended audience, UI, and
programming languages. Configure only needed tools, users, roles, labels, and immutable URL paths.

Create `PROJECT-RELEASES.md`: repository/source location, default download, directory structure, stable version,
artifacts by OS/architecture, source archive, license/notices, release notes, install/upgrade/rollback directions,
checksums/signatures/SBOM where practical, malware/secret scan, support/security reporting, and retirement policy.
Test each public download in a clean environment and verify filenames, sizes, hashes, redirects, and version.

## Step 9: Build the review and response plan

Use a SourceForge-generated review URL or current supported vendor workflow. Invite the full eligible cohort at
the same experience point with neutral language, suppression, frequency limits, privacy approval, and no rating
condition. Never generate customer review text.

Default to no incentives. If the user explicitly wants an incentive, verify the current Vendor Reviews Program,
upgraded-plan eligibility, country and recipient restrictions, fixed cap, value limit, disclosure, and equal
treatment regardless sentiment; SourceForge must administer it. Prepare professional response SLAs and reply
without PII, arguments, or pressure to edit/remove criticism.

## Step 10: Operate and measure

Record current Free versus paid/plan-gated entitlements. Build a 30/60/90-day plan plus weekly/monthly/quarterly
cadence for field freshness, release health, broken links/downloads, support, reviews, category accuracy,
competitors, media, pricing, integrations, and security incidents.

Track profile impressions/views where exposed, SourceForge referral sessions, CTA clicks, trials/demos/signups,
downloads by file/version/platform, update adoption, review volume/recency, response time, support load, and
downstream conversion. Use privacy-safe UTMs and first-party events; never scrape reviewer identities.

## Step 11: Validate and hand off

Read `references/artifact-templates.md`, write every applicable artifact, and verify:

- route and eligibility verdict are explicit
- duplicate and authority gates pass
- browser evidence contains exactly five relevant pages per active route
- ordinary-blocked targets were retried with `$browse-stealth`
- promoted placements are separated
- every live field and visible limit is captured
- categories, claims, pricing, license, release files, and reviews are truthful
- public URLs, media, downloads, and mobile/desktop display work
- private data is absent

Final verdict must be one of `READY TO SUBMIT BUSINESS LISTING`, `READY TO CREATE PROJECT`,
`READY TO SUBMIT BOTH LINKED ROUTES`, `LIVE — OPERATIONS ACTIVE`, or `NOT READY — BLOCKERS REMAIN`.

Never submit, publish, upload a release, enable invitations, buy a plan, or contact users without the user's
explicit approval.
