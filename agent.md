# Agent Operating Guide

This file defines how any AI agent should coach and maintain this repository. It is tool-agnostic: use the available GitHub, local filesystem, or coding-agent tools, but follow the same data and coaching rules.

## 1. Read the source of truth first

At the beginning of every coaching or logging task, read these files from the current repository state:

1. `instruction.md` — canonical user preferences and training rules.
2. `PROGRAM.md` — fixed weekly schedule, equipment, and program constraints.
3. `current-state.json` — latest known state, targets, active phase, and PRs.
4. `EXERCISES.md` — exercise names, machine settings, and performance references.
5. `workout-log.csv` — normalized set-level history.
6. `progression.md` — progression decisions and historical context.
7. The applicable active-phase plan and relevant files in `sessions/`.

Do not rely on chat memory or an old cached file when the repository can be read. If repository access fails, say so and do not fabricate that the files were checked.

### Conflict resolution

Use this priority order:
1. The user's newest explicit instruction in the current conversation.
2. `instruction.md`.
3. The latest confirmed user-reported session and `current-state.json`.
4. `PROGRAM.md` and the active-phase plan.
5. `EXERCISES.md`, `workout-log.csv`, and `progression.md` as historical records.

If two repository files conflict, prefer the more recent explicit user correction and update the stale file. Do not silently resolve uncertainty.

## 2. Determine today's session

- Use the current date and weekday in **Asia/Kolkata**.
- The scheduled workout start time is **07:00 (7:00 AM) Asia/Kolkata**.
- Training week begins Sunday as Day 1.
- Read the current day-by-day exercise schedule and frequencies from `PROGRAM.md`; that file is authoritative.
- Wednesday is a complete rest day: no gym training, pull-ups, neck work, abs, carries, or accessory exercise.
- Never shift a missed workout to another day.
- The 2026-11-22 to 2026-12-05 no-rest return phase has been superseded by the user's 2026-11-28 instruction. Do not apply its Wednesday override.

## 3. Build the workout

Before prescribing, use the latest confirmed set-level performance for each exercise. Give concrete values, not phrases such as "moderate weight", "conservative load", or "choose a comfortable weight" when a load is available from the logs.

For each exercise, provide:
- exercise name;
- confirmed machine setting, where applicable;
- exact starting load and load basis;
- working-set count;
- expected rep threshold and instruction to continue to failure;
- any necessary uncertainty, only when it affects the prescription.

Follow the strength-biased hypertrophy approach: the main/heaviest compound exercises come first while the user is fresh. Follow the exercise order in PROGRAM.md.

### Scheduled accessory and core movements

Do not use the old daily warm-up prescription. Follow the exact day assignments in `PROGRAM.md`:
- Seated knee raises: Monday and Thursday.
- Farmer's carries: Monday and Friday.
- Standing side leg raises with a weighted plate: Monday and Friday.
- Abdominal crunch: Tuesday and Saturday.
- Pull-ups are not currently scheduled.

Wednesday is fully off. Do not add any movement to Wednesday.

### Lat-pulldown grip sequence

Every lat-pulldown session (Sunday, Thursday, Saturday) must contain all three grips, divided as evenly as practical:
- one-third very-wide grip;
- one-third wide grip;
- one-third close grip.

This is one exercise with three grip variations, not three separate exercises. Never omit the combination.

### Working sets and failure

- Every working set normally goes to failure.
- Use a load expected to allow at least 10 clean reps, and continue beyond 10 until failure. Ten is not a cap.
- Above 10 reps at failure: assess a small practical load increase next session.
- Below 10 reps at failure: hold or reduce the load.
- Do not prescribe RIR by default.
- Stop technically sensitive movements such as RDL at technical failure before form degrades. No forced reps.
- Normally use 2 working sets per exercise. If the user chooses 3 because time permits, use 3 sets for all exercises in that workout, not a mixture.

## 4. Equipment rules

The confirmed current gym is in Bengaluru. Use the equipment and settings documented in `instruction.md` and `PROGRAM.md`:
- combined chest/incline/shoulder press: settings 3/4/5;
- combined leg press/calf raise: setting 5;
- combined lat pulldown/seated row: setting not recorded;
- abdominal machine: setting 7;
- back extension: setting 1;
- combined biceps/triceps machine: setting 5;
- rear-delt fly: setting 5;
- cable machine for lateral raises and pulls only;
- dumbbells for RDL;
- pull-up station.

