---
title: "SASP Baseline Assessment Protocol"
document_type: "framework"
status: "draft"
version: "0.1"
last_updated: "2026-05-06"
author: "Coach Jim West"
organization: "Wilco Shooting Sports"
audience:
  - coaches
  - athletes
summary: "A four-test isolated component assessment protocol for SASP athletes. Measures first-shot time, trigger cycle speed, transition speed, and applied full-stage execution, then combines them into a Theoretical Stage Time model and coaching score framework."
related_documents:
  - "frameworks/steel-performance-framework.md"
  - "frameworks/execution-models.md"
  - "frameworks/impact-assessment-model.md"
  - "doctrine/terminology.md"
  - "templates/steel-baseline-assessment-log.md"
canonical_terminology: "doctrine/terminology.md"
tags:
  - framework
  - steel-challenge
  - assessment
  - baseline
  - metrics
  - draft
---

# SASP Baseline Assessment Protocol

> **Canonical terminology reference:** [doctrine/terminology.md](../doctrine/terminology.md)
>
> **Data capture form:** [templates/steel-baseline-assessment-log.md](../templates/steel-baseline-assessment-log.md)

---

## Purpose

This protocol isolates and measures the individual components of the SASP shooting sequence. Rather than analyzing a complete stage run, each test is designed to produce a clean measurement of one component at a time — free from the interference of other variables.

The resulting measurements serve three purposes:

1. **Establish a personal baseline** against known benchmark ranges for skill level
2. **Direct coaching focus** toward the component with the highest development leverage
3. **Track progression** by repeating assessments at intervals and comparing results over time

This protocol does not replace run classification or in-session coaching. It supplements them with quantified, comparable data.

> **Principle:** A stage time is the sum of its components. Improvement in any component improves stage time. Improvement across multiple components compounds. Understanding which components are weak directs effort efficiently.

---

## Equipment Requirements

- Shot timer (audible start signal)
- Target array appropriate to each test (described per test):
  - **Tests 1 and 3:** One target at a safe distance (stage-typical: 7–10 yards)
  - **Test 2:** Wide stage array with targets at the full lateral range of a typical Steel stage (e.g., Focus); use the same wide stage for Tests 1–3 if available, to standardize conditions
- Magazine / speed-loader loadout prepared before evaluation (per discipline tested):
  - **Ideal baseline loadout:** 6 complete magazines or speed loaders, loaded with **10 rounds each** when equipment allows
  - **Acceptable alternative loadout:** 5 complete magazines or speed loaders, loaded with **8 rounds each** for lower-capacity platforms
  - **Minimum baseline requirement:** enough preloaded ammunition to complete all four tests without reloading on the clock (see allocation guide below)
  - Keep at least one additional loaded magazine/speed loader available as contingency in case of dropped magazine, unexpected misses, or restart needs
- Athlete in full competition-legal gear (firearm — same setup used in matches)
- Two-coach staffing recommended for speed and quality:
  - **Coach A:** runs sequence, enforces safety/process, and cues athlete
  - **Coach B:** records timer data, scores observations, and logs notes in real time
- Log sheet

### Suggested Loadout Allocation by Test

| Test | Round plan | Recommended loadout allocation |
|------|------------|--------------------------------|
| Test 1 — Trigger Speed | 8–10 shots, single run by default | 1 magazine/speed loader |
| Test 2 — Transition Speed | 10 runs total (5 L→R + 5 R→L), 2 shots each (20 shots total) | 2 magazines/speed loaders total (one per direction, or mixed by direction as needed) |
| Test 3 — First-Target Acquisition | 8–10 single-shot reps | 1 magazine/speed loader |
| Test 4 — Full Stage Runs | Remaining rounds for 3–5 full runs + observation scoring | 2–3 magazines/speed loaders |

> **Planning note:** For most athletes, 6×10 is ideal. 5×8 can still run the baseline, but with less margin for extra runs or contingency.

---

## Test 1: Trigger Speed Test (Rapid Fire)

### Purpose

Isolate the athlete's trigger mechanics from all other variables. Measure:

- **First Shot Time (1st Shot Time)** — reaction time plus the mechanical response to the beep
- **Split Times** — the trigger cycle speed between consecutive shots
- **Average Split Time** — the athlete's sustainable mechanical pace
- **Fastest Split Time** — the athlete's mechanical ceiling
- **Reaction Time** — the neurological component of First Shot Time, derived by calculation

