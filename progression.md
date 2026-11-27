# Progression Decisions

## Current user-specific progression rules

The canonical rules are in [instruction.md](instruction.md). In brief:

- Strength-biased hypertrophy. Prioritize main/heaviest compound movements while fresh, after the user's established warm-up.
- Every working set normally goes to failure. Select the heaviest practical load that permits at least 10 clean reps, then continue past 10 until failure. Ten is not a cap.
- Above 10 reps at failure: assess the smallest practical load increase next session. Below 10: hold or reduce. Do not prescribe RIR by default.
- RDL and other technically sensitive movements stop at technical failure before form deteriorates. No forced reps.
- Normally 2 working sets per exercise. If the user opts for 3, use 3 across every exercise in that workout.
- Warm-up is seated knee raises (75 reps on training days except Wednesday), Farmer's carries (20 kg each hand, 3 rounds on normal training days), and side-lying leg raises (20 kg per leg × 30 per leg daily). Do not add generic warm-up routines.
- Pull-ups are daily max-rep bodyweight work; latest report: 4 reps.
- Carry each new confirmed load and rep target forward. Track load PR and rep PR separately; do not infer estimated 1RM.

## Confirmed Bengaluru equipment

The current Bengaluru inventory is confirmed in [PROGRAM.md](PROGRAM.md) and [instruction.md](instruction.md): combined chest/incline/shoulder press (settings 3/4/5); combined leg press/calf raise (setting 5); combined lat pulldown/seated row; abdominal machine (setting 7); back extension (setting 1); combined biceps/triceps (setting 5); rear-delt fly (setting 5); cable machine used for lateral raises and pulls; dumbbells for RDL; pull-up station. Seated/lying hamstring curl is unavailable. Do not classify the confirmed machines as Kanpur-only.

## Automatic carry-forward

- Farmer's carries: 20 kg in each hand, 3 rounds on normal training days, walking to and fro.
- Seated knee raises: 75 bodyweight reps on training days except Wednesday.
- Side-lying leg raises: 20 kg per leg × 30 reps per leg, daily.
- Pull-ups: daily max clean bodyweight reps, latest 4.
- RDL: 15 kg per dumbbell, 30 kg total.
- Cable lateral raise: 5 kg per hand.
- Use the latest dated set records for every other exercise.

## Historical ambiguities to resolve
1. Earlier dumbbell RDL entries do not always distinguish per-dumbbell from combined load. Latest 2026-11-24 entry remains unspecified.
2. Lateral raise equipment/load convention remains unspecified.
3. Side-lying leg-raise reps on 2026-11-24 may be per leg or total; not confirmed.
4. Farmer's carry distance/time per round was not supplied on 2026-11-24.
5. Historical machine availability from Kanpur/previous gyms is not confirmed for Bengaluru.

## Older reconstructed ambiguities from previous gyms
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

## Daily coaching protocol

Read `instruction.md`, `agent.md`, `PROGRAM.md`, `EXERCISES.md`, `current-state.json`, `workout-log.csv`, and relevant session notes before coaching. Follow the tool-agnostic workflow in `agent.md`. Determine local date/day in Asia/Kolkata. Apply only dated active-phase exceptions. Never shift the weekly split after a missed day.

Use the complete confirmed Bengaluru equipment inventory in `instruction.md` and `PROGRAM.md`. The only explicitly unavailable listed machine is seated/lying hamstring curl. Warm-up is exactly seated knee raises, Farmer's carries, and side-lying leg raises. Pull-ups are also performed daily as separate max-rep bodyweight work.

Follow the user's strength-biased hypertrophy style, failure-based minimum-10-rep method, and 2-or-3-sets-for-all rule. Recommend exact starting loads from latest results. Track load PR and rep PR separately and carry every new confirmed load/rep target forward. Log each set individually and preserve ambiguity. After reported sessions, update the CSV, current state, exercise references, progression notes, and dated session file. Verify GitHub writes before reporting a commit.


## Confirmed update: 2026-11-02 Monday
- Lat pulldown machine setting remains unknown. Grip-by-grip sequence: 30 kg wide 5, less-wide 5, close 10; 33.75 kg wide 5, less-wide 5, close 5; 37.5 kg wide 5, less-wide 5, close 4. These are recorded as separate sets in the CSV; set type and RIR were not supplied.
- The 37.5 kg pulldown sets fell below the default 8–12 rep range. Do not increase load; use a lower load on the next pulldown session if needed to keep controlled working sets in range.
- Seated row: 37.5 × 10, 41.25 × 13, 45 × 10. The 45 kg set is not evidence for increasing load because the full sequence did not reach the top of the rep range across all sets.
- Abdominal machine setting 7: 45 × 10.
- Farmer's carry: 15 kg each hand, then 17.5 kg each hand. The fixed daily target remains 15 kg each hand.
- Seated knee raises: bodyweight × 50.
- Warm-up/working classification and RIR were not reported; no such labels have been inferred.

