# launch-on v1.0.0

`launch-on` gives Claude Code and Codex the same twelve workflows for preparing and running grounded,
platform-compliant product launches.

## Skills TOC

| Skill | Purpose |
|---|---|
| `launch-g2` | Get listed, build a stellar buyer-facing profile, collect compliant reviews, and operate G2 as a sustained trust channel |
| `launch-g2-digital-markets` | Complete the shared listing for Capterra, GetApp, and Software Advice, benchmark the category, and grow authentic reviews |
| `launch-alternativeto` | Pass the seven-day account gate, submit a complete listing, map true alternatives, and grow organic discovery |
| `launch-trustpilot` | Claim the right business profile, derive content requirements from five live category leaders, and run a compliant review program |
| `launch-sourceforge` | Choose the commercial or open-source route, benchmark five live peers, complete every profile field, and operate listings, downloads, releases, and reviews |
| `launch-product-hunt` | Prepare the listing, launch plan, outreach, readiness gate, and post-launch follow-up |
| `launch-hacker-news` | Prepare a compliant Show HN post and thread runbook with no vote mobilization |
| `launch-x` | Write and run an X launch thread with the product link in a reply |
| `launch-linkedin` | Write and run a LinkedIn launch with the product link in the first comment |
| `launch-copy` | Create grounded launch copy across multiple angles and platform constraints |
| `launch-outreach` | Build compliant audience segments, messages, and launch-day outreach plans |
| `launch-analytics` | Add consistent UTMs, conversion events, validation, and launch attribution |

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

The five directory/review workflows and four platform runners create durable launch packages under
`.ulpi/launch/<channel>/`. They compose the bundled copy, outreach, and analytics skills while enforcing
each platform's mechanics and policy.
Shared product positioning lives at `.ulpi/launch/positioning.md` so every channel uses the same grounded
source of truth.

The skills use the [`browse`](https://github.com/ulpi-io/plugin-browse) plugin to inspect live products and
verify current platform details. G2, G2 Digital Markets, AlternativeTo, Trustpilot, and SourceForge require it
for top-five benchmarks. If a site blocks normal browser automation, the workflow switches to the bundled
`browse-stealth` Camoufox runtime; unresolved IP-reputation blocks remain explicit live-research blockers.

## Repository layout

```text
.claude-plugin/plugin.json  Claude Code plugin manifest
.codex-plugin/plugin.json   Codex plugin manifest and catalog interface
skills/                     Shared skill implementations
```

## License

MIT © [ulpi.io](https://github.com/ulpi-io)
