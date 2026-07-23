# Trustpilot Reviews and Compliance

## Contents

1. Governing rule
2. Eligible review population
3. Prohibited conduct
4. Supported invitation methods
5. Neutral invitation design
6. Privacy and data handling
7. QA and rollout
8. Replies and recovery
9. Flagging and integrity incidents

## 1. Governing rule

Trustpilot's current Guidelines for Businesses are the controlling source:
`https://legal.trustpilot.com/for-reviewers/guidelines-for-businesses`.

The core standard is fair, neutral, unbiased collection through supported methods from people with genuine
experiences. Recheck the guidelines and current account immediately before every new invitation workflow.

## 2. Eligible review population

Write one deterministic rule, for example:

> Invite every customer whose paid or free account completed [real experience event], after [neutral delay],
> once per experience, except documented legal, consent, deliverability, duplicate, or opt-out exclusions.

The event must allow enough experience to form an opinion. It must not be reachable only by satisfied users.
Do not use NPS/CSAT, sentiment, support outcome, refund status, plan, spend, tenure, location, relationship, or
predicted rating to decide who receives a Trustpilot invitation.

Exclude owners, employees, close family, shareholders, competitors, agencies/contractors working with the
business, and anyone else with a conflict of interest. Do not invite test accounts or people without a genuine
experience.

## 3. Prohibited conduct

Never:

- invite only happy customers or suppress dissatisfied customers
- ask for a positive, five-star, favorable, or "supportive" review
- offer discounts, refunds, money, loyalty points, gifts, coupons, contest entries, referrals, or benefits
- condition customer service, refunds, access, or resolution on a review, edit, or deletion
- pressure, threaten, shame, or repeatedly harass reviewers
- write, rewrite, translate into changed sentiment, ghostwrite, or generate review content for a customer
- ask owners, employees, family, shareholders, partners, or competitors to review
- buy reviews or use review farms, shared devices, office kiosks, or coordinated campaigns
- ask customers to review on company equipment; in-premises collection needs Trustpilot's prior permission
- use unsupported invitation links or workflows
- flag reviews simply because they are negative or disputed

Violations can trigger invitation restrictions, loss of Trustpilot designs/widgets, account action, hidden
TrustScore, profile warnings, search-data blocking, termination, or legal action.

## 4. Supported invitation methods

Use only a method currently supported and available in the user's Trustpilot Business account. Depending on
plan and current product, examples may include:

- automated invitations / Automatic Feedback Service
- approved ecommerce, CRM, payment, support, or marketing integrations
- Trustpilot's manual invitation/upload/send tools
- a supported business-generated link or approved API flow

Verify the exact entitlement, monthly allowance, sender controls, reminders, timing, templates, reference data,
and review labels live. Public pricing observed July 2026 advertises 50 automated invitations per month on Free;
this is a volatile plan fact, not a permanent allowance.

Do not build a custom link or external campaign merely because it technically reaches the review form. The
Guidelines say businesses must use supported invitation methods, including when invitations originate outside
Trustpilot.

## 5. Neutral invitation design

Safe baseline email:

~~~text
Subject: Share your experience with [Business]

Hi [First name],

You recently [neutral experience event] with [Business]. We invite customers at this stage to share an honest
review on Trustpilot. Your feedback can be positive, negative, or anything in between and helps other customers
and our team understand the experience.

[Official Trustpilot invitation button/link]

Thank you,
[Business/team]
[Required privacy and preference information]
~~~

Do not add star imagery that preselects positive sentiment, "help us maintain our rating," gift language,
staff performance pressure, or an NPS gate. If a reminder is available, apply it uniformly and respect current
frequency limits and opt-outs.

Use the same neutral logic for SMS and in-app copy. Keep the destination and brand identity unmistakable.

## 6. Privacy and data handling

Before sending, identify:

- lawful basis/consent requirements by market
- data controller and Trustpilot/integration processor roles
- allowed fields and purpose
- privacy-notice coverage
- suppression/opt-out source of truth
- retention/deletion period
- cross-border transfers and vendor agreement where applicable
- security owner and incident route

Minimize customer data. Do not place raw email lists, phone numbers, order IDs, message payloads, or reviewer
identities in repository artifacts. Store schema, counts, owners, and approved system locations instead.

## 7. QA and rollout

Before production:

1. Confirm the cohort query includes all eligible sentiment outcomes.
2. Confirm exclusions are limited to documented compliance/operational reasons.
3. Use internal test identities that do not publish reviews.
4. Verify sender, subject, personalization fallback, destination, branding, and mobile rendering.
5. Verify no duplicate invitations and once-per-experience logic.
6. Verify timing, time zone, frequency cap, reminder, opt-out, and suppression.
7. Verify reference/order data is correct and minimal.
8. Check delivery/bounce/error handling.
9. Obtain privacy and channel-owner approval.
10. Start with a controlled operational batch that is still representative, then reconcile counts.

Do not call a small handpicked happy-customer cohort a pilot. A pilot must be selected neutrally.

## 8. Replies and recovery

Reply principles:

- timely, human, specific, calm, and proportional
- acknowledge the described experience without admitting unverified legal liability
- never reveal personal, account, health, payment, employee, or order details
- explain what can be explained publicly
- offer an official private support route when investigation is needed
- state a concrete improvement only when owned and real
- never demand a rating change or deletion

Templates are scaffolds, not copy-paste automation. Tailor each response.

Critical-review structure:

~~~text
Thank you for raising this, [public display name if appropriate]. We're sorry the experience did not meet the
standard we aim for. We want to investigate [brief issue category] without discussing account details publicly.
Please contact [official private channel] and reference [safe case route]. Our team will review it and follow up.
~~~

Do not imply the reviewer is lying. Do not publish transaction evidence.

## 9. Flagging and integrity incidents

Valid flagging depends on the current guidelines and may include personal information, harmful/illegal content,
advertising/spam, or lack of a genuine experience. A low rating, criticism, competitor mention, or disagreement
alone is not enough.

Create a private evidence record containing:

- profile URL and review ID
- observed date/time and screenshot where permitted
- exact guideline ground
- internal experience lookup and result
- evidence owner and secure location
- flag submission date/status
- Trustpilot decision and appeal route if available

Misuse of flagging is itself prohibited. Maintain service and public response work while Trustpilot evaluates a
flag. For a warning, sudden abnormal pattern, credential issue, data leak, or invitation error, pause affected
automation, preserve evidence, notify legal/privacy/owner roles, and use official Trustpilot support.