## Confirmed update: 2026-11-03 Tuesday
- Shoulder press setting 5: 15 kg x 10, 15 kg x 8.
- Rear-delt fly setting 5: 33.75 kg x 12, 37.5 kg x 10, 45 kg x 5.
- Cable lateral raise: 2.5 kg each hand x 10, then 5 kg each side x 10. The exact cable loading convention is recorded as reported.
- Leg press setting 5: 52.5 kg x 20, 60 kg x 21, 63.75 kg x 21.
- Calf raise setting 5: 30 kg x 23, 33.75 kg x 21, 37.5 kg x 23.
- Dumbbell RDL: 12.5 kg x 10, 15 kg x 10, 15 kg x 10. Per-dumbbell versus combined load was not specified; do not assume.
- Seated knee raises: bodyweight x 50.
- Farmer's carry: 17.5 kg each hand, 2 rounds. This becomes the standard farmer's carry target on every training day, replacing 15 kg each hand.
- Warm-up/working classifications and RIR were not supplied.
- Coaching calibration: the prior prescriptions materially undershot the user's demonstrated loads and repetitions. Future working-load recommendations must use these latest performances rather than treating old lower reference loads as current targets. Distinguish warm-up loads from working loads and do not label challenging demonstrated loads as easy.


## Confirmed update: 2026-11-05 Thursday
- Biceps curl setting 5: 37.5 kg x 7, 37.5 kg x 5, 37.5 kg x 4.
- Triceps setting 5: 37.5 kg x 5, 37.5 kg x 6, 37.5 kg x 3.
- Chest press setting 3: 22.5 kg x 30, then 26.25 kg x 10 and 26.25 kg x 10 (26.25 kg reported as 22.5 + 3.75).
- Incline chest press setting 4: 18.75 kg x 10 for three sets (reported as 15 + 3.75).
- Farmer's carry: 17.5 kg each hand for 2 sets, walking to and fro inside gym.
- Seated knee raises: bodyweight x 50.
- Warm-up/working classifications and RIR were not supplied. Chest press 22.5 kg x 30 is recorded literally as reported; confirm if 30 reps was intended.


## Temporary return-to-training phase: 2026-11-22 to 2026-12-05
- The user reports five gym visits during a two-week hometown break, with a maintenance rather than strength-gain objective. The final hometown session used two sets per exercise. The user confirms lateral raises and seated rows stayed at the same loads across the hometown sessions. Dates, complete exercise coverage, exact machine identities, and all individual sets are not established. Do not fabricate session dates or add these sessions to workout-log.csv.
- A 14-day return-to-training phase runs Sunday 2026-11-22 through Saturday 2026-12-05. The user explicitly requests no rest days during this temporary phase. The regular Wednesday full-rest rule is temporarily replaced by low-stress active recovery on 2026-11-25 and 2026-12-02. This override expires after 2026-12-05.
- Normal lifting days use two working sets per exercise, week 1 around 3 RIR and week 2 around 2–3 RIR. Wednesday active recovery is easy cardio/mobility only, no hard sets. Do not chase PRs or force load increases.
- User explicitly sets Farmer's carries to 15 kg in each hand, walking to and fro inside the gym, every training day. Use two rounds on normal lifting days and at most one easy round on Wednesday if comfortable. This is a temporary explicit override of the older 17.5 kg repository baseline.
- Seated knee raises remain bodyweight × 50 every day except Wednesday.
- Detailed 14-day prescription, conservative starting loads, warm-ups, and return to the permanent split are in PHASE-2026-11-22-to-2026-12-05.md.
- Resume the fixed six-training-days/one-full-rest-day schedule on Sunday 2026-12-06. Do not shift days after missed sessions.


