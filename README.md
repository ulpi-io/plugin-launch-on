# launch-on v1.0.0

`launch-on` gives Claude Code and Codex the same fourteen workflows for preparing and running grounded,
platform-compliant product launches.

## Skills TOC

| Skill | Platform | Purpose |
|---|---|---|
| `launch-g2` | [G2](https://www.g2.com) | Get listed, build a stellar buyer-facing profile, collect compliant reviews, and operate G2 as a sustained trust channel |
| `launch-g2-digital-markets` | [Capterra](https://www.capterra.com), [GetApp](https://www.getapp.com), [Software Advice](https://www.softwareadvice.com) | Complete the shared listing, benchmark the category, and grow authentic reviews across all three G2 Digital Markets properties |
| `launch-alternativeto` | [AlternativeTo](https://alternativeto.net) | Pass the seven-day account gate, submit a complete listing, map true alternatives, and grow organic discovery |
| `launch-trustpilot` | [Trustpilot](https://www.trustpilot.com) | Claim the right business profile, derive content requirements from five live category leaders, and run a compliant review program |
| `launch-sourceforge` | [SourceForge](https://sourceforge.net) | Choose the commercial or open-source route, benchmark five live peers, complete every profile field, and operate listings, downloads, releases, and reviews |
| `launch-trustradius` | [TrustRadius](https://www.trustradius.com) | Claim or create a complete product profile, benchmark five live category leaders, build authentic long-form reviews, and operate awards, content, and conversion analytics |
| `launch-gartner-peer-insights` | [Gartner Peer Insights](https://www.gartner.com/reviews/home) | Prove enterprise and market-capability eligibility, request a suite-level listing, write Gartner-compliant profiles, source authentic reviews, and operate VoC readiness |
| `launch-product-hunt` | [Product Hunt](https://www.producthunt.com) | Prepare the listing, launch plan, outreach, readiness gate, and post-launch follow-up |
| `launch-hacker-news` | [Hacker News](https://news.ycombinator.com) | Prepare a compliant Show HN post and thread runbook with no vote mobilization |
| `launch-x` | [X](https://x.com) | Write and run an X launch thread with the product link in a reply |
| `launch-linkedin` | [LinkedIn](https://www.linkedin.com) | Write and run a LinkedIn launch with the product link in the first comment |
| `launch-copy` | Shared workflow | Create grounded launch copy across multiple angles and platform constraints |
| `launch-outreach` | Shared workflow | Build compliant audience segments, messages, and launch-day outreach plans |
| `launch-analytics` | Shared workflow | Add consistent UTMs, conversion events, validation, and launch attribution |

The skills share one canonical implementation in `skills/`. Both plugin manifests point to that
directory, so Claude Code and Codex receive the same workflows and references.

## Installation

Launch On is intended for distribution through the
[ULPI plugin marketplace](https://github.com/ulpi-io/marketplace).

### Claude Code

```text
/plugin marketplace add ulpi-io/marketplace
/plugin install launch-on@ulpi
```

### Codex

```bash
codex plugin marketplace add ulpi-io/marketplace
codex plugin add launch-on@ulpi
```

Once published, the plugin resolves directly from this repository. Updating it means pushing here,
not to the marketplace repository.

## How it works

The seven directory/review workflows and four platform runners create durable launch packages under
`.ulpi/launch/<channel>/`. They compose the bundled copy, outreach, and analytics skills while enforcing
each platform's mechanics and policy.
Shared product positioning lives at `.ulpi/launch/positioning.md` so every channel uses the same grounded
source of truth.

The skills use the [`browse`](https://github.com/ulpi-io/plugin-browse) plugin to inspect live products and
verify current platform details. G2, G2 Digital Markets, AlternativeTo, Trustpilot, SourceForge, TrustRadius,
and Gartner Peer Insights require it for top-five benchmarks. If a site blocks normal browser automation, the workflow switches to the bundled
`browse-stealth` Camoufox runtime; unresolved IP-reputation blocks remain explicit live-research blockers.

## Repository layout

```text
.claude-plugin/plugin.json  Claude Code plugin manifest
.codex-plugin/plugin.json   Codex plugin manifest and catalog interface
skills/                     Shared skill implementations
```

## License

MIT © [ulpi.io](https://github.com/ulpi-io)