### Setup

- One target at safe stage-typical distance (7–10 yards); no accuracy requirement beyond keeping all rounds on or near target
- Firearm loaded with a full magazine; firearm aimed at the target; finger on trigger
- Shooter is in the shooter's box, ready; no low ready involved
- Shot timer positioned to capture all shots

> **Context note on split time:** In this test, the split time isolates the pure trigger press cycle — engage slack, reach the wall, prep, prep, prep, break, reset. No transition or recoil movement is involved. This is the most controlled measurement of mechanical trigger speed.

### Procedure

1. Athlete establishes grip, stance, and sight picture — finger on trigger, aimed at target
2. Coach signals to timer operator: "Shooter Ready"
3. On the beep, athlete fires every round in the magazine as fast as possible, keeping all rounds in the general target area
4. Timer captures the full string; coach records total time, # of shots recorded, First Shot Time and all split times as displayed on the timer
5. Default protocol is **one run only**. Repeat only if instructions were not understood, timer capture failed, or safety/process setup was invalid.

### Measurements Recorded

| Measurement | How Recorded |
|-------------|-------------|
| First Shot Time (1st Shot Time) | Time from beep to first shot break |
| Split times (all) | Time between each consecutive shot break |
| Total shots fired | Count from the string |
| Total string time | Time from beep to last shot break |

### Calculations

| Calculation | Formula |
|-------------|---------|
| Average Split Time | Sum of all split times ÷ number of splits |
| Fastest Split Time | The lowest single split time recorded |
| Reaction Time | First Shot Time − Average Split Time |

> **Note on Reaction Time:** The timer start beep is a randomized countdown (typically 1–3 seconds), which reduces athlete ability to predict the start from human cues. Watch for start cheating indicators: finger creeping into trigger guard/onto trigger before beep, or muzzle movement off start-cone position before beep. The average split time represents mechanical trigger cycle time; subtracting it from First Shot Time approximates neurological reaction delay.
>
> **Benchmark placeholder:** Reaction Time benchmark bands are **TBD** and will be added after sufficient field data is collected.

### Benchmark Classifications

| Classification | Average Split Time |
|---------------|-------------------|
| World Class / Elite | 0.12–0.13 sec |
| Senior | Below 0.20 sec |
| Intermediate | 0.20–0.30 sec |
| Rookie / Foundation | 0.30–0.50 sec |

> These benchmarks reflect the sustained pace during rapid fire on a single target. They are not stage split times, which include transitions. Use these ranges for component-level diagnosis only.

---

## Test 2: Transition Speed Test

### Purpose

Isolate the athlete's lateral inter-target movement speed. Measure:

- **Inter-Target Transition Time (ITT)** — the time from the shot break on one target to the shot break on the next (T1→T2, T2→T3, T3→T4, T4→T5)
- **Directional asymmetry** — which direction is faster, and by how much

Each transition covers a different angular distance (short adjacent moves vs. long cross-stage sweeps), so ITT is best treated as an average across all moves and multiple runs. The sub-components of ITT — lateral muzzle movement, recoil management, direction reversals, impact confirmation, and the trigger cycle on the new target — are difficult to isolate individually at this level and are captured in aggregate.

> **Distinction from Test 3:** ITT measures movement *between* targets. The time from the start signal (beep) to the first shot — from low-ready to T1 — is a separate component called **First-Target Acquisition Time**, measured in Test 3.

This reveals whether body geometry, stance orientation, or dominant-side mechanics favor one direction, and informs positioning and footwork adjustments.

### Setup

- Wide stage with targets at the far left and far right of the array (a stage like *Focus* works well; targets should be separated by the full lateral range of a typical Steel stage)
- Firearm loaded; aimed at the starting target; finger on trigger
- Shooter in the shooter's box in competition stance
- Shot timer ready

### Procedure

1. Athlete aims at the far-left target, finger on trigger, firearm ready
2. On beep, fire one round at the far-left target, immediately transition to the far-right target, fire one round
3. Record the total time from beep to second shot break; record the split time from the 1st shot to the 2nd shot as the **Inter-Target Transition Time (ITT)**
4. Repeat 5 runs in this direction; average the results
5. Reverse: start aimed at far-right target, transition left; repeat 5 runs; average
- Note body positions and form

