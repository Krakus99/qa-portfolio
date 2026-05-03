# Test Plan: Horse Fence Collision (Diagonal Movement Bug)

## Title
Validate horse collision consistency with fences during diagonal movement

---

## Description
This test plan verifies that the horse in Stardew Valley does not clip through fences when the player performs diagonal movement inputs while riding alongside fence structures.

The system must ensure consistent collision detection regardless of movement direction.

---

## Repository Context
- Game: Stardew Valley
- Version: 1.6.15
- Module: Movement / Collision System
- Feature Area: Horse Riding Mechanics

---

## Objective
Ensure horse collision behaves correctly in all movement directions and prevents clipping through fence geometry.

---

## Preconditions
- Player has access to a horse
- Horse is mounted
- Fence objects with active collision are present
- Player is positioned near a fence

---

## Test Scenarios

### TC-01: Straight Movement Collision Validation
1. Mount horse
2. Move parallel to fence (vertical/horizontal)
3. Observe collision behavior
4. Ensure no clipping occurs

---

### TC-02: Diagonal Movement Collision Test (Primary Case)
1. Mount horse
2. Ride alongside fence
3. Press diagonal inputs (Forward + Left / Forward + Right)
4. Observe horse movement relative to fence

---

### TC-03: Reverse Diagonal Test
1. Repeat diagonal movement using backward inputs
2. Validate collision consistency in reverse direction

---

### TC-04: Boundary Edge Test
- Test horse movement at fence corners
- Test narrow fence gaps
- Validate collision stability in tight spaces

---

### TC-05: Repeatability Test
- Perform diagonal movement multiple times in same location
- Check for inconsistent clipping behavior

---

## Expected Result
- Horse should not clip or pass through fences in any direction
- Collision detection must be consistent for diagonal movement
- No access to restricted areas via movement exploits

---

## Failure Criteria
- Horse partially or fully passes through fences
- Collision fails only on diagonal movement
- Inconsistent collision behavior depending on input direction

---

## Risk
- Map traversal exploits
- Collision system inconsistency
- Gameplay boundary breaking
- Exploitable movement mechanics

---

## Notes
- Likely issue in diagonal movement vector collision resolution
- Possible mismatch between movement input handling and physics collision checks

---

## Tester
Emre Sedef

## Test Date
June 27, 2025
