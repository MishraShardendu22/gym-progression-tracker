# Gym Progression Tracker

Private source of truth for the user's gym program, workout logs, exercise settings, and progression decisions.

## Operating rules for the assistant
- Scheduled workout start time: **07:00 (7:00 AM), Asia/Kolkata**, on every scheduled training day.
- Before prescribing or logging a session, read `PROGRAM.md`, `EXERCISES.md`, `current-state.json`, and the relevant session logs.
- After the user reports a workout, record only details actually supplied. Never fabricate dates, loads, reps, machine settings, warm-up/working classification, or RIR.
- Commit updates to this repository when GitHub tools are available. Use descriptive commit messages and preserve historical records.
- Treat this repository as the canonical workout record; chat memory is only a convenience. In a new chat, fetch the repository before relying on prior numbers.
- Separate machine adjustment settings from weight-stack load. For dumbbells, specify whether load is per hand or total whenever known.
- Mark ambiguous or conflicting historical values as uncertain; do not silently resolve contradictions.
- Follow the user's failure-based loading method: choose the heaviest practical load that permits at least 10 clean reps, continue past 10 until failure, and log actual reps. If failure occurs above 10, evaluate the smallest practical load increase next session; if below 10, hold or reduce. Do not stop sets at 10 or prescribe RIR by default.
- The full equipment inventory below is confirmed available in the current Bengaluru gym. Do not incorrectly classify chest/incline press, lat/row, abs/back, biceps/triceps, rear-delt or cable equipment as Kanpur-only. Continue to exclude only explicitly unavailable equipment such as the hamstring curl machine.
- The training week starts on Sunday as Day 1. Sunday is Chest + Legs + Hamstrings. Wednesday is the full rest day. Never move the schedule to compensate for a missed session.
- The user's warm-up is seated knee raises, Farmer's carries, and side-lying leg raises. Pull-ups are also performed daily as a separate max-rep exercise. Do not add separate cardio, ramp-up sets, or generic warm-up blocks unless requested.
- Carry forward updated loads and rep targets from the latest session. Do not revert to older baselines: current targets include 20 kg each hand for Farmer's carries, 75 bodyweight seated knee raises, and daily max-rep pull-ups (4 reps latest).
- Do not infer that a missing exercise was completed. Ask when required data is ambiguous.

## Operating documents
- `instruction.md`: canonical user training rules and preferences.
- `agent.md`: tool-agnostic instructions for any AI agent coaching and maintaining this repository.

## Files
- `PROGRAM.md`: weekly split and fixed constraints.
- `EXERCISES.md`: equipment/settings and known performance records.
- `current-state.json`: latest known reference state.
- `workout-log.csv`: normalized per-set log.
- `sessions/`: human-readable session notes, one file per session.
- `progression.md`: progression rules and decision history.

## Data quality
Historical records include some inconsistent or unclear entries. Uncertain values are explicitly marked and should be confirmed before being used for precise progression decisions.
