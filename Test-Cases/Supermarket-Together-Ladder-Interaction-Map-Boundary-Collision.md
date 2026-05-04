# Test Scenario: TS-003

## Feature Tested
Ladder Interaction / Map Boundary Collision  

---

## Preconditions
- The player must have access to a ladder  
- The player must be near a map corner with a street lamp  
- The game must be in a normal playable state  

---

## Test Steps
1. Place the ladder near the street lamp  
2. Climb the ladder  
3. Move onto the top of the street lamp  
4. Reposition the ladder beneath the player if needed  
5. Attempt to move beyond the map boundary  
6. Observe player behavior  

---

## Expected Result
- The player should not be able to stand on the street lamp  
- Collision detection must prevent climbing unintended objects  
- Map boundaries must block movement outside the playable area  

---

## Actual Result
- The player can climb onto the street lamp  
- The player can reposition the ladder to gain advantage  
- The player can move beyond the map boundary  

---

## Test Date
June 27, 2025  

## Tester
**Emre Sedef**
