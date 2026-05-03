# Test Plan: Multiplayer Qi Quest Synchronization – Casino Bodyguard Bug

## Title
Validate multiplayer synchronization of Qi’s quest state and Casino bodyguard NPC behavior

---

## Description
This test plan verifies that Qi’s quest progression is correctly synchronized between players in a multiplayer session and that the Casino entrance behavior (bodyguard NPC visibility and access control) is consistent for all players.

The system must ensure that quest completion state and NPC behavior are properly synchronized across all connected clients.

---

## Repository Context
- Game: Stardew Valley
- Version: 1.6.15
- Module: Multiplayer / Quest System / NPC Logic
- Feature Area: Qi Quest Continuation / Casino Access

---

## Objective
Ensure consistent multiplayer state synchronization for:
- Quest completion status
- NPC visibility (Bodyguard at Casino entrance)
- Player access to Casino area

---

## Preconditions
- Multiplayer session active (minimum 2 players)
- Player A and Player B are connected in same world
- Qi’s quest continuation is available
- Player A can complete quest while Player B does not

---

## Test Scenarios

### TC-01: Quest Completion Sync Validation
1. Player A completes Qi’s quest continuation
2. Player B does not complete the quest
3. Verify quest state across both clients

---

### TC-02: NPC Visibility Consistency Test
1. Move both players to Casino entrance
2. Observe bodyguard NPC visibility for Player A and Player B
3. Compare NPC state across both clients

---

### TC-03: Access Restriction Validation
1. Player B attempts to enter Casino
2. Observe teleport/denial behavior
3. Validate correct feedback is shown

---

### TC-04: State Desynchronization Check
- Check if NPC is visible/invisible inconsistently between players
- Verify server vs client state alignment

---

### TC-05: Repeat Session Test
- Restart multiplayer session
- Repeat quest completion scenario
- Validate persistence of correct synchronization state

---

## Expected Result
- Qi quest completion state must be synchronized correctly across players
- Bodyguard NPC visibility must be consistent for all players
- If access is restricted, all players should see the same restriction state
- Player should receive proper feedback when blocked

---

## Failure Criteria
- NPC disappears for one player but not others
- Player is blocked without consistent NPC presence
- Players experience different world states
- Teleport/blocking occurs without explanation or synced state

---

## Risk
- Multiplayer state desynchronization
- Progression inconsistency between players
- Broken immersion due to inconsistent NPC behavior
- Potential softlock in multiplayer progression flow

---

## Notes
- Likely issue in multiplayer quest state replication
- Possible mismatch between client-side NPC rendering and server-side quest flags

---

## Tester
Emre Sedef

## Test Date
June 16, 2025
