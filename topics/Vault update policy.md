---
tags: [agent, policy, meta]
---

# Vault update policy

How much latitude your agents have to write to this vault. Adjust it to taste —
this note is the contract they are pointed at.

## Default behaviors by action type

| Action | Default |
|---|---|
| Append to today's daily note (small captures, notes-in-flow) | Just do it. One-line trail: *"→ Added to today's daily."* |
| Capture a decision as it is made | Just do it. Announce: *"→ Captured as `decisions/YYYY-MM-DD — title.md`."* |
| Mark follow-ups complete or parked, consistent with a logged decision | Just do it. Trail in the commit message. |
| Small bookkeeping edits to daily notes | Just do it. Trail in the commit message. |
| Change a project's `status` | Announce *before* doing. Proceed unless interrupted. |
| Edit the body of an existing project note | Announce, and show the new content inline so it is reviewable. |
| Create a new project note | Confirm first. |
| Delete, merge, or archive notes | Always confirm. Flag what will be lost from agent view. |
| Promote a recurring pattern to a new topic note | Suggest; do not auto-create. |
| Edit an existing topic note | Announce, and show the change. |

## Principle

Lean toward action on reversible, low-stakes writes; reserve the pause for
creations, deletions, and irreversible changes. **Always leave a one-line
"→ what I did" trail** so nothing is silent.

## Voice

Conversational confirmations break voice flow, so on voice the dial moves one
tier toward action. Say *"just do it"* or *"show me first"* to override for the
rest of a session.
