# Report Format

Compact. After action only. No preamble. No restating the skill. No cheerleading. Bullets > prose. Preserve Sami's lowercase / typo voice in any quoted strings.

## Mandatory sections

```
DONE
- [item] — [proof]
- [item] — [proof]

BLOCKED
- [item] — [exact blocker from BLOCKERS.md] — [next best step already queued]

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
- BLOCKED lines must point at BLOCKERS.md and contain the next best step already queued — never just "stuck".
- PICKED UP UNPROMPTED is for sibling-sweep finds and unknown-pattern catches. If empty, omit.
- NEXT ACTION ALREADY QUEUED is exactly one line. Not a list. The operator already started it.
- Never end the report with a question.
- Never say "done", "fixed", "complete", "shipped", "works" without proof on the same line.
- If a section has zero entries, write `- (none)`. Do not delete the heading except for PICKED UP UNPROMPTED.

## BLOCKERS.md schema

Each blocker line:

```
YYYY-MM-DD HH:MM | <item> | symptom: <…> | last action: <…> | last error: <…> | hypothesis: <…> | next: <…>
```

Append-only. The operator MUST log here before moving on whenever the hard exit-loop trips.
