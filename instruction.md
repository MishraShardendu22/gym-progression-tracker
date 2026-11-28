# Training Instructions

**Canonical user preferences.** Last explicitly confirmed: 2026-11-24.  
**Current gym:** Bengaluru, India.  
**Time zone for dates and training-day decisions:** Asia/Kolkata.  
**Scheduled workout start time:** 07:00 (7:00 AM), Asia/Kolkata, every scheduled training day.

This file records the user's training rules. Do not silently replace them with generic fitness templates. When the user explicitly changes a rule, update this file and the current-state records. If a newer explicit user instruction conflicts with this file, the newer instruction wins and must be persisted.

## 1. Training objective and style

The user trains with a **strength-biased hypertrophy** approach: build muscle while prioritizing progressive strength increases. Start the main/heaviest compound work while fresh. Follow the exercise order in PROGRAM.md. Arrange the session with the main compound movements before accessory/isolation movements where practical.

The user normally takes **every working set to failure**. Choose a load expected to permit at least 10 clean reps, then continue beyond 10 until failure. Ten reps is a minimum load-selection reference, not a stopping point or rep cap.

- If a set reaches failure above 10 clean reps, assess the smallest practical load increase for the next exposure.
- If failure occurs below 10 clean reps, hold or reduce the load so the next attempt can meet the minimum.
- If failure occurs at 10 reps, use the other sets and recent performance to decide whether to hold or progress.
- Never tell the user to stop at 10 simply because the threshold has been reached.
- Do not prescribe RIR targets by default. The user's normal method is failure.
- Failure means the next full, clean concentric repetition cannot be completed. Do not use forced repetitions or intentionally degrade technique. On RDLs and other technically sensitive free-weight movements, stop at technical failure before position or execution breaks down.

### Working-set count

The normal prescription is **2 working sets per exercise**. When the user has enough time and chooses a third set, use **3 working sets for every exercise in that workout**. Do not mix 2 sets for some exercises and 3 for others unless the user explicitly asks for that exception.

Any preparation activity, if later specified, does not count toward working-set volume.

## 2. Scheduled accessory and core movements

The former daily warm-up routine is superseded by the current weekly split. Do not automatically perform seated knee raises, Farmer's carries, or side-lying/standing leg raises every day. Follow the exact exercise days in the current split:
- Seated knee raises: Monday and Thursday.
- Farmer's carries: Monday and Friday.
- Standing side leg raises with a weighted plate: Monday and Friday.
- Abdominal crunch: Tuesday and Saturday.

Wednesday is a complete rest day. None of these movements, or any other training, is scheduled on Wednesday.

Current historical references:
- Seated knee raises: bodyweight × 75 reps.
- Farmer's carry: 2026-11-28 report was 22.5 kg × 3 sets; per-hand versus total load is unconfirmed.
- Standing side leg raise: 15 kg reported on 2026-11-28; repetitions and load basis require confirmation before precise progression.

## 3. Pull-ups

Pull-ups are not included in the current weekly split. Do not prescribe daily pull-ups or schedule pull-ups on Wednesday. If the user wants them restored, confirm the days and loading method first.

## 4. Fixed weekly split

The training week begins on **Sunday, Day 1**. The current authoritative day-by-day schedule and exact exercise list are in [PROGRAM.md](PROGRAM.md). Follow it without substitutions or frequency changes.

- Sunday: Upper body A.
- Monday: Legs + core.
- Tuesday: Pressing + posterior chain.
- Wednesday: Complete rest, no gym training or scheduled exercise.
- Thursday: Upper body B.
- Friday: Legs + accessories.
- Saturday: Strength day.

Lat pulldown is scheduled Sunday, Thursday, and Saturday. Every session must include the full three-grip combination: one-third very-wide grip, one-third wide grip, and one-third close grip. These are grip variations within the same exercise, not separate additional exercises.

Flat chest press is scheduled twice weekly; incline chest press and shoulder press are each scheduled twice weekly. Do not add chest fly. Rear-delt fly remains the rear-delt isolation exercise.

Never shift the split to compensate for a missed workout. Wednesday remains the fixed complete rest day.

## 5. Confirmed Bengaluru gym equipment

All equipment and settings below are confirmed by the user as present in the current Bengaluru gym. Do not label these machines as Kanpur-only or unavailable.

| Equipment | Exercise / use | Setting |
|---|---|---:|
| Combined press machine | Chest press | 3 |
| Same combined press machine | Incline press | 4 |
| Same combined press machine | Shoulder press | 5 |
| Combined leg press / calf machine | Wide-stance leg press | 5 |
| Same leg press / calf machine | Calf raises | 5 |
| Combined lat pulldown / seated row machine | Lat pulldown and seated row | Not recorded |
| Abdominal machine | Abs | 7 |
| Back extension machine | Back extension | 1 |
| Combined biceps / triceps machine | Biceps and triceps exercises | 5 |
| Rear-delt fly machine | Rear delts | 5 |
| Cable machine | Lateral raises and pulls only | Lateral raise: 5 kg per hand |
| Dumbbells | Romanian deadlifts | Latest: 15 kg per dumbbell |
| Pull-up station | Daily bodyweight pull-ups | Bodyweight |

