## Bug Details

| **Bug Title** | Money progression on Daily Missions goes up when player sell an item and undo selling. |
| --- | --- |
| **Date Found** | 9 April 2025 |
| **Game Version** | Travel Town 2.12.1511 | 81812 (iOS / Android) |
| **Tester** | Emre Sedef  |

## Description

When a player sells an item from their inventory and then immediately undoes the selling action, the money progression on Daily Missions incorrectly increases. This behavior allows players to artificially inflate their money progression by repeatedly selling and undoing items. The Daily Missions system should only register actual earned money, and reversing a sale should not impact mission progress.

## Steps to Reproduce

1. Open the game and navigate to Daily Missions.
2. Check the current money progression value.
3. Sell any item from the inventory.
4. Immediately undo the selling action.
5. Observe the money progression in Daily Missions.

## Expected Result

Money progression should remain the same; selling and undoing an item should not affect Daily Missions progress.

## Actual Result

- Money progression value increases after undoing the selling of an item.

## Frequency

Every time

## Evidence

https://drive.google.com/file/d/1UyonyqsTKh1f-nnCnCaPUvqGSmvusBfv/view?usp=drive_link

I did some tests on daily events, but I am sure that it works on daily missions too. 

## Bug Type

- Progression / Economy Bug

## Severity

<aside>
Medium

</aside>
