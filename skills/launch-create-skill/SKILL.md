---
name: launch-create-skill
description: |
  Create a new custom, research-backed launch-on platform skill from a hunt-list row. Requires live $browse research,
  five existing listings or peer surfaces, platform-specific fields and constraints, README TOC URL/purpose updates,
  hunt-list status, validation, and one dedicated commit/push. Use when extending launch-on to a new platform.
---

<EXTREMELY-IMPORTANT>
1. ONE PLATFORM, ONE DEDICATED SKILL, ONE DEDICATED COMMIT. Read the exact hunt-list row and current repo state first.
   Do not batch unrelated platforms or mark a row done until the skill, README, manifests, validation, commit, and push
   have succeeded.
2. LIVE RESEARCH IS MANDATORY. Use $browse to inspect the platform's current public route, creation/claim route, and
   exactly five relevant existing listings, product pages, company pages, deals, programs, or stories. If normally
   blocked, use $browse-stealth with the existing authorized Camoufox session. Interact visually when a current
   Turnstile is visible; record unresolved blockers, never invent fields.
3. ACCOUNT-GATED FORMS MUST BE OBSERVED AFTER USER AUTHORIZATION. Never create/login, submit, claim, buy, apply,
   message, review, or otherwise change external state without explicit user approval. Use public evidence now and
   instruct the new skill to capture every account-gated field, required marker, limit, and policy after approval.
4. MAKE THE SKILL PLATFORM-SPECIFIC. It must distinguish the platform's actual model—directory, review marketplace,
   employer profile, investor workflow, local listing, community, editorial submission, deal partnership, or
   application. Include eligibility gates, actual required facts/assets, peer benchmark fields, operating rules,
   privacy/commercial constraints, approval gates, outputs, and measurement.
5. MAINTAIN THE REPOSITORY CONTRACT. Update root `README.md` TOC with the exact platform URL and concise purpose;
   increment numeric workflow counts; update both plugin manifests as needed; mark `[x]` in the ignored hunt list only
   after completion. Never stage `.browse/` or `launch-on-hunt-list.md`. Validate and push the skill.
</EXTREMELY-IMPORTANT>

# Create a launch-on platform skill

## Inputs

Request or extract: platform name/URL, hunt-list row, platform type, intended user outcome, product/company context,
known eligibility, potential sensitive/commercial actions, and whether a live authorized browser session exists.

## Procedure

### 1. Inspect current repository truth

Run `git status --short`, read the exact hunt-list row, inspect `README.md`, manifests, `.gitignore`, and 1–2 closest
existing skills. Confirm the next platform has no existing equivalent. Preserve unrelated dirty work.

### 2. Perform live platform research

Use `$browse` on the platform homepage, relevant directory/category, creation/claim route, and exactly five peer
surfaces. Capture: current model; eligibility; public fields; creation/claim/account requirements; content/media;
ratings/reviews; paid/editorial labels; terms/risks; and operational hooks. Use `$browse-stealth` for blocks. Save the
observed date and label account-gated or unresolved information as such.

### 3. Design the skill

Create `skills/launch-<platform>/SKILL.md` and `agents/openai.yaml` using `skill-creator` conventions. Keep the skill
under 500 lines. It must contain:

- precise trigger description and `<EXTREMELY-IMPORTANT>` guardrails;
- mandatory `$browse` and exactly-five-peer benchmark requirement;
- current-route/eligibility logic and state-changing approval rule;
- truthful field/asset requirements and a rule to capture current gated form fields;
- platform-specific review, privacy, fundraising, employment, local-presence, or commercial safeguards;
- required `.ulpi/launch/<platform>/` deliverables; and
- a concise workflow from route resolution through launch operations and measurement.

### 4. Update documentation and tracking

Add one `README.md` TOC row: backticked skill name, clickable platform URL, and concrete purpose. Keep numeric counts
numeric. Update `.codex-plugin/plugin.json` and `.claude-plugin/plugin.json` descriptions/keywords if needed for
discoverability. Mark the platform `[x]` in `launch-on-hunt-list.md` only after all completion checks pass; mark `[-]`
with exact live blocker if research cannot be completed.

### 5. Validate, commit, and push

Run:

```bash
python3 /Users/ciprian/.codex/skills/.system/skill-creator/scripts/quick_validate.py skills/launch-<platform>
python3 /Users/ciprian/.codex/skills/.system/plugin-creator/scripts/validate_plugin.py .
python3 -m json.tool .codex-plugin/plugin.json >/dev/null
python3 -m json.tool .claude-plugin/plugin.json >/dev/null
git diff --check
```

Then stage only `README.md`, both manifests, and the new skill directory; do **not** stage `.browse/` or the ignored
hunt list. Commit `feat: add <Platform> launch skill`, push `origin main`, and verify clean status. Report commit SHA,
live evidence, skill name, README row, validation, and any unresolved platform limitation.