## Confirmed update: 2026-11-22 Sunday
- Chest press setting 3: 26.25 kg (22.5 + 3.75) x 17, then x 16.
- Incline chest press setting 4: 18.75 kg (15 + 3.75) x 12, then 22.5 kg x 10.
- Wide-stance leg press setting 5: 63.75 kg (60 + 3.75) x 17, then x 9. This is the first explicitly recorded wide-stance session. Future sessions should use the name Wide-stance leg press; historical leg-press records remain stance-unspecified.
- Dumbbell RDL: 12.5 kg x 12, then 15 kg x 7 to failure. Per-dumbbell versus combined load was not specified.
- Back extension setting 1: 41.25 kg (37.5 + 3.75) x 10 and x 9.
- Farmer's carry: 17.5 kg each hand x 2 rounds, walking to and fro inside gym.
- Seated knee raises: bodyweight x 50.
- Set classifications were not supplied. RIR was not supplied except the second RDL set was explicitly to failure.
- Wide stance generally shifts emphasis toward the gluteal muscles and hip adductors; it should not be described as activating more muscles universally. Keep stance, depth, and foot placement consistent when comparing progression.


## Confirmed update: 2026-11-23 Monday
- Side-lying leg raises (side-lying hip abduction) are now a daily fixed exercise, including rest days. User confirmed this was intended as an everyday exercise.
- Completed today: 10 kg per leg x 20 reps per leg. Use this as the latest performance reference; retain reps-per-leg logging.


## Confirmed update: 2026-11-24 Tuesday
- Wide-stance leg press setting 5: 60 kg x 23, then 63.75 kg (60 + 3.75) x 10.
- Rear-delt fly setting 5: 37.5 kg x 10, then 41.25 kg (37.5 + 3.75) x 5. The heavier set fell below the usual isolation rep range; do not increase load.
- Dumbbell RDL: 12.5 kg x 10, then 15 kg x 10. Per-dumbbell versus combined load was not specified.
- Calf raise setting 5: 37.5 kg x 19 and x 18.
- Shoulder press setting 5: 15 kg x 17 and x 10.
- Lateral raise: 5 kg x 5; equipment type and load basis were not specified.
- Seated knee raises: bodyweight x 75.
- Side-lying leg raise: 15 kg x 30; whether reps were per leg or total was not specified.
- Farmer's carry: 15 kg each hand, 3 x 20; the unit for 20 was not specified. Route remains walking to and fro inside gym.
- Set types and RIR were not supplied. Preserve these unknowns in the log.
- Equipment correction: user confirmed no hamstring curl machine is available at the current gym. Do not prescribe or assume access to one.


## Coaching system correction: 2026-11-24
- User confirms the current gym is in Bengaluru. Historical Kanpur/previous-gym equipment must not be treated as available in Bengaluru.
- The warm-up is seated knee raises, Farmer's carries, and side-lying leg raises. No extra warm-up routine by default.
- User's working sets normally go to failure; 10 reps is a minimum, not a cap.
- Farmer's carries corrected to 20 kg each hand for 3 rounds. Carry 20 kg each hand forward as the next starting load.
- Seated knee raise target updated to 75 bodyweight reps on training days except Wednesday.
- Side-lying leg raise latest load updated to 15 kg × 30; whether reps are per leg or total remains unspecified.
- Preserve historic machine data, but do not prescribe a machine unless Bengaluru availability is explicitly confirmed.


## User confirmation and current-gym corrections: 2026-11-24
- Full Bengaluru equipment inventory confirmed: combined chest/incline/shoulder press machine with settings 3/4/5; combined leg press/calf raise machine setting 5; combined lat pulldown/seated row machine; abdominal machine setting 7; back extension setting 1; combined biceps/triceps machine setting 5; rear-delt fly setting 5; cable machine used for lateral raises and pulls; dumbbells; pull-up station. These are not Kanpur-only machines. Seated/lying hamstring curl remains unavailable.
- RDL load basis: 15 kg per dumbbell, 30 kg total. 2026-11-24 set data corrected accordingly.
- Lateral raise: 5 kg per hand on the cable machine.
- Side-lying leg raise: 20 kg per leg × 30 reps per leg. 2026-11-24 record corrected from the earlier ambiguous/wrong entry.
- Farmer's carries: 20 kg each hand, 3 rounds. 2026-11-24 record clarified and carried forward.
- Seated knee raises: bodyweight × 75, replaces the older 50-rep target.
- Pull-ups: daily, bodyweight maximum clean reps. Latest 2026-11-24 performance: 4 reps.
- Warm-up: seated knee raises, Farmer's carries, side-lying leg raises only. Do not add other warm-up blocks by default.
- All working sets normally go to failure. Choose a load permitting at least 10 clean reps, then continue beyond 10 until failure. Track weight and rep PRs separately. Do not use RIR targets by default.
- Working-set count: normally 2 per exercise; if the user elects 3 due to time, use 3 across all exercises that workout.
- Strength-biased hypertrophy preference: perform main/heaviest lifts early while fresh after the established warm-up.
- Carry the newest load and rep targets forward. Do not revert to old performance baselines.


