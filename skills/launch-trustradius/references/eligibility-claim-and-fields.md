# TrustRadius Eligibility, Claim, and Fields

## Eligibility and identity

List a distinct, available B2B technology product represented by an authorized vendor. Search exact/former
product and company names, domains, spellings, acquisitions, and editions. Claim or request correction instead
of duplicating. Keep company listing and product listing distinct.

## Claim flow

The live July 23, 2026 public claim page offered:

- Free Profile — claim and build a product profile
- Premium Profile — sales/demo path for enhanced vendor capabilities
- Vendor Portal Login

The Free CTA led to a TrustRadius vendor login/signup URL with `nexturl=/vendoradmin`. Authentication may render
through a protected widget. Capture the live signup and claim fields during execution; do not guess hidden
fields or persist credentials/MFA.

## Complete field inventory

After access, inspect `Product Listing` and `Company Listing`. Existing live profiles and the current claim page
show these content families:

- product/company name, logo, canonical website, description
- categories and use cases
- media gallery: screenshots with captions, videos, product demos
- pricing, starting price, price unit/period, contact sales, free option/trial
- category features/capabilities
- integrations and API
- security information
- technical details: deployment types, mobile/OS support
- competitors/alternatives
- company information and FAQs
- website/demo/contact CTA; lead form may be plan-gated

Record exact label, section/order, required state, control/options, value, visible limit, evidence, owner, and
status. Recheck because portal fields and limits are not fully public and change over time.

## Browser fallback

Normal TrustRadius access returned 403 during the July 23, 2026 research run. Headed Camoufox succeeded. Always
try normal `$browse` first, then use `$browse-stealth`. If both fail, require the permitted handoff/proxy and
leave live fields blocked.
