## Bug Details

| **Bug Title** | Bodyguard NPC disappears for player who hasn't completed Qi's quest in multiplayer, causing softlock at Casino entrance |
| --- | --- |
| **Date Found** | 16 June 2025 |
| **Game Version** | Stardew Valley v1.6.15 - Multiplayer (Steam, PC) |
| **Tester** | Emre Sedef (Player 2) |

## Description

In a multiplayer session, when Player 1 completes Qi's continuation quest and Player 2 does not, the bodyguard outside the Casino in the desert disappears for both players. However, Player 2 - who did not complete the quest - is still unable to enter the Casino and is forcefully teleported back to the entrance as if the bodyguard is still blocking entry. This causes visual inconsistency and prevents progress for Player 2.

## Steps to Reproduce

1. Start a multiplayer session with two players (Player A and Player B)
2. Ensure both players have not yet completed Qi's continuation quest
3. Let only Player A complete the quest
4. Travel to the desert with Player B
5. Observe the Casino entrance

## Expected Result

The bodyguard should remain visible to Player B until they complete the quest themselves. If the bodyguard is gone, Player B should be allowed inside the Casino.

## Actual Result

- The bodyguard disappears for Player B (visually)
- Player B cannot enter the Casino and gets teleported back to the entrance
- No message or feedback is shown explaining the restriction

## Evidence

<img width="1920" height="1080" alt="casino_entrance" src="https://github.com/user-attachments/assets/999b4a4b-8782-4643-a289-0c978ae4d18d" />

https://github.com/user-attachments/assets/c682634c-8d13-4035-a195-1398bd2c81f1



## Bug Type

- Visual Bug
- Logic Bug
- Sync / Multiplayer State Inconsistency

## Severity

<aside>
Medium - Blocks access to content in multiplayer; inconsistent behavior

</aside>
