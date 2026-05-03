**Test Plan
1. Objective

Verify that selling an item and undoing the action does not incorrectly affect Daily Missions gold progression and that the system properly handles rollback of economy-related actions.

2. Scope
Daily Missions gold progression system
Inventory item creation, selling, and undo functionality
Economy tracking and rollback logic
UI and backend consistency of gold values
3. Test Approach
Functional testing of sell and undo mechanics
State validation before and after each action
Regression testing on progression system
Repeated action testing to detect exploit behavior
Comparison of UI vs backend progression values
4. Test Scenarios
Basic Flow
Record gold progression → sell item → undo → verify full rollback
Consistency Checks
Verify item state returns correctly after undo
Verify gold progression matches pre-action state
Exploit Testing
Repeat sell/undo cycles multiple times
Check for artificial progression increase
Edge Cases
Sell multiple items and undo last action
Perform actions rapidly (stress input testing)
5. Preconditions
Player has access to inventory
Daily Missions system is active and visible
At least one item is available for creation/selling
6. Expected Result
Selling increases gold progression correctly
Undo action fully reverts:
Item state
Gold progression
No unintended accumulation of progression should occur
7. Pass / Fail Criteria
Pass: Gold progression correctly reverts after undo
Fail: Any mismatch between item state and progression system
8. Risk
Economy exploitation via sell/undo loops
Progression system desynchronization
Potential reward inflation in Daily Missions
9. Test Data
Single item
Multiple items
Different item values (low / high gold value items)
10. Tester / Date
Tester: Emre Sedef
Test Date: 9 April 2025**
