# Execution Phases

The morning operator MUST execute every phase. No skipping. No reordering.

## Phase A — Context Pull

Read and verify the live state before deciding anything. Cheap reads first.

- Active screen / clipboard / current chat thread (when accessible).
- Active repo(s): branch, `git status`, `git stash list`, recent commits, open PRs.
- Task systems: in-progress items, blockers, recent status changes (Linear, Notion, Asana, ClickUp, etc., per what is connected).
- Alerts, CI, deploys, cron/jobs, uptime, error surfaces, dashboards.
- Inboxes, outreach/application threads: use the inbox skill for complete ID census, later-history reconciliation, final-stage employment versus advanced commerce qualification, separate official public cases, and actual cash-profit calculations.
- Monetization surfaces, experiment surfaces, fraud/legal/evidence surfaces.
- Any live operational risks.

If a connector is missing, log a 1-line substitution and continue. Do not block on tool absence.

## Phase B — Truth Diff

Compare claimed state vs actual state. Find:

- stale claims
- false finishes
- partial closes
- forgotten siblings
- dead branches
- unverified deploys
- orphaned drafts
- status mismatches between code/infra and tracker/dashboard/communication

Reopen, finish, or log each one. Every in-scope diff gets an authorized action or an exact external dependency recorded in the existing native/runtime ledger.

## Phase C — Triage

Rank candidate items by:

1. revenue / downside protection
2. momentum recovery
3. blocker removal
4. blast radius
5. time-to-kill

For earning work, apply qualified stage and supported cash-profit gates first; keep public cases, advanced commerce, obligations, early leads and noncash benefits distinct. A real loss can override action priority without becoming revenue. Pick the top items that fit the authorized scope of this run. Execute now. Do not produce a roadmap or a plan-only output.

## Phase D — Per-Item Loop

For each top item:

1. 1-line diagnosis with evidence (file:line, log line, dashboard delta, message URL).
2. Choose smallest KISS move.
3. Execute.
4. Verify with fresh proof (see proof standard in SKILL.md).
5. Run sibling sweep across code, infra, docs, dashboards, tasks, communication.
6. Ship / deploy / send / update / close.
7. Log 1-line proof.
8. Do obvious cleanup (clear stash, delete dead branch, revert temp flag, remove dead code).

On failure, retain successful state and inspect the precise cause before a materially different supported correction. Keep blockers in existing native/runtime state, with no arbitrary attempt/time cap and no new local tracker. Continue independent work.

## Phase E — Global Sweeps (every morning)

Run all of these. Each may produce additional Phase D items.

- false-finish sweep — items marked done without proof.
- missed-sibling sweep — single-instance fixes that should have been multi-instance.
- stale-claim sweep — docs, dashboards, status pages, marketing claims out of sync with reality.
- no-evidence sweep — recent claims of "fixed/deployed/works" without artifact.
- over-engineering sweep — recent diffs that introduced abstraction where a one-liner would do.
- permission-loop sweep — places where prior runs stopped to ask instead of acting.
- looping-issue sweep — recurring failures that keep being patched superficially.
- unknown-pattern sweep — anything that feels off, drifting, suspiciously quiet, or untouched too long.

## Phase F — Weekly / Suspicion Health Check

Run when due (every 7 days) or when any signal triggers it. Cover:

- dependency drift
- secret age
- backup freshness
- cron liveness
- billing vs usage
- dead feature flags
- broken links
- orphaned branches / stashes
- quiet failures
- stale dashboards
- expiring certs / domains
- degraded momentum
- tool decay

Log findings tersely, route to Phase D when actionable.

## Phase G — Report

Use the format defined in `report-format.md`. Compact. After action only. No preamble.
