# G2 eligibility, submission, and category evidence

Verified against official G2 sources on 2026-07-23. Recheck the live form and sources before submission.

## Contents

- Eligibility gate
- Product identity rules
- Duplicate search
- Current submission route
- Category methodology
- Special cases
- Official sources

## Eligibility gate

A software listing should proceed only when all applicable statements are true:

- The offer is a business-to-business software product or eligible service.
- The product is generally available, not alpha or beta.
- The product is associated with a real vendor or an open-source project.
- The seller is a legally registered business with a unique web domain.
- The public website clearly shows what the product does for business users.
- The product or pricing page URL is public, canonical, and specific enough for G2 to verify the offer.
- The submitted product name matches the name on the product website.

G2 excludes B2C-only products. A mixed B2B/B2C product can be represented only for its B2B product and use
case. If the public site does not make the B2B offer clear, fix the site before submitting.

## Product identity rules

- Represent one individually purchasable software product with one profile.
- Do not create separate profiles for tiers, editions, or feature bundles sharing the same core product.
- Do not add keywords, category phrases, marketing claims, or trademark symbols to the profile name.
- Do not create a separate profile for a first-party add-on when its functionality belongs to the core
  product.
- Separately sold extensions or plugins may qualify when they have their own SKU and meet a category's full
  criteria.
- Broad B2B APIs may qualify; narrow APIs are decided by G2 Research.
- Model software and services accurately. A service is primarily delivered through human intervention; a
  software product is primarily delivered through software functionality.

## Duplicate search

Before submitting:

1. Search G2 for the exact product name.
2. Search for the vendor/company name.
3. Search former product names, abbreviations, and spelling variants.
4. Search likely category pages and competitor comparison pages.
5. Check whether the product is listed under a parent vendor or legacy brand.

Record every match in SUBMISSION.md with its URL, name, vendor, claim state, categories, and correctness.
Claim or request correction of an existing profile instead of creating a duplicate.

## Current submission route

Use G2's official Finding or listing a product documentation and follow its Product Submission Form link.
The form route can be dynamic or require authentication, so treat the live form as authoritative.

The live form observed on 2026-07-23 requests these product fields in this order:

1. Product or pricing page URL
2. Product Name
3. Vendor Domain
4. Vendor Name
5. LinkedIn Company Page URL
6. Description of Product
7. Upload a Logo, either as a file or from a web URL
8. Upload Screenshots, each with a Title and Description
9. Whether the submitter works at the company that develops the product: Yes or No
10. Whether the submitter wants to serve as admin for the profile: Yes or No
11. Up to three customer email addresses G2 can contact for a review

The form says SVG gives the best logo result and suggests obtaining a current, high-quality logo from the
product's LinkedIn or X/Twitter profile when needed. Prefer the vendor's canonical brand asset when available;
do not scrape or substitute a logo the vendor does not control.

Prepare the form fields above plus supporting internal evidence for:

- general-availability state
- requested categories
- deployment model
- pricing or trial model
- supporting feature, pricing, documentation, and demo URLs
- submitter identity, business email, title, and relationship to the vendor

The live form says the software product will be conditionally approved after completion and that G2 will
email submission details. Record the resulting email/case identifier and follow its instructions rather than
assuming the public profile is fully approved.

The observed approval screen says an approved profile should become visible within a few minutes, while G2
continues assigning relevant categories and later emails the direct profile URL. Verify each state:

1. submission accepted
2. conditional approval
3. profile approved
4. public profile visible
5. categories assigned
6. direct profile URL received
7. profile claimed and admin access working

Do not start category-performance reporting until the assigned categories and direct URL are verified.

The reviewer-contact fields are optional outreach data, not a shortcut around review policy:

- provide only real customers with sufficient first-hand product experience
- do not select only happy customers
- exclude vendor employees and direct-competitor employees
- confirm the company has an appropriate privacy/legal basis for sharing each email with G2
- do not commit raw customer emails to the repository; enter them directly in G2 or use an approved secure
  system
- document only consent/basis status and a non-sensitive internal customer reference in SUBMISSION.md

The form currently promotes that profiles with at least one review can see an average traffic increase of up
to 200%. Treat this as G2 marketing language, not a forecast, guarantee, or campaign KPI.

The product or pricing page URL should:

- resolve without authentication
- use the canonical HTTPS domain
- land directly on product, feature, or pricing information
- make the B2B buyer and value proposition obvious
- expose enough current functionality or pricing evidence for G2 Research to validate the submission
- avoid temporary campaign URLs, URL shorteners, affiliate links, and generic corporate homepages

For each screenshot prepare:

- the image file
- a short factual title
- a description explaining the workflow and buyer value shown
- confirmation that the image contains no customer PII, secrets, or misleading claims

After G2 approves a new listing, claim it before customizing the profile. G2's current help documentation says
claim review generally takes one to three business days.

## Category methodology

G2 categorizes products by native functionality, not by:

- the job title or audience using the product
- a hypothetical or incidental use case
- competitor category membership
- integrations that supply the missing capability
- future roadmap features

A product must satisfy every inclusion criterion in the category definition. Products appear in child
categories, not taxonomy-only parent categories.

### Evidence table

Create one table per requested category:

| Inclusion criterion | Native support | Evidence URL/artifact | Evidence excerpt | Result |
|---|---|---|---|---|
| Exact current criterion | Yes/No | Public docs, demo, screenshot, or release | What proves it | PASS/FAIL |

Rules:

- Copy criteria from the current category page; do not paraphrase away constraints.
- Prefer public product documentation and current product UI.
- A recorded demo or presentation can support a research request when public documentation is insufficient.
- Mark FAIL if the product cannot demonstrate the criterion now.
- Request the category only if every criterion passes.

### Main category selection

Choose the main category from categories already associated with the product. Prefer the category that best
matches the product's core, independently purchased workflow and current customer use—not merely the easiest
competitive set.

If no defined category fits:

- document the closest relevant Other category, or
- request a new category with market and product evidence.

G2 says a proposed new category is normally evaluated only when the market has at least ten products, and it
first considers improving existing categories.

## Special cases

Escalate to G2 Research instead of guessing when the offer is:

- a mixed software and managed-service business
- an API without a clear standalone business workflow
- an extension, plugin, add-on, or marketplace-only product
- open source with no clear vendor
- a product suite, bundled suite, or recently split/merged product
- sold under a different public brand from the legal entity
- available to consumers and businesses through materially different experiences

## Official sources

- [Finding or listing a product on G2](https://documentation.g2.com/help/docs/finding-or-listing-a-product-on-g2)
- [G2 Research Categorization Methodology](https://research.g2.com/methodology/categorization)
- [G2 Research FAQ](https://research.g2.com/methodology/research-faq)
- [Product Information](https://documentation.g2.com/g2/docs/product-information/)
- [G2 Community Guidelines](https://legal.g2.com/community-guidelines)
