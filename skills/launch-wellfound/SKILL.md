---
name: launch-wellfound
description: |
  Build and operate an eligible Wellfound startup employer presence. Covers live route verification, employer identity,
  jobs, candidate-facing company content, recruiting operations, paid-versus-free hiring products, privacy, and
  measurement. Use when a startup is hiring or assessing whether Wellfound currently offers an appropriate company
  profile; do not use it to invent a generic directory listing.
---

<EXTREMELY-IMPORTANT>
1. VERIFY THE LIVE PRODUCT BEFORE PROMISING A LISTING. The observed July 23, 2026 Wellfound site is a startup hiring
   platform: it promotes employer job posts, applicant management, AI sourcing, and managed recruiting. Do not assume
   the legacy generic startup-directory/company-profile route still exists or is open to the product.
2. REQUIRE A REAL EMPLOYER/HIRING USE CASE. Use the employer route only for an authorized company with a genuine role,
   honest company facts, an accountable hiring owner, and lawful candidate-data handling. If the company is not
   hiring and there is no current public company-profile route, output `NOT ELIGIBLE — NO CURRENT LISTING ROUTE`.
3. BROWSE THE LIVE FLOW AND FIVE PEERS. Use `$browse` to inspect the current employer/signup/job flows and exactly
   five comparable startup employer pages or job posts when publicly accessible. Use `$browse-stealth` for challenges;
   document any unresolved gate instead of inventing fields or observations.
4. NEVER MISREPRESENT JOBS OR COMPANY FACTS. No phantom openings, salary/equity ranges, locations, remote policy,
   immigration status, benefits, team size, funding, customers, traction, or technical claims. Never use hiring
   content as a disguised backlink campaign.
5. PROTECT CANDIDATE DATA. Do not scrape/export candidate identities, credentials, protected characteristics, or
   private application data. Define access controls, retention, deletion, equal-opportunity requirements, and
   candidate-contact consent with the responsible employer.
6. SEPARATE FREE FROM PAID PRODUCTS. The public site says job posting/ATS is free and AI sourcing, managed recruiting,
   and promoted visibility may be paid. Verify current entitlement, cost, labels, and terms; do not imply paid reach
   is organic or guaranteed.
7. REQUIRE HUMAN APPROVAL. Never create an account, post/change a role, message a candidate, purchase a product,
   or export data without explicit user approval.
</EXTREMELY-IMPORTANT>

# Launch on Wellfound

## Goal

Create `.ulpi/launch/wellfound/` with `ROUTE-AND-ELIGIBILITY.md`, `EMPLOYER-PROFILE.md`, `JOB-PACKAGE.md`,
`BENCHMARK.md`, `RECRUITING-OPERATIONS.md`, `PRIVACY-AND-COMPLIANCE.md`, `CHECKLIST.md`, `analytics.md`, and
shared positioning.

## Workflow

### 1. Resolve route

Ask for company URL/name, hiring status, actual open roles, hiring locations/remote policy, employer owner, company
facts, candidate-data owner, existing Wellfound URL, and recruiting budget. Browse the live company flow and return
`EMPLOYER PROFILE + JOBS`, `CLAIM/UPDATE`, `PAID RECRUITING EVALUATION`, or `NOT ELIGIBLE — NO CURRENT ROUTE`.

### 2. Benchmark five live peers

Capture five comparable hiring companies/job posts plus their official careers sites. Record company positioning,
role title/level, responsibilities, must-have/nice-to-have criteria, location/remote rules, salary/equity disclosure
where public, benefits, recruiting CTA, employer proof, and candidate objections. Do not copy job text. Classify
surfaces `LIVE-FORM`, `CATEGORY BASELINE`, `RECOMMENDED`, `PLATFORM-GENERATED`, `PAID`, or `NOT APPLICABLE`.

### 3. Prepare truthful employer and job content

Create evidence-backed company narrative, mission, product/team context, locations, working model, hiring contact,
legal entity/EEO language where applicable, and per-role title, mission, work, requirements, compensation only when
approved, location, benefits, application flow, and recruiter owner. Explicitly distinguish company profile facts
from job-specific promises. Capture every live account/job form field in exact order before submission.

### 4. Operate safely

Configure job review, response SLA, candidate communication templates, rejection/withdrawal process, privacy notice,
data retention/access controls, and accommodation/escalation owner. Measure qualified applies, interview rate,
offer/acceptance rate, time to fill, source quality, candidate experience, and spend separately for free jobs, AI
sourcing, promoted visibility, and managed recruiting. End `READY TO CREATE EMPLOYER PRESENCE`,
`READY TO POST APPROVED JOBS`, `LIVE — HIRING OPERATIONS ACTIVE`, or `NOT ELIGIBLE — NO CURRENT LISTING ROUTE`.

