# Gym Progression Tracker

Private source of truth for the user's gym program, workout logs, exercise settings, and progression decisions.

## Operating rules for the assistant
- Before prescribing or logging a session, read `PROGRAM.md`, `EXERCISES.md`, `current-state.json`, and the relevant session logs.
- After the user reports a workout, record only details actually supplied. Never fabricate dates, loads, reps, machine settings, warm-up/working classification, or RIR.
- Commit updates to this repository when GitHub tools are available. Use descriptive commit messages and preserve historical records.
- Treat this repository as the canonical workout record; chat memory is only a convenience. In a new chat, fetch the repository before relying on prior numbers.
- Separate machine adjustment settings from weight-stack load. For dumbbells, specify whether load is per hand or total whenever known.
- Mark ambiguous or conflicting historical values as uncertain; do not silently resolve contradictions.
- Progress conservatively: generally increase reps within the target range first; increase load by the smallest practical increment after all working sets reach the top of the range with sound technique and about 1–2 reps in reserve. Do not assume every set is to failure.
- The training week starts on Sunday as Day 1. Sunday is Chest + Legs + Hamstrings. Wednesday is the full rest day. Never move the schedule to compensate for a missed session.
- Do not infer that a missing exercise was completed. Ask when required data is ambiguous.

## Files
- `PROGRAM.md`: weekly split and fixed constraints.
- `EXERCISES.md`: equipment/settings and known performance records.
- `current-state.json`: latest known reference state.
- `workout-log.csv`: normalized per-set log.
- `sessions/`: human-readable session notes, one file per session.
- `progression.md`: progression rules and decision history.

## Data quality
Historical records include some inconsistent or unclear entries. Uncertain values are explicitly marked and should be confirmed before being used for precise progression decisions.
