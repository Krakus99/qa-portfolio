### 1. Bug Report ID

BR-003

### 2. Bug Title

Money progression on Daily Missions goes up when player sell an item and undo selling.

### 3. Tested Game / Version

Travel Town 2.12.1511 | 81812 (iOS / Android)

### 4. Test Date

9 April 2025

### 5. Tester

Emre Sedef

### 6. Preconditions

- Player is in the game with Daily Missions active
- At least one item available in inventory to sell
- Daily Missions progress is visible

### 7. Steps to Reproduce

1. Open the game and navigate to **Daily Missions**
2. Check the current money progression value
3. Sell any item from the inventory
4. Immediately undo the selling action
5. Observe the money progression in Daily Missions

### 8. Expected Result

Money progression should remain unchanged. Selling and undoing an item should not affect Daily Missions progress.

### 9. Actual Result

Money progression increases after undoing the sale of an item.

### 10. Priority / Severity

Medium 

### 11. Notes

This issue may also affect Daily Events based on additional testing, suggesting a potential economy progression tracking bug.
