- **Test Scenario ID:** TS-002
- **Feature Tested:** Horse Riding
- **Preconditions:**
    - The horse must be mounted by the player.
    - The player must be near a fence with collision enabled.
- **Test Steps:**
    1. Mount the horse.
    2. Approach a fence and ride alongside it vertically.
    3. While riding next to the fence, press forward and left (or right) keys simultaneously to move diagonally toward the fence.
    4. Observe that the horse clips through or passes inside the fence.
- **Expected Result:**
    - The horse should **not pass through or clip into the fence** when moving diagonally. Collision detection must prevent the horse from entering the fence boundary at all times.
- **Actual Result:**
    - When moving diagonally next to the fence, the horse **clips through and partially passes inside the fence**, allowing access to restricted areas.
- **Test Date:** June 27, 2025
- **Tester:** Emre Sedef
