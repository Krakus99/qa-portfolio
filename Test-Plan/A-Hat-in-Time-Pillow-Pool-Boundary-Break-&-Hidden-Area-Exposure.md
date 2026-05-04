# QA Test Plan: Pillow Pool Boundary Break & Hidden Area Exposure

## Title
Validate collision integrity and movement behavior in pillow pool area when interacting with ladder edges

---

## Description
This test plan verifies that the player cannot bypass intended movement mechanics in the pillow pool by clipping under ladders. Normally, the player should be in a swimming state inside the pool. However, by moving into a corner and interacting with the underside of a ladder, the player can transition into a walking state beneath the pool, access unintended areas, and break progression boundaries.

---

## Repository Context
- **Project:** A Hat in Time  
- **Module:** Player Movement / Physics / Collision System  
- **Feature Area:** Swimming Mechanics & Boundary Enforcement  

---

## Objective
Ensure correct synchronization between:

- Swimming vs walking state transitions  
- Ladder collision and interaction system  
- Environment boundary enforcement  
- Hidden area visibility restrictions  

---

## Preconditions
- Player has access to the pillow pool area  
- A ladder exists at the edge/corner of the pool  
- Player is in normal gameplay state  
- Game physics and collision are functioning normally  

---

## Test Scenarios

### TC-01: Ladder Underside Clipping
1. Move to the corner of the pillow pool  
2. Position character under/near the ladder  
3. Jump or move into the underside of the ladder  
4. Observe if the character gets stuck or clips  

---

### TC-02: State Transition Break (Swim → Walk)
1. Perform clipping under the ladder  
2. Observe player movement behavior  
3. Check if the character transitions from swimming to walking  

---

### TC-03: Under-Pool Exploration
1. After clipping, attempt to move beneath the pillow pool  
2. Observe if player can freely walk in unintended areas  

---

### TC-04: Hidden Room Exposure
1. Navigate under the pool  
2. Locate the hidden room  
3. Verify visibility without required progression  

---

### TC-05: Entry Attempt to Hidden Room
1. Attempt to enter the hidden room  
2. Observe player behavior  

---

### TC-06: Infinite Air Suspension Bug
1. Attempt to enter the hidden room  
2. Observe if the character becomes stuck mid-air  
3. Check if movement is disabled or physics breaks  

---

## Expected Result
- Player should remain in swimming state inside the pillow pool  
- Player should not clip under ladders  
- Collision should prevent entry into unintended areas  
- Hidden rooms should not be visible without required abilities  
- Player should not become stuck or suspended in air  

---

## Actual Result
- Player can clip under the ladder  
- Player transitions into walking state beneath the pool  
- Player can explore unintended areas  
- Hidden room becomes visible prematurely  
- Attempting to enter the room causes the player to be stuck mid-air indefinitely  

---

## Failure Criteria
- Player exits intended swimming state unexpectedly  
- Player accesses restricted or hidden areas  
- Collision system fails at ladder/environment interaction  
- Player becomes stuck in an unrecoverable state  

---

## Risk
- Gameplay break / immersion loss  
- Progression bypass  
- Softlock (player stuck in air)  
- Physics system instability  

---

## Notes
- Possible collision gap between ladder and pool boundary  
- Incorrect state transition trigger (swim → walk)  
- Missing fail-safe outside valid navigation area  
- Hidden content not properly gated by progression  

---

## Tester
**Emre Sedef**
