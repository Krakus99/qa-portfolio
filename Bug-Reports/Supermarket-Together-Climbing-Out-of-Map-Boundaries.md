# Bug Report

## Bug Details

**Bug Title:** Player can exit map boundaries using ladder and street lamp  
**Date Found:** June 27, 2025  
**Game Version:** Supermarket Together (Latest)  
**Tester:** Emre Sedef  

---

## Description

When a player places a ladder next to a street lamp located at the corner of the map, they can climb onto the lamp and use it to bypass map boundaries. By repositioning the ladder and adjusting their position, the player is able to move خارج the playable area.

This issue breaks map boundary restrictions and allows unintended exploration of out-of-bounds areas. The system fails to properly enforce collision on environmental objects and map edges.

---

## Steps to Reproduce

1. Launch the game  
2. Move to a map corner where a street lamp is located  
3. Place a ladder next to the street lamp  
4. Climb the ladder  
5. Move onto the top of the street lamp  
6. Reposition the ladder if needed  
7. Attempt to move beyond the map boundary  

---

## Expected Result

- Player should not be able to stand on the street lamp  
- Collision detection should block climbing unintended objects  
- Map boundaries should prevent any out-of-bounds movement  

---

## Actual Result

- Player can climb onto the street lamp  
- Player can use the ladder to gain positional advantage  
- Player can exit the map boundaries  

---

## Frequency

Every time  

---

## Evidence



---

## Bug Type

Gameplay / Collision / Level Design Bug  

---

## Severity

High  
