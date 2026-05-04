# Test Scenario: TS-004

## Feature Tested
Swimming Mechanics / Stairs Collision / Boundary System  

---

## Preconditions
- The player must be in the pillow pool area  
- Stairs must exist at the edge/corner of the pool  
- The player must be in a normal gameplay state  

---

## Test Steps
1. Move to the corner of the pillow pool  
2. Position the character under or near the stairs  
3. Jump or move into the underside of the stairs  
4. Observe that the character clips under the stairs  
5. Attempt to move beneath the pillow pool  
6. Observe player movement behavior  
7. Locate the hidden room under the pool  
8. Attempt to enter the hidden room  

---

## Expected Result
- The player should not clip under the stairs  
- The player should remain in swimming state inside the pool  
- Collision must prevent access to unintended areas  
- Hidden room should not be visible without required abilities  
- The player should not become stuck or enter invalid states  

---

## Actual Result
- The player clips under the stairs  
- The player transitions from swimming to walking under the pool  
- The player can explore unintended areas  
- The hidden room becomes visible prematurely  
- Attempting to enter the room causes the player to become stuck mid-air indefinitely  

---

## Test Date
June 27, 2025  

## Tester
**Emre Sedef**
