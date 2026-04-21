---
description: File conversation decisions into a scene card or create a new one
---

You just had a conversation with the user about a scene or chapter. Your job is to file the decisions into the right scene card document. You are a filing clerk, not a co-author.

## Phase 1: Identify the scene

`$ARGUMENTS` may contain a chapter number or scene name (e.g., `chapter 5`, `The Cave`, `12`). If empty, infer from the conversation context.

Find the matching file. Check in order:
1. `Scene Cards - THE KING'S DEBT.md` (master scene card file — contains cards for all chapters)
2. `Scene Cards - Chapter <N> Beats.md` (per-chapter beat sheets)
3. `Scene Cards - Revised Chapter Order.md` or `Scene Cards - CURRENT Chapter Order.md`
4. Individual scene files in `drafts/Scene - <name>.md`

If the scene is discussed but has no card yet, create a new card using this template:

```markdown
## Chapter <N> - <Title>

POV:

- [character]

Objective:

- [What does the chapter want?]

Conflict:

- [What resists that want?]

Turn:

- [What changes irreversibly?]

Ending image:

- [What image should the reader leave with?]
```

## Phase 2: Read existing content

Read the relevant scene card file(s). Note what is already documented for this scene.

## Phase 3: Extract decisions from the conversation

Scan the conversation above. Extract only **decisions the user confirmed**. Categorize:
- **POV** — whose perspective
- **Objective** — what the chapter/scene wants
- **Conflict** — what resists
- **Turn** — what changes irreversibly
- **Ending image** — closing visual
- **Beats** — specific moments within the scene (ordered)
- **Dialogue notes** — specific lines or exchanges decided
- **Continuity** — links to other chapters, setup/payoff connections

## Phase 4: Update the file

For each new decision:
1. Find the matching field in the scene card.
2. If the field exists and is empty, fill it.
3. If the field has content, append the new detail (do not overwrite unless the user explicitly superseded the old version).
4. If the decision is a beat, add it to a `Beats:` section in scene order.
5. If the scene card does not exist in the master file, append it at the correct chapter position.

Use the Edit tool. Preserve existing structure.

## Phase 5: Report

Print:
1. Scene/chapter name and file path updated.
2. Numbered list of decisions filed.
3. Any continuity links to flag — if the scene decision affects another chapter, name which one.
4. Anything ambiguous from the conversation — list for the user to confirm.
