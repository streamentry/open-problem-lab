# Project Change Note

Open Problem Lab should preserve important maintainership changes in a lightweight, searchable format.

Use this note for changes that affect review gates, evidence standards, generated outputs, contributor workflow, or problem-pack scope.

## Entry format

```markdown
## PCN-YYYY-NNN — Short name

**Date:** YYYY-MM-DD.

**Change:** One sentence.

**Context:** Why the change was needed.

**Options considered:** Short bullet list.

**Chosen path:** What changed.

**Expected benefit:** What should improve.

**Known cost:** What becomes harder or slower.

**Review trigger:** What would make the project revisit this change.
```

## When to add an entry

Add an entry when a change affects how contributors work or how accepted artifacts are interpreted.

Do not add entries for routine typo fixes, small copy edits, or ordinary issue triage.

## Reviewer guidance

Reviewers should ask for a project change note when a PR changes a policy but the reason would otherwise live only in a PR thread.

## Acceptance test

A future maintainer should be able to understand what changed, why, and what would justify changing it again.
