# Progression Decisions

## Default progression method
Use double progression unless a specific exercise requires another approach. Start with a practical rep range (typically 8–12 for compounds/machines, 10–15 for isolation, 10–20 for abs/calves). Add reps while maintaining consistent technique. When every working set reaches the top of the selected range with around 1–2 reps in reserve, consider a small load increase. Reassess after increases; reps may drop back toward the lower end.

Do not assume the user trains every set to failure. RIR should only be recorded when supplied or explicitly estimated with the user's agreement. Pain, technique breakdown, and unusual fatigue override load progression.

## Historical ambiguities to resolve
1. Chest press: user clarified the same weight/reps as incline press, currently represented as 10 kg × 10, but older entries differ.
2. Incline press: both 10 kg × 10 and 10 kg × 12 appear in historical notes; set type is unclear.
3. Dumbbell RDL: 7.5 kg × 10 recorded, but it is unknown whether this is per dumbbell or total.
4. Several machine records lack clear warm-up/working-set labels.
5. Lat pulldown, seated row, and calf raise machine adjustment settings are unknown.

## Update policy
- New confirmed workout data takes precedence over inferred/reconstructed reference values.
- Do not delete old session records to hide corrections. Amend current-state files and append a clear note in the relevant session or progression log.
- Use a separate commit for a workout session or a coherent batch of corrections, with a descriptive commit message.
- If GitHub is unavailable, tell the user and avoid claiming that a commit was made.

## Daily load-coaching protocol
When the user asks what to lift for a given training day, use the latest confirmed session data in `workout-log.csv`, `current-state.json`, and session notes. Recommend a specific starting load for each exercise, retaining the established machine settings and using conservative double progression. If the previous load hit the top of the rep range on all working sets with good form and about 1–2 reps in reserve, recommend the smallest practical increase; otherwise hold the load or adjust downward when needed. Treat old reconstructed values as provisional until confirmed. Ask the user to report completed sets and update the repository only after a successful commit. Sunday is always a full rest day; do not shift the split if a day is missed.
