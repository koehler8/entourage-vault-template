---
tags: [meta, conventions]
---

# Vault conventions

How content is organized here. Folders carry the *type* of a note; tags carry
cross-cutting context.

## Folders vs tags

| Layer | Purpose | Example |
|---|---|---|
| **Folder** | What kind of thing this is | `projects/`, `people/`, `decisions/` |
| **Tag** | Cross-cutting context; a note can have several | `[health]`, `[family]`, `[side-project]` |
| **Frontmatter** | Structured metadata | `status: live`, `owner: …`, `relationship: …` |

**No type tags.** `[project]`, `[decision]`, `[person]` duplicate the folder and
are not used.

## Where new content goes

- New idea worth keeping → `projects/<Name>.md`
- Non-trivial decision → `decisions/YYYY-MM-DD — title.md`
- Evergreen knowledge → `topics/<Title>.md`
- A person → `people/<Name>.md`
- Today's captures → the daily notes (`morning/`, `after-work/`, `before-bed/`),
  via your agents
- Follow-ups → `follow-ups.md`, the one list (Open / Parked / Done) — through
  your agents or by ticking a box; the morning note shows what is open
- Anything without a home yet → `inbox.md`

## Naming

- Daily notes and data files: `YYYY-MM-DD.md`
- Decisions: `YYYY-MM-DD — title.md`
- Everything else: Title Case, spaces are fine (`Vertex CMS and SEO.md`)

Links are `[[Note name]]` — resolved by name, not path, so moving a note between
folders does not break them.

## Retirement

Move a note to `archive/` instead of deleting it. `archive/` sits outside every
agent's read access, so archiving genuinely removes it from what agents see
while keeping the history. **A note describing something you no longer do is
worse than no note** — an agent reads it as current.

Machine-written day files older than 90 days belong in `archive/<folder>/YYYY/`. Note the root `archive/` — a nested `feeds/archive/` would still sit inside the `feeds/**` grant and stay visible to agents.

## How agents write here

See [[Vault update policy]].
