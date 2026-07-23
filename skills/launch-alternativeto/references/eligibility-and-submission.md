# AlternativeTo Eligibility and Submission

Use this reference for the account gate, product eligibility, duplicate route, and exact live form.

## Contents

- Account gate
- Eligibility
- Common rejection risks
- Duplicate and ownership routes
- Suggest a new application form
- Cost and license classification
- Media contract
- Submission and approval

## Account gate

The current signup and FAQ state that new accounts must be seven full days old before submitting a new app
page. New accounts may vote, comment, and edit existing apps immediately, but those actions must not be used as
promotional spam.

Record:

- account username
- email verification status
- account creation date, time, and time zone
- earliest eligible submission timestamp: creation + 7 full days
- current gate: ELIGIBLE, AGING, or UNKNOWN

The current email signup says usernames cannot be changed later and passwords require at least eight
characters. Mark email, password, and account identifiers private; never store a password in Markdown.

## Eligibility

Required or strongly enforced rules:

- The product supports English.
- A merely announced or closed-beta app is not accepted.
- An open beta may be accepted when access is reasonably available.
- Hardware is generally not accepted as an app, though popular hardware may sometimes be a platform.
- US and Europe are the primary markets; single-country or narrowly local services are often rejected.
- The app provides sufficient value and quality for AlternativeTo users.
- The app has a working official website and is actually available.
- Porn sites are not accepted; sexual-topic apps without hardcore content may be accepted but cannot use
  explicit images.

AlternativeTo admins retain final discretion. Similar existing listings do not guarantee approval because
criteria change and saturated categories receive stricter review.

## Common rejection risks

The current FAQ says AlternativeTo often rejects:

- custom-made services, personal sites/blogs, local newspapers, books/magazines, independent radio
- collections of sounds, ringtones, wallpapers, screensavers, or video playlists
- local/domestic apps and narrowly geo-restricted offers
- low-effort, low-quality, indistinguishable, cloned, or oversaturated submissions
- simple converters, calculators, resizers, croppers, compressors, generators, downloaders, counters,
  solvers, formatters, cleaners, testers, timers, editors, uploaders, URL shorteners, and PDF tools
- temporary email providers, resume/CV or invoice generators, QR/barcode tools, random video chats
- AI tool directories, basic AI tools, AI humanizers, rewriting/headshot/background/watermark tools,
  AI wrappers around LLMs, and collections of simple tools
- guides/tutorials, review/comparison sites, document generators, coloring-page tools
- tests/quizzes, typing tests, coupon sites, numerology, astrology, and tarot tools
- low-quality online/mobile games and products that merely rebundle the same app

Do not hide a risky product behind different wording. Issue `ADMIN REVIEW DISCRETION` with evidence or stop.

## Duplicate and ownership routes

Search AlternativeTo and a search engine using product name, creator, domain, former names, and variants.

If the page exists:

- `Contribute to this page` → `Edit / Update Information` for Platforms, License, Description, Tags, etc.
- `Contribute to this page` → `Report something wrong` for incorrect URL, platform, price, status, or danger
- email `support@alternativeto.net` for developer admin rights with username, app, and ownership proof
- send ownership mail from the product/company domain when possible
- do not submit a duplicate

Name collisions may use a concise functional qualifier, such as product name plus its primary purpose.

## Suggest a new application form

Observed July 23, 2026.

### Main info

| Field | Required | Live guidance |
|---|:---:|---|
| Name | Yes | Official name with correct spelling and letter case |
| Short Description | Not marked | Main purpose; short, preferably one concise sentence |
| Website | Yes | Official website of the app/software; use a clean canonical URL |
| Full Description | Not marked | Longer description written by submitter or taken from official material |
| Supported Languages | English required | Specify actual supported languages; English is mandatory |
| Pricing | Yes | Select current pricing classification from live options |
| Is Opensource? | Verify live state | Answer truthfully; provide repository/license evidence when Yes |

Descriptions must not contain URLs, email addresses, phone numbers, or physical addresses. Dedicated URL fields
exist for websites, stores, and social profiles. AlternativeTo generally does not permit UTM parameters in the
Official Website URL.

### Tags

| Field | Required | Live guidance |
|---|:---:|---|
| Tags | Yes | Add tags used for categories and Application Type |
| Features | Contextual | Select only highlighted features the product actually supports |

Application Types act as a subcategory and describe the app's main purpose. Tags are more generic; Features
describe supported functions/options. The system may convert misclassified tags/features automatically, but
submit them accurately rather than relying on correction.

### Platforms

`Platforms` is required. Use exact live labels.

- For web apps, use only Online and/or Software as a Service (SaaS).
- Add desktop/mobile operating systems only when a native app exists for that platform.
- Browser access from an OS is not native platform support.
- Self-Hosted means users can install/run the app on their own server.
- Custom Platforms reference another app/platform already in AlternativeTo.

### Author / Social Media

| Field | Required | Live guidance |
|---|:---:|---|
| Company / Author | Yes | Select the company or person that created the app |
| X username | No marker | App or company X username |
| Facebook URL | No marker | App or company Facebook URL |

Use product/company social accounts, not an unrelated personal profile. If the company/author selector lacks
the correct entity, inspect the live path for adding or requesting it; do not select a wrong entity.

### Icon & Screenshots

See Media contract below.

### Videos

`Add a new video URL`; YouTube only at present.

### Meta

`Note about your changes` is optional. Use it to explain potentially ambiguous platform, license, naming,
pricing, or alternative decisions and provide concise moderation context. Do not add promotional hype.

### Final action

`Submit the application` sends the entry for admin verification. It is an external state-changing action and
requires explicit user authorization after reviewing the final worksheet.

## Cost and license classification

Current high-level choices include Open Source, Free with limited functionality/Freemium, Free for personal
use, Free, and Commercial. The live form may expose separate Pricing and Open Source controls plus detailed
open-source license families.

Rules:

- Freemium: the free version performs the app's main purpose without payment, with additional paid capacity or
  features.
- Commercial: a trial limited by time, executions, credits, or other major usage cap; or no durable free tier.
- Free: no payment required for the offered product.
- Free for personal use: free only for qualifying personal/noncommercial use.
- Open Source: source and a real license are publicly verifiable; select the exact current license/family.
- Proprietary: source is not offered under an open-source license.

Do not create separate entries for free/pro editions sharing the same main purpose. Use one generic entry and
explain editions in the description where useful.

## Media contract

### Application Icon — required

- JPEG, PNG, SVG, or WebP
- transparent square suggested
- live form suggests 128×128 or larger
- FAQ recommends 280×280 or larger for stronger quality
- upload local file or use `Upload icon by URL`

### Screenshots — strongly expected

- JPEG, PNG, or WebP
- maximum 3 MB per screenshot
- animated screenshots unsupported
- upload local files or use `Upload screenshot by URL`
- submissions missing screenshots may be denied

Use real, current product screens. Remove PII, secrets, internal domains, customer data, and unreleased
features. Record local path, source URL, dimensions, format, bytes, caption, rights, and privacy review.

### Video — optional

- YouTube URLs only in the current form
- public/playable product video
- no misleading or unreleased functionality

## Submission and approval

Track:

1. Account created and email verified
2. Seven-day wait in progress or passed
3. Duplicate/ownership route resolved
4. Form/package ready
5. User authorized submission
6. Submitted for verification
7. Changes requested
8. Approved
9. Public profile verified
10. Developer admin rights confirmed
11. Alternative associations approved

The official FAQ says approval usually takes a couple of days to one week. A submitted page is not approval.