> **Note on accuracy:** Hits are not required for this test. The athlete should fire in the general direction of each target. The purpose is speed measurement only. If accuracy significantly degrades, note it — it may indicate the athlete is pushing beyond a controlled threshold.

### Measurements Recorded

| Measurement | How Recorded |
|-------------|-------------|
| Total time per run (beep to 2nd shot) | From shot timer |
| ITT (split time from 1st shot to 2nd shot) | Read directly from shot timer — **primary measure** |
| Direction of each run (L→R or R→L) | Noted by coach |

### Calculations

Two methods produce the same ITT value — use the split-time read as the primary and the subtract-First-Shot-Time method as a cross-check against Test 1:

| Calculation | Formula | Method |
|-------------|---------|--------|
| ITT (direct) | Split time: 2nd shot elapsed − 1st shot elapsed | **Primary** — read directly from timer |
| ITT (derived) | Total run time − First Shot Time (from Test 1 Best Run) | Cross-check — validates against Test 1 |
| Average ITT (L→R) | Average of all L→R ITT values | |
| Average ITT (R→L) | Average of all R→L ITT values | |
| Overall Average ITT | Average of all runs across both directions | Used in Theoretical Stage Time formula |
| Directional Advantage | Identify which direction is consistently faster | |

---

## Test 3: Low-Ready First Shot Test

### Purpose

Measure the **First-Target Acquisition Time** — the time from low-ready position to the first shot break on the first target. Commonly called **"1st shot time."** This component contains three sub-elements: neurological reaction time + muzzle presentation movement from low ready to the first target + trigger press.

Combined with values from Test 1, the presentation movement can be isolated:
> Presentation Time ≈ First-Target Acquisition Time − Reaction Time − Avg Split Time

First-Target Acquisition Time is typically the **first and most accessible place to reduce time in a clean run** — small improvements here apply directly to every string. Understanding its sub-components enables a targeted coaching plan.

Combined with values from Tests 1 and 2, it completes the isolated component model before Test 4 applied validation.

### Setup

- One target at stage-typical distance (7–10 yards)
- Firearm loaded; held in low-ready position (firearm pointed down at approximately 45°, grip established, finger outside trigger guard)
- Shot timer ready

### Procedure

1. Athlete establishes low-ready position
2. On beep, raise to target and fire one shot
3. Record elapsed time from beep to shot break
4. Repeat 4–5 times; average all runs; note fastest run

### Measurements Recorded

| Measurement | How Recorded |
|-------------|-------------|
| Time from beep to shot break (per run) | From shot timer |

### Calculations

| Calculation | Formula |
|-------------|---------|
| Average Low-Ready First Shot Time | Sum of all runs ÷ number of runs |
| Fastest Low-Ready First Shot Time | Lowest single run time |
| Derived First-Shot Transition Time (low ready → first target) | Avg First Shot Time (Test 3) − Avg Trigger Press Time (Test 1) − Avg Reaction Time (Test 1) |

> **Clarification:** This derived formula is correct for coaching decomposition. It estimates the movement/presentation component from low ready to first target. Use average values when available for stability.

---

## Test 4: Full Stage Runs (Applied Validation)

### Purpose

Validate whether isolated gains from Tests 1–3 appear in full-stage execution. This test captures applied decision quality, consistency under match-like flow, and observation-based coaching scores.

### Setup

- Standard SASP stage setup (e.g., Focus or equivalent)
- Athlete in normal competition flow and sequence
- Remaining baseline loadout (typically 2–3 magazines/speed loaders)
- Two-coach staffing preferred (Coach A runs sequence, Coach B logs scoring/notes)

### Procedure

1. Athlete shoots 3–5 full stage runs
2. Record string times and classify run quality
3. Complete observation scoring (1–5 scale) for stage prep, shot-call execution, stop-plate execution, on-deck readiness, between-string behavior, and other baseline observation items
4. Capture final coaching notes tied to repeatable findings and corrective actions

### Measurements Recorded

| Measurement | How Recorded |
|-------------|-------------|
| Full string time | Timer |
| Run quality | Coach classification (clean / sloppy / recovery) |
| Observation scores (1–5) | Log form scoring rows |
| Final coaching notes | Coach narrative synthesis |

---

## Composite Analysis: Theoretical Stage Time

### Overview

Once the first three isolated tests are complete, the individual components can be combined to calculate a **Theoretical Stage Time** for a given stage layout. Test 4 then validates those component findings in full-stage execution. This model shows how the athlete's measured components would add up if performed in sequence.

