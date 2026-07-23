# SourceForge Routes, Eligibility, and Submission

## Contents

1. Route decision
2. Eligibility
3. Duplicate and ownership checks
4. Business listing request
5. Open-source project creation
6. Live-form capture rules

## 1. Route decision

SourceForge has two materially different listing systems.

| Route | Use when | Do not use when |
|---|---|---|
| Business software | A vendor offers publicly available commercial software to businesses | Consumer-only product, reseller page, consulting/custom work, unreleased offer |
| Open-source project | Public source uses an Open Source Definition-compatible license and needs a project/download page | Merely freeware, closed source, source-available under a non-open license |
| Both linked | The same ecosystem genuinely has an eligible open-source project and a distinct commercial B2B offer | It would duplicate one product or confuse edition/license/pricing boundaries |

Official eligibility and form behavior can change. Re-open the current vendor terms, new-vendor form, project
creation docs, Terms of Use, and privacy notice immediately before submission.

## 2. Eligibility

### Business software

Current vendor terms observed July 23, 2026 require software to be publicly and commercially available to
businesses, submitted by the vendor or an authorized representative, and eligible for at least one SourceForge
category. Record:

- canonical product and vendor sites
- public availability and purchase/contact path
- actual B2B audience and use
- authorization/ownership
- current category evidence
- whether the listing already exists

Do not represent an affiliate, integrator, consultant, reseller, lead-generation page, or custom development
service as the vendor without explicit authorization accepted by SourceForge.

### Open-source project

SourceForge project hosting is for open-source software. Record:

- repository and exact license file
- OSI/Open Source Definition compatibility
- ownership or maintainer authority
- source and binary relationship
- current release and support status
- any bundled dependencies and their notices/licenses

Escalate license ambiguity to qualified legal review; do not guess from repository visibility.

## 3. Duplicate and ownership checks

Search exact names, punctuation variants, vendor/author, canonical/former domains, repository, product editions,
and likely Unixname/URL names. Compare identity, URLs, description, files, maintainers, activity, and reviews.

Prefer claim/access/correction/support over a duplicate. Keep commercial and community pages linked and clearly
named when both routes are legitimate. Never create a fresh listing to escape criticism or an old project history.

## 4. Business listing request

The current initial request at `https://sourceforge.net/software/vendors/new` showed:

### About Your Company

- Your Name
- Email Address
- Company
- Your Title
- Website
- Phone
- Company Founded
- Company Location

### About Your Software

- Software Title
- Logo — square and high resolution is preferred; JPG, GIF, or PNG shown
- Product Description — describe full functionality clearly
- Audience

The page also included acceptance of current terms/privacy and communications. JavaScript may reveal additional
fields. Inspect the entire rendered form and subsequent onboarding; never treat this snapshot as exhaustive.

## 5. Open-source project creation

Current official project documentation observed July 23, 2026 described:

- account/login
- Project Name
- URL name: 3–30 characters, letters/numbers/dashes; a later rename requires support
- selected services/tools
- Create
- possible phone verification for a first project; PIN lifetime was documented as five minutes

Post-create metadata includes Name, Unixname, Home Page, YouTube Video, Short Summary (plain text, one or two
sentences), Full Description (plain text), Support Page, X/Twitter handle, Facebook Page, Project Logo, and
Project Status. Admins can add users/roles and enable tools. A tool's label can be changed; its URL path should
be treated as immutable after creation.

## 6. Live-form capture rules

For every visible field record exact label, section/order, required state, control type, options, character/file
limit, candidate value, source evidence, and status. Count characters deterministically. Mark private identity,
phone verification, passwords, or codes `ENTER DIRECTLY`; never persist their values.

If ordinary `$browse` is blocked, use `$browse-stealth` with headed Camoufox. If it still fails due to IP
reputation, require the permitted user-assisted handoff/proxy route and mark the affected gate blocked.
