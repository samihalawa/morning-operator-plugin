# Report Format

Compact. After action only. No preamble. No restating the skill. No cheerleading. Bullets > prose. Preserve Sami's lowercase / typo voice in any quoted strings.

## Mandatory sections

```
DONE
- [item] — [proof]
- [item] — [proof]

BLOCKED
- [item] — [exact blocker in existing native/runtime state] — [next best step already queued]

PICKED UP UNPROMPTED
- [item] — [why it mattered]

NEXT ACTION ALREADY QUEUED
- [single next action]
```

## Rules

- Every DONE line MUST include fresh proof in the same line. Examples:
  - `commit a1b2c3d pushed; CI green; curl /api/health → 200`
  - `linear ENG-412 moved to Done; screenshot saved at outputs/ENG-412.png`
  - `email to investor@x sent at 09:14; thread id <abc>; logged in notion CRM row 87`
- BLOCKED lines name the exact verified dependency and next actor/action in existing native/runtime state. A queued action is not execution proof.
- PICKED UP UNPROMPTED is for sibling-sweep finds and unknown-pattern catches. If empty, omit.
- Include NEXT ACTION ALREADY QUEUED only when an action was actually queued or started under current authority; otherwise state the real external wait. Do not create a scheduler to fill this heading.
- Never end the report with a question.
- Never say "done", "fixed", "complete", "shipped", "works" without proof on the same line.
- If a section has zero entries, write `- (none)`. Do not delete the heading except for PICKED UP UNPROMPTED.

## Blocker evidence

Keep symptom, exact target, last successful checkpoint, literal failure, tested correction and next actor/action in the existing supported native/runtime ledger. Do not create a BLOCKERS.md or other parallel tracker. A future organic outcome is a real wait, not unfinished agent work; saved configuration never proves an automation ran.
