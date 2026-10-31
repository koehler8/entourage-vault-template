# Vault

Your Entourage vault: a plain folder of Markdown notes in a git repo, readable
and editable by hand (Obsidian works well) and by your agents through the vault
MCP tools.

## Layout

The folder names are the product's contract — agents are granted access by path,
so renaming a folder revokes the grant that points at it.

| Folder | What lives here |
|---|---|
| `morning/` `after-work/` `before-bed/` | Daily notes, one `YYYY-MM-DD.md` per day. Created from templates by your agents. |
| `projects/` | One note per project. |
| `decisions/` | One note per decision, `YYYY-MM-DD — title.md`. |
| `topics/` | Evergreen knowledge, one note per subject. |
| `people/` | One note per person. |
| `logs/` | Append-only data surfaces with no editorial voice. |
| `templates/` | Scaffolds for new notes, for you — daily-note templates live in vault config. |
| `attachments/` | Binaries. Filled forms land in `attachments/forms/`. |
| `archive/` | Retired content. **Deliberately outside every agent's read access.** |

Some folders appear only once you install the extension that writes them:
`finance/`, `health/`, `feeds/`, `intel/`, `analytics/`, and `portfolio.md`.

`inbox.md` at the root is the quick-capture drain.

## Archiving

Moving a note into `archive/` removes it from what agents can see, without
deleting anything. Use it for content that is historical rather than wrong —
notes describing systems you no longer run are worse than useless to an agent,
because they read as current.

## Conventions

See `topics/Vault conventions.md` for how content is organized and
`topics/Vault update policy.md` for how much latitude agents have to write here.
