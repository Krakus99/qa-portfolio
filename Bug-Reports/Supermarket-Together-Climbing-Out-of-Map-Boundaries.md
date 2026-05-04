# Bug Report

## Bug Details

**Bug Title:** Player can exit map boundaries using ladder and street lamp  
**Date Found:** May 5, 2026  
**Game Version:** Supermarket Together (Latest)  
**Tester:** Emre Sedef  

---

## Description

When a player places a ladder next to a street lamp located at the corner of the map, they can climb onto the lamp and use it to bypass map boundaries. By repositioning the ladder and adjusting their position, the player is able to move out of boundaries of the playable area.

This issue breaks map boundary restrictions and allows unintended exploration of out-of-bounds areas. The system fails to properly enforce collision on environmental objects and map edges.

---

## Steps to Reproduce

1. Launch the game  
2. Move to a map corner where a street lamp is located  
3. Place a ladder next to the street lamp  
4. Climb the ladder  
5. Move onto the top of the street lamp  
6. Take the ladder again when you are on the street lamp  
7. Move the corner of the map
8. Drop the ladder at the exact point while aiming the exact point
9. Once you fly, move forward to go out of the map

---

## Expected Result
  
- Collision detection should block climbing unintended objects  
- Map boundaries should prevent any out-of-bounds movement  

---

## Actual Result
 
- Player can exit the map boundaries  

---

## Frequency

Every time  

---

## Evidence

https://drive.google.com/file/d/1yvLF1afgKpd6dHPUojHWRCFt9fgTnETs/view?usp=sharing

---

## Bug Type

Gameplay / Collision / Level Design Bug  

---

## Severity

High  
