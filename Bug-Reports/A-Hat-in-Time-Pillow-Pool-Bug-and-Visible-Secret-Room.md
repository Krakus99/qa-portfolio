# Bug Report

## Bug Details

| Field        | Value |
|-------------|-------|
| Bug Title    | Player can clip under stairs in pillow pool and access hidden area causing softlock |
| Date Found   | 5 May, 2026 |
| Game Version | A Hat in Time (Latest) |
| Tester       | Emre Sedef |

---

## Description

When the player moves to the corner of the pillow pool and interacts with the underside of the stairs, the character can clip through collision and enter an unintended area beneath the pool.

During this state, the player incorrectly transitions from swimming to walking and is able to move under the environment. This allows visibility of a hidden room that is normally locked behind progression.

Attempting to enter the hidden room results in the player becoming stuck mid-air indefinitely, causing a softlock.

---

## Steps to Reproduce

1. Launch the game  
2. Go to the pillow pool area  
3. Move to a corner with stairs  
4. Position the character under or near the stairs  
5. Jump or move into the underside of the stairs  
6. Observe clipping under the environment  
7. Move beneath the pillow pool  
8. Locate the hidden room  
9. Attempt to enter the room  

---

## Expected Result

- Player should not clip through stairs  
- Player should remain in swimming state inside the pool  
- Collision should block access to unintended areas  
- Hidden room should not be visible without required progression  
- Player should not become stuck or enter invalid states  

---

## Actual Result

- Player clips under stairs  
- Player transitions from swimming to walking under the pool  
- Player can explore unintended areas  
- Hidden room becomes visible prematurely  
- Player becomes stuck mid-air when attempting to enter the room  

---

## Frequency

Every time  

---

## Evidence

-  https://drive.google.com/file/d/1mgu2okx6VLLnJ1OBnoLmsjOhxqQ_z8C0/view?usp=sharing

---

## Bug Type

Gameplay / Collision / Physics / Progression Bug  

---

## Severity

Critical  