## Explicit user correction: 2026-11-24
- The complete machine inventory above is confirmed in Bengaluru. Do not confuse it with Kanpur equipment. The settings are: chest 3, incline 4, shoulder 5, leg press/calf 5, lat/row combined setting unknown, abs 7, back extension 1, biceps/triceps 5, rear delt 5.
- Daily pull-ups are a separate max-rep exercise, including Wednesdays. Latest is 4 bodyweight reps.
- Side-lying leg raises are 20 kg per leg for 30 reps per leg.
- Farmer's carry is 20 kg in each hand, 3 rounds on normal training days.
- Seated knee raises are bodyweight × 75 on training days except Wednesday.
- RDL is 15 kg per dumbbell, total 30 kg. Cable lateral raise is 5 kg per hand.
- Usually 2 working sets per exercise. If user elects 3 because of time, use 3 for all exercises in that workout, never a mixture.
- User prefers strength-biased hypertrophy: perform main/heaviest compound exercises early while fresh, following their established warm-up. All working sets are taken to failure; load should allow at least 10 clean reps, then continue beyond 10 until failure.


## Confirmed update: 2026-11-25 Wednesday
- Lat pulldown at 41.25 kg (37.5 + 3.75): two reported grip sequences, each wide 5, less-wide 5, close 4 on the first sequence and close 3 on the second. Full sequence logged as six individual sets. Hold or reduce load next exposure because all reported grip results were below 10.
- Seated row: 45 kg × 9 for both sets. Hold or reduce next exposure to target at least 10 clean reps.
- Abdominal machine setting 7: 48.75 kg (45 + 3.75) × 18 and × 16. Assess smallest practical increase next exposure.
- Back extension setting 1: 45 kg × 15 and × 8. Mixed result; retain 45 kg for now rather than increasing, and prioritize clean reps.
- Farmer's carry: 20 kg each hand × 3 rounds; seated knee raises: bodyweight × 75.
- Side-lying leg raise: 15 kg per leg × 30 reps per leg today. Previous 20 kg per leg × 30 remains the historical best; latest completed load is 15 kg.
- User explicitly corrected the temporary phase: no rest days this week or next week. Wednesday 2026-11-25 was completed as Back + Abs, and Wednesday 2026-12-02 is also a training day. This supersedes the phase plan's earlier active-recovery-only Wednesday text.


## Confirmed update: 2026-11-26 Thursday
- Chest press setting 3: 33.75 kg (30 + 3.75) × 10, then × 7. Qualifying load PR: 33.75 kg × 10; next exposure hold or reduce to achieve at least 10 clean reps on both sets.
- Incline press setting 4: 26.25 kg (22.5 + 3.75) × 10. Qualifying load PR: 26.25 kg × 10; only one set was reported.
- Biceps curl setting 5: 30 kg × 10, then 33.75 kg (30 + 3.75) × 8. Qualifying load PR: 30 kg × 10; do not use 33.75 kg as a qualifying load until it reaches 10 clean reps.
- Triceps setting 5: 30 kg × 15, then 33.75 kg (30 + 3.75) × 9. Qualifying load PR: 30 kg × 15; reduce/hold next exposure to meet the 10-rep minimum.
- Daily pull-ups: bodyweight × 6, new rep PR. Set/attempt structure was not specified.
- Warm-up reported: side-lying leg raise interpreted as 15 kg per leg × 30 per leg; seated knee raises 75 reps with no added load reported; Farmer's carry 20 kg each hand, rounds not reported.


## Confirmed update: 2026-11-27 Friday
- Lat pulldown: two grip sequences, very-wide/wide/close, with reps 5/2/2 and 5/3/3. Load and machine setting were not stated. Keep load unknown; all reported reps were below 10.
- Rear-delt fly setting 5: 41.25 kg × 8 for both sets. Below the 10-rep minimum; do not increase.
- Biceps curl setting 5: 37.5 kg × 6. Below the 10-rep minimum; reduce or hold at a lower load next exposure.
- Triceps setting 5: 33.75 kg × 11, then 11 reps with load unspecified. First set qualifies at 33.75 kg for the 10-rep load threshold; second set's load remains unknown.
- Dumbbell RDL: 15 kg per dumbbell × 11, then × 10 (30 kg total). Keep the load for now; preserve technical execution.
- Pull-ups: bodyweight × 6; same reported rep count as 2026-11-26, no new rep PR. Set/attempt structure unspecified.
- Warm-up movements were not reported.
