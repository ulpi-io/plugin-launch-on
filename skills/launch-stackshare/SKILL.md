---
name: launch-stackshare
description: |
  Create, claim, optimize, and operate a StackShare developer-tool profile and, where truthful, a company tech
  stack. Requires live five-peer browser research, accurate category/features/integrations/alternatives, official
  ownership verification, community-safe adoption, and measurable developer conversion. Use when a developer-tool,
  API, cloud, data, DevOps, or engineering SaaS vendor wants to establish or improve its StackShare presence.
---

<HUMAN-WRITING-RULES>
For every user-facing prose artifact produced by this skill, run the full embedded-mode process in `../../references/human-writing.md` before finalizing. Its no-fabrication rule and all 33 pattern checks are mandatory; preserve the intended platform voice and do not alter code, structured data, link targets, quotations, titles, or proper names.
</HUMAN-WRITING-RULES>

<EXTREMELY-IMPORTANT>
Treat these rules as blocking:

1. CHOOSE THE RIGHT ROUTE. A tool profile represents a real developer-facing product. A company stack represents
   tools the company genuinely uses. Do not create a company stack that falsely claims customers, employees, or the
   vendor uses the product; do not list a service, consultancy, renamed duplicate, unreleased feature, or wrapper as
   an independent tool.
2. SEARCH, THEN CLAIM OR CREATE. Use `$browse` to search product/company names, spelling variants, former names,
   official site, GitHub, category, alternatives, and comparison URLs before adding anything. Claim/correct an
   existing profile instead of making a duplicate.
3. BROWSE EXACTLY FIVE LIVE COMPARABLES. Before choosing a category or drafting copy, inspect the target category
   and exactly five live comparable tool profiles, plus official sites and a relevant comparison/alternatives page.
   Search snippets do not meet this gate.
4. USE `$browse-stealth` WHEN BLOCKED. Start with normal browse. On a challenge/403, load `browse-stealth` and retry
   in headed Camoufox. If it is still IP-blocked, record the evidence and require the permitted handoff/proxy; leave
   `BLOCKED — LIVE TOP-FIVE BROWSE REQUIRED`. Never invent benchmark observations.
5. CLAIM ONLY AS THE OFFICIAL TEAM. StackShare says claiming via a domain email or qualifying GitHub permissions
   gives a verified badge. Never claim a tool without authority or give credentials to the agent.
6. DO NOT MANIPULATE COMMUNITY SIGNALS. Never buy, fabricate, coordinate, or ask employees/customers to falsely
   add a tool to stacks, follow, vote, write pros/cons, post a decision, or represent independent adoption. Do not
   seed fake comparisons, discussions, or company stacks.
7. KEEP THE PROFILE PROVABLE. Every product claim, category, feature, pricing/licensing, integration, compatibility,
   security claim, screenshot, video, and competitor relationship needs current first-party evidence. No roadmap,
   private, inflated, or copied claims.
8. PROTECT DATA AND PRESERVE HUMAN AUTHORITY. Do not store credentials, private customer lists, non-public stack
   details, or secrets in artifacts. Never create/claim/edit/publish, invite anyone, or contact StackShare without
   explicit user approval.
</EXTREMELY-IMPORTANT>

# Launch on StackShare

## Goal

Create `.ulpi/launch/stackshare/` containing `ROUTE-AND-CLAIM.md`, `SUBMISSION.md`, `BENCHMARK.md`,
`CONTENT-REQUIREMENTS.md`, `TOOL-PROFILE.md`, `COMPANY-STACK.md` when applicable,
`COMMUNITY-AND-OPERATIONS.md`, `CHECKLIST.md`, `analytics.md`, and shared
`.ulpi/launch/positioning.md`.

## Step 0: Identify the product and route

Ask if unclear:

> Which developer-facing product are you listing on StackShare? Send its canonical URL, product/vendor name,
> intended category, developer buyer/job, official GitHub URL if any, and any existing StackShare tool or company
> profile. Do you also want a company tech stack, and can you prove every tool in it is genuinely used?

Gather canonical names/URLs, owner authority, product maturity, developer job, category, pricing/licensing,
open-source status, supported platforms, API/docs, integrations, proof, approved media, and community owner.
Choose and justify one route:

- `NEW TOOL PROFILE`
- `CLAIM/UPDATE TOOL PROFILE`
- `CORRECT OR MERGE DUPLICATE`
- `COMPANY STACK ONLY`
- `TOOL PROFILE + GENUINE COMPANY STACK`
- `NOT READY`

## Step 1: Load references and perform live research

Read before action:

- `references/routes-claim-and-fields.md`
- `references/benchmark-and-content.md`
- `references/community-operations-and-templates.md`

