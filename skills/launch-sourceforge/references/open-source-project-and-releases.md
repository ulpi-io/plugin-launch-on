# SourceForge Open-Source Project and Releases

## Contents

1. Top-five project benchmark
2. Project metadata
3. Tools and access
4. Files and releases
5. Security and maintenance

## 1. Top-five project benchmark

Use `$browse` on the relevant live directory and exactly five comparable projects. Apply `$browse-stealth` after
a normal-browser block. Record current sort, category, rank, downloads/time window, review count, last update,
and any ad/promoted modules separately.

The Most Popular directory observed July 23, 2026 showed qBittorrent, AutoClicker, XAMPP, PortableApps.com, and
TortoiseSVN among the first five actual projects, with commercial ads interleaved. This is research evidence,
not a permanent benchmark set: always select the current top five relevant to the user's category.

Compare name/tagline, summary, features, samples, categories, license, official site, platforms, languages,
intended audience, UI, programming languages, files/releases, download path, update recency, support/docs,
activity, reviews, and repository/source consistency.

## 2. Project metadata

Prepare:

- Name and immutable-sensitive Unixname/URL name
- Home Page and Support Page
- Short Summary: plain text, one or two concise sentences
- Full Description: plain text, use case, core workflow, differentiators, and project status
- logo, screenshots/project samples, YouTube video, social links
- project status and maintainer identity
- categories, exact license, OS, languages, intended audience, UI, programming languages
- feature list grounded in the current stable release

Keep the listing consistent with README, website, repository, documentation, and package metadata.

## 3. Tools and access

Enable only tools the team will maintain: Files, source control, tickets, discussion, wiki, mailing lists, or
other live options. For each tool record purpose, owner, label, URL path, moderation/support SLA, and backup.
Treat URL paths as immutable. Grant the least privilege required; keep at least two recoverable admins where
appropriate and review access quarterly.

## 4. Files and releases

Every stable release should include:

- clear semantic or documented version and release date
- default recommended download matched to platform when supported
- unambiguous filenames containing version, OS, architecture, and package type
- binaries/installers plus corresponding source archive and license/notices
- release notes: highlights, fixes, breaking changes, security impact, known issues
- install, upgrade, rollback/uninstall, compatibility, and dependency instructions
- SHA-256 or stronger checksums and cryptographic signatures where practical
- SBOM where the project can reliably produce one
- link to documentation, support, issue tracker, and vulnerability-reporting process

Test every artifact from a clean environment. Verify size/hash, signature, executable/notarization status where
applicable, redirect/default-download logic, archive contents, launch/install, upgrade, uninstall, and rollback.

## 5. Security and maintenance

Scan binaries and archives for malware and secrets before upload. Never bundle unrelated software, deceptive
installers, advertisements, miners, or unwanted browser/system changes. Keep signing keys and upload credentials
outside artifacts. Publish a security contact/process and coordinate disclosure.

Define supported versions, release owner, backup owner, support SLA, stale-file policy, mirror strategy, and
project retirement/archive procedure. Monitor broken downloads, false-positive antivirus reports, checksum or
signature failures, compromised maintainer accounts, unexpected file changes, and sudden download anomalies.
