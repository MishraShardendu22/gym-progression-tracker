# Exercise Reference and Performance

The machine inventory below is confirmed for the user's current Bengaluru gym. The records table preserves historical sessions and latest reported performances. Use the newest dated performance for coaching. Machine setting and machine load are separate values.

## Confirmed Bengaluru equipment

- Combined press machine: chest press setting 3, incline press setting 4, shoulder press setting 5.
- Combined leg press/calf raise machine: setting 5 for both.
- Combined lat pulldown/seated row machine: setting not recorded.
- Abdominal machine: setting 7.
- Back extension machine: setting 1.
- Combined biceps/triceps machine: setting 5.
- Rear-delt fly machine: setting 5.
- Cable machine: used for lateral raises and pulls only. Lateral raise load: 5 kg per hand.
- Dumbbells for RDL: 15 kg per dumbbell, 30 kg total.
- Pull-up station: daily bodyweight max-rep pull-ups.
- Seated knee raises, Farmer's carries, and side-lying leg raises.
- Explicitly unavailable: seated/lying hamstring curl machine.

## Exercise records

| Exercise | Machine setting | Known load × reps | Confidence / notes |
|---|---:|---|---|
| Chest press | 3 | 26.25 kg × 10 | Latest session 2026-11-05: 22.5 × 30, then 26.25 × 10 for two sets. The 30-rep entry is recorded literally as reported. |
| Incline press | 4 | 18.75 kg × 10 | Latest session 2026-11-05: 18.75 × 10 for three sets (reported as 15 + 3.75 kg). |
| Shoulder press | 5 | 15 kg × 17, 10 | Latest session 2026-11-24: 15 × 17 and 15 × 10. |
| Lat pulldown | Unknown | 37.5 kg × 4 | Latest session 2026-11-02: at 30 kg, wide 5, less-wide 5, close 10; at 33.75 kg, 5/5/5; at 37.5 kg, 5/5/4. Grip order preserved. |
| Seated row | Unknown | 45 kg × 10 | Latest session 2026-11-02: 37.5 × 10, 41.25 × 13, 45 × 10. |
| Rear-delt fly | 5 | 37.5 kg × 10; 41.25 kg × 5 | Latest session 2026-11-24: 37.5 × 10, then 41.25 × 5. |
| Biceps curl machine | 5 | 37.5 kg × 7 | Latest session 2026-11-05: 37.5 × 7, 5, 4. |
| Triceps exercise/machine | 5 | 37.5 kg × 6 | Latest session 2026-11-05: 37.5 × 5, 6, 3. Exact exercise/machine naming should be confirmed if needed. |
| Abdominal machine | 7 | 45 kg × 10 | Latest confirmed session 2026-11-02: 45 × 10. Earlier 33.75 kg × 12 and × 15 (30 + 3.75). |
| Back extension | 1 | 45 kg × 10 | Earlier 33.75 kg × 12 and × 15. |
| Leg press (historical stance unspecified) | 5 | 63.75 kg × 21 | Latest historical session 2026-11-03: 52.5 × 20, 60 × 21, 63.75 × 21. Stance was not recorded. |
| Wide-stance leg press | 5 | 60 kg × 23; 63.75 kg × 10 | Latest session 2026-11-24: 60 × 23, then 63.75 × 10. Earlier session 2026-11-22: 63.75 × 17 and × 9. |
| Calf raise | 5 | 37.5 kg × 19, 18 | Latest session 2026-11-24: 37.5 × 19 and × 18. |
| Lateral raise | Cable machine | 5 kg per hand × 5 | Latest session 2026-11-24; user confirmed cable machine and per-hand load. |
| Side-lying hip abduction | N/A | 20 kg per leg × 30 per leg | User clarified 2026-11-24: 20 kg each leg, 30 reps per leg. |
| Dumbbell Romanian deadlift | N/A | 15 kg per dumbbell × 10 (30 kg total) | Latest session 2026-11-24: 12.5 kg per dumbbell × 10, then 15 kg per dumbbell × 10. |
| Seated knee raises | N/A | Bodyweight × 75 | Latest session 2026-11-24. Every training day except Wednesday. |
| Farmer's carry | N/A | 20 kg each hand × 3 rounds | Latest Bengaluru session 2026-11-24: walking to and fro inside the gym. |
| Pull-ups | N/A | Bodyweight × 4 max reps | Daily maximum clean reps; latest report 2026-11-24. Attempt/set count not separately specified. |


## Machine adjustment settings

| Machine / movement | Setting | Availability |
|---|---:|---|
| Chest press | 3 | Bengaluru, combined press machine |
| Incline press | 4 | Bengaluru, combined press machine |
| Shoulder press | 5 | Bengaluru, combined press machine |
| Leg press | 5 | Bengaluru, combined leg press/calf machine |
| Calf raise | 5 | Same machine as leg press |
| Lat pulldown / seated row | Not recorded | Bengaluru, combined machine |
| Abdominal machine | 7 | Bengaluru |
| Back extension | 1 | Bengaluru |
| Biceps / triceps | 5 | Bengaluru, combined machine |
| Rear-delt fly | 5 | Bengaluru |
| Cable machine | N/A | Lateral raises and pulls only |

## Current fixed performance references

- RDL: 15 kg per dumbbell, 30 kg total.
- Cable lateral raise: 5 kg per hand.
- Side-lying leg raise: 20 kg per leg × 30 reps per leg.
- Farmer's carry: 20 kg each hand × 3 rounds.
- Seated knee raises: bodyweight × 75 reps on training days except Wednesday.
- Pull-ups: daily max clean bodyweight reps; latest report 4 reps.

See `instruction.md` for the complete coaching rules and `agent.md` for the agent workflow. Preserve the historical context in old rows; do not treat an old PR as the latest session result.