Use `$browse` and record URL, access date/timezone, observed UI/form fields, and screenshots where useful. Browse
the product site, docs, pricing/licensing, changelog, integration directory, security/legal pages, GitHub if
applicable, and approved asset sources. Recheck any exact form field in the live UI immediately before a human
submits it.

## Step 2: Search duplicates and determine category fit

Search product and vendor variants, prior names, GitHub repository, category listings, tool profiles, and company
profiles. Capture candidate URL, owner signal, mismatch, and action. Choose the narrowest category that matches the
primary developer job—not the broadest category with the largest traffic. List true alternatives: products a buyer
could realistically evaluate for that same job. Use integrations only for real technical connections, not adjacent
brands.

## Step 3: Benchmark exactly five live tool profiles

Open the target category, record its definition and sort/order, then inspect exactly five comparable tools and their
official sites. Also inspect at least one relevant StackShare alternatives/comparison page. In `BENCHMARK.md` capture:

- name, vendor, URL, category/rank where shown, stack/follow/vote counts, and dated evidence
- information architecture: Overview, Discussions, Adoption, Alternatives, Integrations, CTA
- product statement, category wording, key features, pricing/open-source cues, supported platforms, proof, and CTA
- integrations, alternatives, comparison framing, community pros/cons and discussion themes as themes only
- profile completeness, media, claim quality, scanability, and what is vendor-controlled vs community-generated

Then write `CONTENT-REQUIREMENTS.md`. For each surface classify `REQUIRED/LIVE-FORM`, `CATEGORY BASELINE`,
`RECOMMENDED`, `STACKSHARE/COMMUNITY-GENERATED`, `UNAVAILABLE`, or `NOT APPLICABLE`, with source, constraint,
buyer question, and owner. Summarize peer content; do not copy it.

## Step 4: Prepare a tool profile and official claim

Build a paste-ready `SUBMISSION.md` in the exact live form order. The observed public tool pages expose a tool name,
vendor/byline where available, official website/CTA, category, “What is …?” overview, key features, alternatives &
comparisons, integrations, adoption, and discussions; counts such as rank, stacks, followers, votes, pros/cons, and
community decisions are generated surfaces, not vendor claims. Capture all fields revealed by the actual create/edit
flow and mark each `READY TO PASTE`, `SELECT`, `UPLOAD`, `NOT APPLICABLE`, `NEEDS OWNER`, or `BLOCKED`.

Prepare:

- exact product and vendor name, canonical domain, official CTA, one-sentence developer-job statement, full overview
- accurate category and rationale; features with evidence; only supported platforms, pricing/licensing, and OSS URL
- real integrations with docs URL, implementation/use-case note, and evidence
- genuine alternatives/comparisons with buyer-fit distinction and factual differentiation
- square logo, screenshots/video, captions, source, rights, dimensions, secret/PII check, and freshness
- three description angles—developer job, implementation/technical workflow, and proof/reassurance—then recommend
  the best factual, distinctive version

For an existing tool, use `Claim this tool` and choose only an official verification method: domain-email link, or
GitHub repository verification with admin/maintain access for an open-source tool. If neither applies, use the live
support path with proof of official role. Record requirements and outcome; never put verification links or secrets
in the artifact.

## Step 5: Prepare a company tech stack only when true

A company stack is not an advertisement. Include only tools the company actually uses and can safely disclose. Map
each to the live layer/category, technical purpose, evidence source, disclosure owner, and freshness date. Prepare
company name, canonical site, concise engineering-relevant description, genuine stack, team/owner, and a truthful
Dev Feed/decision plan if available. Do not publish internal architecture, credentials, customer stacks, or use of
the vendor’s product unless it is real and disclosed.

## Step 6: Run ethical community and conversion operations

Keep the official listing current; answer community questions only with clear vendor affiliation, useful evidence,
and no PII. Publish technical decisions only from genuine adopters with authority and their own words. Never
incentivize follows, votes, pros, stack additions, or review-like content. Build opt-in developer distribution around
real documentation, integrations, migration guidance, and launch notes—not a coordinated engagement campaign.

Track category/profile referrals, CTA clicks, docs/trial/demo conversion, comparison referrals, verified-claim
status, truthful stack additions, integration-page referrals, and qualified downstream activation with privacy-safe
UTMs and first-party events. Separate observed community signals from vendor-controlled metrics.

## Step 7: Validate and hand off

Before external action, confirm route, duplicate search, exactly-five live browser evidence, live field/limit check,
claim authority, fact sources, media rights, category/alternative/integration fit, no private data, no manipulated
community plan, and explicit human approval. End with one verdict:

- `READY TO CREATE TOOL PROFILE`
- `READY TO CLAIM/UPDATE TOOL PROFILE`
- `READY TO PUBLISH COMPANY STACK`
- `LIVE — OPERATIONS ACTIVE`
- `NOT READY — BLOCKERS REMAIN`

