# Cortson BioFiber — Staged Activation and Multi-Cell Coordination

**Date:** May 6, 2025  
**Project:** Cortson BioFiber  
**Prototype:** Multi-Core Strand (v1.x)  
**Location:** Home Workshop  
**Builder:** Mason Hunt  

---

## Summary

During continued experimentation with multi-core BioFiber strands, staged (non-simultaneous) activation of individual coils was explored. This approach revealed improved contraction smoothness, reduced instantaneous current draw, and more controllable thermal behavior compared to fully synchronous pulsing.

This session marks the first recognition that BioFiber performance is strongly influenced by **activation sequencing**, not just field strength.

---

## Test Configuration

- Multi-core strand with independently addressable coils.
- Manual pulse triggering with intentional delay between coil activations.
- Supply voltage in the 20–24 V range.
- Visual inspection, tactile feedback, and thermal monitoring by touch and time-to-cool.

---

## Observations

- Sequential activation produced smoother contraction than simultaneous firing.
- Peak current draw appeared reduced when coils were offset in time.
- Mechanical motion felt more controlled and less abrupt.
- The strand exhibited less audible noise and vibration under staged pulses.
- Thermal rise per activation cycle was lower when pulses were distributed.

---

## Comparative Behavior

**Simultaneous Activation**
- High instantaneous current demand.
- Sharper contraction onset.
- Faster localized heating.
- Increased risk of saturation and inefficiency.

**Staged Activation**
- Distributed magnetic loading.
- More gradual force buildup.
- Improved controllability.
- Reduced thermal stress per cycle.

---

## Insight: Timing as a Control Dimension

This test demonstrated that timing itself functions as a control variable:

- Force output is not solely a function of voltage or current.
- Pulse sequencing alters magnetic coupling dynamics.
- Multi-cell strands behave more like coordinated systems than single actuators.

This reframes the strand from a “single muscle” into a **coordinated actuator array**.

---

## Design Implications

- Future control systems must support per-coil timing offsets.
- Control architecture should treat each cell as an addressable unit.
- Staged activation opens the door to:
  - Wave-based contraction
  - Peristaltic motion
  - Load-adaptive sequencing

These ideas later inform Pulse Node channel design and reflex-loop concepts.

---

## Directional Shift

This session marks a conceptual shift from:
> “Drive all coils equally”  
to  
> “Shape motion through timing relationships.”

Timing becomes as important as magnitude.

---

## Next Steps

- Formalize timing offsets using electronic control.
- Test repeatable delay intervals between cells.
- Explore sequential patterns under load.
- Evaluate thermal benefits quantitatively.

---

## Status

- Staged activation validated.
- Multi-cell coordination identified as a key performance lever.
- Timing recognized as a first-class design parameter.
