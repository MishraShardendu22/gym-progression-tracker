# Progression Decisions

## Default progression method
Use double progression unless a specific exercise requires another approach. Start with a practical rep range (typically 8–12 for compounds/machines, 10–15 for isolation, 10–20 for abs/calves). Add reps while maintaining consistent technique. When every working set reaches the top of the selected range with around 1–2 reps in reserve, consider a small load increase. Reassess after increases; reps may drop back toward the lower end.

Do not assume the user trains every set to failure. RIR should only be recorded when supplied or explicitly estimated with the user's agreement. Pain, technique breakdown, and unusual fatigue override load progression.

## Historical ambiguities to resolve
1. Chest press: user clarified the same weight/reps as incline press, currently represented as 10 kg × 10, but older entries differ.
2. Incline press: both 10 kg × 10 and 10 kg × 12 appear in historical notes; set type is unclear.
3. Dumbbell RDL: 7.5 kg × 10 recorded, but it is unknown whether this is per dumbbell or total.
4. Several machine records lack clear warm-up/working-set labels.
5. Lat pulldown and seated row machine adjustment settings are unknown.

## Confirmed update: 2026-11-01 Sunday
- Chest press machine setting updated to 3. Latest recorded sets: 11.25 × 10, 15 × 10, 18.75 × 10.
- Incline chest press machine setting updated to 4. Latest recorded sets: 15 × 15, 15 × 15, 15 × 10.
- Dumbbell RDL loads are confirmed as per dumbbell: 7.5 × 10, 10 × 10, 12.5 × 10.
- Leg press setting remains 5. Latest sets: 48.75 kg with reps not recorded, 52.5 × 10, 52.5 × 9.
- Calf raise setting remains 5. Latest sets: 30 × 12, 30 × 12, 30 × 16.

## Update policy
- New confirmed workout data takes precedence over inferred/reconstructed reference values.
- Do not delete old session records to hide corrections. Amend current-state files and append a clear note in the relevant session or progression log.
- Use a separate commit for a workout session or a coherent batch of corrections, with a descriptive commit message.
- If GitHub is unavailable, tell the user and avoid claiming that a commit was made.

## Daily load-coaching protocol
When the user asks what to lift for a given training day, use the latest confirmed session data in `workout-log.csv`, `current-state.json`, and session notes. Recommend a specific starting load for each exercise, retaining the established machine settings and using conservative double progression. If the previous load hit the top of the rep range on all working sets with good form and about 1–2 reps in reserve, recommend the smallest practical increase; otherwise hold the load or adjust downward when needed. Treat old reconstructed values as provisional until confirmed. Ask the user to report completed sets and update the repository only after a successful commit. Sunday is always a full rest day; do not shift the split if a day is missed.

## Confirmed update: 2026-11-02 Monday
- Lat pulldown machine setting remains unknown. Grip-by-grip sequence: 30 kg wide 5, less-wide 5, close 10; 33.75 kg wide 5, less-wide 5, close 5; 37.5 kg wide 5, less-wide 5, close 4. These are recorded as separate sets in the CSV; set type and RIR were not supplied.
- The 37.5 kg pulldown sets fell below the default 8–12 rep range. Do not increase load; use a lower load on the next pulldown session if needed to keep controlled working sets in range.
- Seated row: 37.5 × 10, 41.25 × 13, 45 × 10. The 45 kg set is not evidence for increasing load because the full sequence did not reach the top of the rep range across all sets.
- Abdominal machine setting 7: 45 × 10.
- Farmer's carry: 15 kg each hand, then 17.5 kg each hand. The fixed daily target remains 15 kg each hand.
- Seated knee raises: bodyweight × 50.
- Warm-up/working classification and RIR were not reported; no such labels have been inferred.