**Explicitly unavailable:** seated/lying hamstring curl machine. Never prescribe it for this gym.

Do not infer extra cable exercises or machine functions beyond those listed. If the user reports a gym/location change, ask what equipment is available there before reusing this inventory.

## 6. Exercise-specific current references

These are the latest confirmed baselines, not prescriptions to blindly repeat regardless of newer logs.

| Exercise | Latest confirmed performance / target |
|---|---|
| Wide-stance leg press | Setting 5. 60 kg × 23, then 63.75 kg × 10, on 2026-11-24 |
| Calf raise | Setting 5. 37.5 kg × 19 and × 18, on 2026-11-24 |
| Shoulder press | Setting 5. 15 kg × 17 and × 10, on 2026-11-24 |
| Rear-delt fly | Setting 5. 37.5 kg × 10, then 41.25 kg × 5, on 2026-11-24 |
| Dumbbell RDL | 12.5 kg per dumbbell × 10, then 15 kg per dumbbell × 10. The second set is 30 kg total |
| Cable lateral raise | 5 kg per hand × 5 on 2026-11-24 |
| Side-lying leg raise | 20 kg per leg × 30 reps per leg |
| Farmer's carry | 20 kg in each hand × 3 rounds, walking to and fro |
| Seated knee raises | Bodyweight × 75 reps |
| Pull-ups | Bodyweight, daily max reps; latest report 4 |

Historical performances remain in `workout-log.csv` and dated session notes. Use the newest dated performance for current coaching. Preserve load basis: dumbbell loads are per dumbbell, lateral raise is per hand, side-lying leg raise is per leg, and Farmer's carry is per hand. `personal-records.csv` is the sole PR index, with one current row per exercise; update that row in place rather than adding historical PR rows.

## 7. Progression and PR tracking

Track these separately for every lifting exercise:

- Maintain exactly one current PR/best benchmark entry per exercise in `personal-records.csv`. Replace that exercise's row in place only when a new qualifying record is established.
- For loaded exercises, a load PR is the heaviest load completed for at least 10 clean reps to failure. A below-10-rep result does not qualify as a load PR.
- For bodyweight and fixed-load movements, retain the single best comparable benchmark (for example, max reps at bodyweight or reps at a fixed load).
- **Latest performance:** every set from the most recent session, including different loads across sets.
- **Machine setting:** preserve the correct adjustment setting separately from the weight-stack load.

Do not estimate a 1RM unless the user asks. Do not turn a rep PR into a load PR. A set below 10 reps does not establish a new 10-rep load PR, but it remains a valid logged performance.

Use the latest confirmed performance to calculate the next starting load. Carry new weights and rep targets forward automatically. Never revert to old loads or targets without a reason grounded in a newer report.

## 8. Reporting and record quality

Ask the user to report each set individually in a simple format such as `Exercise, Set 1: reps × kg`. Preserve whether a load is per dumbbell, per hand, total, or machine stack. Record machine settings where applicable.

Never invent:
- sets, reps, dates, loads, machine settings, RIR, failure status, distance, duration, or load basis;
- equipment availability;
- whether a daily pull-up number represents one set or several attempts.

The standing rule is that working sets go to failure. Apply it to new sessions after the user confirmed it. Do not retroactively rewrite old sessions as failure sets unless the user explicitly confirms that historical classification.

When an entry is ambiguous, preserve the ambiguity and ask only if it materially changes the next prescription or record.


## Missing-load carry-forward

A blank load in a recent workout entry does not mean the exercise has no known load. Before presenting a load as unknown, inspect the latest earlier confirmed load for the same exercise and equipment. When the user confirms that an omitted load was unchanged, apply that confirmed load to every affected set in workout-log.csv, current-state.json, EXERCISES.md, progression.md, and the dated session note. Preserve the reported reps and keep unrelated unknown fields (such as machine adjustment setting) unknown. Do not ask the user to repeat a load they have already confirmed. If no prior confirmed load exists, or the user has not confirmed that it was unchanged, preserve the blank and ask one focused clarification only when the missing value materially affects the next prescription or log accuracy.

For lat pulldown specifically, the last confirmed machine-stack load is 41.25 kg. The user confirmed on 2026-11-28 that all six sets reported on 2026-11-27 used this same load. The 2026-11-27 reps were 5/2/2 and 5/3/3 across two very-wide/wide/close sequences. The 41.25 kg load is known; the machine adjustment setting remains unknown.


## PR index and history separation

`personal-records.csv` is the only source for current PR/best benchmark lookup and contains one row per exercise at most. When a new qualifying PR occurs, update the existing exercise row in place; do not append another row for that exercise. `workout-log.csv` continues to append every reported set and is never pruned to keep the PR table small. `current-state.json` stores latest session state and latest performance, not a duplicate PR catalogue.
