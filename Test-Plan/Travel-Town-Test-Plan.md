Test Plan
Title

Validate Daily Missions gold progression consistency during Sell & Undo item actions

Description

This test plan verifies that selling an item and immediately undoing the action does not incorrectly affect the Daily Missions gold progression. The system must ensure proper state rollback in both frontend (UI) and backend (progression tracking).

Repository Context
Project: Travel Town (or related game repo)
Module: Economy / Daily Missions / Inventory System
Area: Sell & Undo mechanics
Objective

Ensure that item sell and undo actions correctly maintain synchronization between:

Inventory state
Gold progression tracking
Daily Missions progression system
Preconditions
Player has access to inventory system
Daily Missions system is active
At least one item is available for creation and selling
Game session is stable (no reconnect/state reset)
Test Scenarios
TC-01: Basic Sell & Undo Flow
Record initial gold progression
Sell an item
Undo the sell action
Verify gold progression matches initial state
TC-02: State Consistency Check
Validate item returns to inventory after undo
Validate gold progression rollback is complete
Compare UI value vs backend stored value (if accessible)
TC-03: Repeated Exploit Attempt
Repeat sell → undo cycle multiple times
Check if progression accumulates incorrectly
TC-04: Multi-item Handling
Sell multiple items
Undo last action
Verify progression consistency
TC-05: Stress Input Test
Perform rapid sell/undo actions
Check for desync or delayed rollback issues
Expected Result
Sell increases gold progression correctly
Undo fully reverts:
Inventory state
Gold progression value
No accumulation or duplication of progression values
UI and backend remain synchronized
Failure Criteria
Gold progression increases after undo
Item state restored but progression not reverted
Mismatch between UI and backend values
Exploitable progression gain via repeat actions
Risk Assessment
Economy system exploitation
Progression inflation in Daily Missions
Desync between client/server state
Potential reward imbalance
Notes
This issue may indicate a missing rollback handler in economy transaction system
Could be related to event-based progression tracking rather than state-based validation
Tester

Emre Sedef