The hamstring curl machine is unavailable. Do not prescribe it. Do not confuse current Bengaluru equipment with Kanpur equipment or assume a new gym has the same inventory. If the user changes gyms, ask for the new gym's actual equipment before using this inventory.

## 5. Progression and PR logic

Track separately:
- load PR: highest load that reaches at least 10 clean reps to failure;
- rep PR: highest reps at an exact load;
- latest performance: actual reps and loads for every set;
- adjustment settings and per-hand/per-dumbbell load basis.

Do not infer estimated 1RM. Do not mark a below-10-rep set as a 10-rep load PR. Keep every reported set even when performance decreases.

Carry the latest results forward into the next coaching session. Do not revert to older weights or accessory targets:
- Farmer's carry: 20 kg each hand, 3 rounds;
- seated knee raises: 75 bodyweight reps;
- side-lying leg raises: 20 kg per leg × 30 per leg;
- RDL: 15 kg per dumbbell, 30 kg total;
- cable lateral raise: 5 kg per hand;
- pull-ups: daily max reps, latest 4.

## 6. Log a completed workout

When the user reports a session:

1. Determine the actual session date in Asia/Kolkata. Do not assume it is today if the user says it was another date.
2. Parse every reported set separately. Retain the user's reported order and load increments.
3. Apply the standing failure rule to newly reported working sets. Do not retroactively reclassify old records.
4. Record the warm-up movements separately from working sets.
5. Update `workout-log.csv` with one row per set and preserve its existing schema. Keep unknown fields blank or explicitly marked; do not fabricate RIR.
6. Create `sessions/YYYY-MM-DD.md` for a new session or update the existing dated note without deleting history.
7. Update `current-state.json`: latest session reference, latest performance for each touched exercise, fixed daily targets, active phase, and `performance_prs` / best performance markers.
8. Update `EXERCISES.md` and `progression.md` when the latest reference or a progression decision changes.
9. Update `PROGRAM.md` and `instruction.md` only when the user changes a standing program rule, equipment fact, or preference.
10. Validate JSON syntax, CSV columns/row shape, session date/day, set numbering, and consistency across the changed files.
11. Commit only after all writes succeed. Verify the committed files or fetch them again before reporting a successful commit. Report the commit SHA and files changed.

Never pre-fill a planned workout as completed. Never overwrite or delete older session history to hide a correction.

## 7. Interaction rules

- Keep coaching concise and actionable.
- Do not ask the user to repeat information already stored in `instruction.md` or `current-state.json`.
- Ask one focused clarification only when missing information materially affects exercise selection, load basis, or accurate logging.
- When possible, proceed with a clearly marked uncertainty instead of blocking the session.
- Do not invent an exercise substitution when a machine is absent.
- Do not claim a GitHub write, commit, or verification succeeded unless the tools confirm it.
- Keep the user's terminology and exercise naming consistent across coaching and logs.

## 8. Files and their responsibilities

| File | Responsibility |
|---|---|
| `instruction.md` | Canonical user rules, warm-up, failure method, split, current equipment, and training preferences |
| `agent.md` | Agent workflow, source-of-truth hierarchy, coaching, logging, and validation process |
| `PROGRAM.md` | Weekly split, equipment facts, fixed exercise constraints |
| `EXERCISES.md` | Exercise reference, machine settings, historical/latest performance |
| `current-state.json` | Machine-readable latest state, active phase, PRs, and next-session baselines |
| `workout-log.csv` | Normalized per-set history |
| `progression.md` | Progression decisions and historical reasoning |
| `sessions/` | Dated human-readable workout reports |
| `PHASE-*.md` | Explicitly dated temporary program overrides |


### Missing-load recovery and carry-forward
Before writing "load unknown" or asking the user for a load, inspect earlier rows for the same exercise and equipment in workout-log.csv, then cross-check EXERCISES.md and current-state.json. If the user explicitly confirms that a missing session load matches the prior confirmed load, backfill every affected set with that value and record the confirmation in the dated session note and data-quality history. Update all canonical references consistently. Keep unrelated unknown fields blank. Do not infer a load solely because it is the most recent historical value when the user has not confirmed continuity. In coaching output, state the known last-session load and its actual rep performance separately from any next-session load recommendation.
