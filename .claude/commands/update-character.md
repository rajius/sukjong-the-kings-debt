---
description: File conversation decisions into a character development document
---

You just had a conversation with the user about a character. Your job is to file the decisions made in that conversation into the right character development document. You are a filing clerk, not a co-author.

## Phase 1: Identify the character

`$ARGUMENTS` may contain a character name (e.g., `Lady Yoon`, `Sukjong`, `The Husband`). If empty, infer from the conversation context — look for the most recently discussed character.

Find the matching file in the project root:
- `CHARACTER DEVELOPMENT - <name>.md`
- `ROMANTIC DEVELOPMENT - <names>.md` (if the conversation was about a relationship)

If no file exists for this character, ask the user whether to create one.

## Phase 2: Read the existing file

Read the full character document. Note all existing sections and their content. You need to know what is already there to avoid duplicating it.

## Phase 3: Identify new decisions from the conversation

Scan the conversation above this skill invocation. Extract only **decisions the user confirmed** — things they said "yes" to, corrections they made, details they provided. Ignore suggestions the user rejected or left unanswered.

Categorize each decision:
- **Background** — origin, education, family, formative events
- **Personality / Psychology** — traits, contradictions, fears, drives
- **Relationships** — connections to other characters, dynamics, tensions
- **Plot function** — what the character does in the story, arcs, turning points
- **Physical / Social** — appearance, age, status, bearing
- **Dialogue / Voice** — speech patterns, register, what they would or would not say

## Phase 4: Update the file

For each new decision:
1. Find the section where it belongs (match to existing headings).
2. If the section exists, append the new detail in the same style as existing bullets.
3. If no section fits, add a new subsection under the most relevant parent heading.
4. If the new detail contradicts an existing one, **do not silently overwrite**. Flag both versions and ask the user which to keep.

Use the Edit tool. Preserve the existing file structure and voice exactly. Do not rewrite existing content.

## Phase 5: Report

Print:
1. Character name and file path.
2. Numbered list of decisions filed (one line each).
3. Any contradictions found (with both versions).
4. Anything from the conversation that seemed like a decision but was ambiguous — list for the user to confirm or discard.