The model has two versions:

- **Serial model:** Each sub-task completes before the next begins — the baseline for less experienced athletes
- **Parallel model:** Trigger prep overlaps with muzzle transition — the model for intermediate and senior athletes executing prep-during-movement

For a full explanation of serial and parallel execution, see [frameworks/execution-models.md](../frameworks/execution-models.md).

### Formula

For a stage with **N targets** (one shot per target):

| Model | Formula |
|-------|---------|
| **Serial** | First-Target Acquisition Time + (N−1) × Avg ITT + (N−1) × Avg Split Time |
| **Parallel** | First-Target Acquisition Time + (N−1) × max(Avg ITT, Fastest Split Time) |

> **Why (N−1):** The first shot is captured in the First-Target Acquisition Time. Each subsequent shot requires one inter-target transition (ITT) and one trigger cycle. For 5 targets, there are 4 ITTs and 4 additional trigger cycles.

> **Formula components:**
> - First-Target Acquisition Time = Test 3 (low ready → T1 shot break)
> - Avg ITT = Test 2 (T1→T2, T2→T3, T3→T4, T4→T5 averaged)
> - Avg / Fastest Split Time = Test 1 (pure trigger cycle)

### Example Calculation

Using the following measured values for an intermediate:

| Component | Value |
|-----------|-------|
| First-Target Acquisition Time (Test 3) | 0.54 sec |
| Average Split Time (trigger cycle, Test 1) | 0.25 sec |
| Fastest Split Time (trigger cycle, Test 1) | 0.15 sec |
| Average ITT (Test 2) | 0.41 sec |
| Derived Reaction Time (Test 1) | 0.07 sec |

**For a 5-target stage (e.g., Focus):**

| Model | Calculation | Result |
|-------|-------------|--------|
| Serial | 0.54 + (4 × 0.41) + (4 × 0.25) | **3.18 sec** |
| Parallel | 0.54 + (4 × 0.41) | **2.18 sec** |

> **Interpretation:** The novice athlete performing all tasks in serial, with some additional hesitation and unaccounted latency between sub-tasks, produces a typical string time in the range of 3.4–3.6 seconds — consistent with observed novice performance. As the athlete's individual components improve and parallel execution is introduced, the theoretical time compresses toward the parallel model floor.  Sub-tasks performed in parallel are limited to the slowest sub-task.  If trigger press is slower than the ITT, a cadence issue may be observed.  Improving transitions in this case will not make meaningful improvement in string time.

### Component Improvement Impact

Each component that improves reduces stage time proportionally:

| Component improved | Effect on a 5-target stage|
|--------------------|---------------------------|
| Avg Trigger press (split) Time −0.05 sec | −0.20 sec per string |
| Avg ITT −0.05 sec | −0.20 sec per string |
| First-Target Acquisition Time −0.05 sec | −0.05 sec per string |
| Serial → Parallel execution | −0.40 to −1.00 sec per string (variable) |

> **Coaching implication:** ITT and trigger press time improvements have equal impact on serial stage time. The single largest gain comes from introducing parallel execution — but limited by the slowest sub-task time threshold.

---

## Tracking and Progression

### Reassessment Frequency

| Context | Frequency |
|---------|-----------|
| Active training athlete | Every 4–6 weeks |
| Competition season | Before season begins and mid-season |
| Following equipment change | Immediately after change, then 2 weeks later |
| Following a coaching intervention targeting a specific component | 2–3 weeks after intervention |

### What to Track Over Time

For each assessment date, record and compare:

- First Shot Time
- Average and fastest split time
- Derived reaction time
- Average ITT (by direction and overall)
- Average and fastest First-Target Acquisition Time
- Theoretical stage time (serial and parallel)
- Benchmark classification for split time

Plotting these values across dates reveals which components are improving, which are plateauing, and whether the athlete is converging toward parallel execution efficiency.

### Comparison Dimensions

This protocol supports comparison across:

- **Dates** — longitudinal progression for one athlete
- **Directions** — left-to-right vs. right-to-left asymmetry
- **Division/class ranges** — comparing individual component values against others in the same division
- **Benchmark standards** — placing each component against the known ranges (World Class / Senior / Intermediate / Rookie)

---

*Wilco Shooting Sports · SASP Baseline Assessment Protocol v0.1 · Draft*
