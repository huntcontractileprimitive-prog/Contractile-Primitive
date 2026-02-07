# Reflex Loop Boundaries and Variable Isolation

Date: June 30, 2025  
Location: Cortson Forge (Home Lab)  
Project: Cortson BioFiber / ForceFiber  
Generation Context: Gen 1.85–1.9  
Note Index: 012  

---

## Context

After reframing contraction testing as a reflex-loop experiment, it became necessary to explicitly define what variables are allowed to change during testing and which must remain fixed.

Without boundary definitions, iterative testing risks conflating system behavior with test drift.

This entry establishes early isolation rules.

---

## Objective

- Identify controllable vs uncontrollable variables
- Prevent accidental multi-variable experimentation
- Create a baseline condition for comparison across days
- Reduce false attribution of cause and effect

---

## Variable Categories

### Fixed Variables (per test series)

These are held constant across a test run:

- Core geometry and lamination arrangement
- Coil wire gauge and winding count
- Mechanical spacing between contraction elements
- Power supply voltage ceiling
- Environmental setup (mounting orientation, ambient airflow)

Any change to a fixed variable defines a *new test series*, not a continuation.

---

### Adjustable Variables (within a test series)

These may be varied intentionally:

- Pulse width
- Duty cycle
- Pulse timing or cadence
- Number of active coils
- Manual vs timed triggering

Only **one adjustable variable** is changed per iteration.

---

### Observed Variables (non-controlled)

These are measured but not directly controlled:

- Temperature rise
- Back-EMF behavior
- Mechanical settling time
- Audible or vibrational artifacts
- Repeatability across cycles

Observed variables are treated as outputs, not tuning inputs.

---

## Boundary Rule

If more than one adjustable variable is changed between runs, the result is invalid for comparison.

If a fixed variable is unintentionally altered, the test sequence is reset and relabeled.

This rule exists to protect clarity, not slow progress.

---

## Rationale

Early-stage systems often “feel” like they are improving when, in fact, the experiment itself is drifting.

By enforcing variable isolation early:
- Later optimization becomes easier
- Data becomes legible
- Confidence becomes grounded in repeatable behavior

This reduces emotional interpretation of results.

---

## Builder Observation

Defining boundaries reduced internal pressure to “make progress” and shifted focus toward understanding behavior.

The system does not need to impress — it needs to respond consistently.

---

## Status

- Variable boundaries defined
- Test discipline increased
- Preparation complete for formal protocol drafting

Next step is documenting a single reflex-loop test protocol using these constraints.
