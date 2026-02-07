# Reflex Loop Baseline Test Protocol

Date: July 1, 2025  
Location: Cortson Forge (Home Lab)  
Project: Cortson BioFiber / ForceFiber  
Generation Context: Gen 1.85–1.9  
Note Index: 013  

---

## Context

With variable boundaries defined, the next requirement is a repeatable baseline test that can be rerun across days, builds, and incremental refinements.

This protocol defines the minimum viable reflex-loop test used to establish reference behavior.

---

## Purpose

- Create a repeatable contraction test
- Establish a known “good” baseline
- Enable comparison across hardware revisions
- Separate reflex behavior from optimization behavior

This protocol is not designed to maximize force or stroke.

---

## Test Configuration

### Hardware State

- Single contraction cell or paired cell segment
- Fixed core geometry and coil configuration
- No flux sheath modifications during baseline
- Mechanical mounting prevents lateral movement
- Manual access to power cutoff at all times

---

### Electrical State

- Fixed supply voltage (documented at test start)
- Single Pulse Node or manual trigger
- Flyback protection in place
- No dynamic modulation beyond pulse width

---

## Test Steps

1. Power system idle for ≥2 minutes
2. Record ambient temperature
3. Apply single pulse of fixed duration
4. Observe contraction behavior
5. Allow full relaxation to rest state
6. Repeat for 5 total cycles
7. Stop test if abnormal heat or noise occurs

---

## Data Logged

- Pulse duration
- Observable contraction distance (approximate)
- Time to full contraction
- Time to full relaxation
- Coil temperature before and after sequence
- Any audible or tactile anomalies

No optimization is performed during this protocol.

---

## Pass / Fail Criteria

Pass:
- Contraction occurs on every pulse
- Relaxation returns to repeatable rest position
- Temperature rise remains gradual and predictable
- No electrical instability observed

Fail:
- Inconsistent contraction
- Delayed or incomplete relaxation
- Rapid or runaway heating
- Mechanical misalignment or binding

A failure does not invalidate the design — it invalidates the test conditions.

---

## Builder Notes

This protocol reduces the temptation to “tune while testing.”

Once baseline behavior is known, optimization becomes intentional rather than reactive.

---

## Status

- Baseline protocol defined
- Ready for reuse across builds
- Enables longitudinal comparison

Next phase will involve controlled deviation from baseline parameters.
