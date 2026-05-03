# Test Plan: Daily Missions Gold Progression (Sell / Undo System)

## Title
Validate Daily Missions gold progression consistency during Sell & Undo item actions

## Description
This test plan verifies that selling an item and immediately undoing the action does not incorrectly affect the Daily Missions gold progression. The system must correctly rollback both inventory state and progression tracking.

---

## Repository Context
- Project: Travel Town
- Module: Economy / Daily Missions / Inventory System
- Feature Area: Sell & Undo Mechanics

---

## Objective
Ensure correct synchronization between:
- Inventory state
- Gold progression system
- Daily Missions progression tracking

---

## Preconditions
- Player has access to inventory system
- Daily Missions system is active
- At least one item exists for testing
- Stable game session

---

## Test Scenarios

### TC-01: Basic Sell & Undo Flow
1. Record initial gold progression
2. Sell an item
3. Undo sell action
4. Verify gold progression returns to initial value

---

### TC-02: State Consistency Validation
- Verify item returns to inventory after undo
- Verify gold progression rollback is complete
- Compare UI vs backend values (if accessible)

---

### TC-03: Repeated Exploit Test
1. Repeat sell → undo cycle multiple times
2. Observe progression values
3. Check for unintended accumulation

---

### TC-04: Multi-Item Handling
1. Sell multiple items
2. Undo last action
3. Verify progression consistency

---

### TC-05: Stress Input Test
- Perform rapid sell/undo actions
- Check for desync, delay, or incorrect updates

---

## Expected Result
- Selling increases gold progression correctly
- Undo fully reverts:
  - Inventory state
  - Gold progression value
- No duplication or accumulation of progression
- UI and backend remain synchronized

---

## Failure Criteria
- Gold progression increases after undo
- Inventory restored but progression not reverted
- UI/backend mismatch
- Exploitable progression gain via repeated actions

---

## Risk
- Economy exploitation
- Progression inflation
- Client/server desynchronization
- Reward imbalance in Daily Missions

---

## Notes
- Possible missing rollback logic in economy transaction system
- Likely event-based progression tracking issue

---

## Tester
Emre Sedef
