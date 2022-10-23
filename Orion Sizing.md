# Orion - Conceptual Sizing Plan
A quick draft by Raihaan to guide the conceptual design sizing of Orion.

Ahhh, the age old question of 'where do I start' when designing a new vehicle, especially when there are so many variables to trade and so few examples to draw from. This document is an attempt to provide a starting point for the conceptual design of Orion, and to provide a framework for the preliminary design process.

### Primary Mission Goals
#### Vehicle Objectives
- [ ] Apogee of 25km
- [ ] Flight-prove our liquid rocket engine
  - [ ] Ignition
  - [ ] Throttle
  - [ ] Shut-off
- [ ] Test upgraded avionics + recovery
  - [ ] In-house deployment system
  - [ ] Stable RF downlink

#### Ground System Objectives
- [ ] Trajectory is actively tracked
  - [ ] Smooth video from ground recorded
  - [ ] Recovery ops are improved

#### Post-flight Objectives
- [ ] Recover the rocket and learn from the mission
  - [ ] Calibrate RocketPy model
  - [ ] Calibrate trajectory observation model

---

At this stage, we only care about the first - apogee.

Apogee is a neat metric - with a well-parametrised trajectory solver, it's easily calculated and can thus be used for initial optimisation.

RocketPy is well parametrised flight trajectory solver and by iterating our design with RPy in the loop, we can quickly get a feel for the design space.

It abstracts away the details of stability margins, aerodynamics, and other factors that are difficult to model and instead focuses on the key parameters that we can easily vary.

---

### Step 1: Define the baseline configuration
- [ ] For each system, identify their high-level components and expected integrated location
  - [ ] Avionics
  - [ ] Recovery
  - [ ] Engine / Propellant Feed
  - [ ] Airframe
  - [ ] Payload
---
### Step 2: Size the configuration

#### Team 1 - RocketPy
- [ ] Find a configuration which is reasonable at a first guess that hits 25km
- [ ] Inject constraints presented by team 2 - iterate until team 2 is happy

#### Team 2 - System Identification
- [ ] Whiteboard: Identify every major inter-system dependency - i.e. what drives what
- [ ] Run through each system and identify any fixed constraints - at this stage, we're only interested in Mass, Volume and Power
- [ ] Feedback intial RocketPy results to other teams to further tuning the model







