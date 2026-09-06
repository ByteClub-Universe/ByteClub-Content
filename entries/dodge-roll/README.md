# Dodge Roll

## Overview

Dodge rolling is the classic "get out of danger free" move. You hit a button, your character tumbles in a direction, and for a few sweet frames nothing can touch you. It's the mechanic that separates the players who survive from the ones who rage quit.

## Core loop

1. Player reads incoming danger (attack, projectile, hazard)
2. Player commits to a direction and hits dodge
3. During i-frames: invincible, feels amazing
4. After i-frames: recovery window where you're stuck and vulnerable
5. If you rolled into a worse position... that's on you

## Design dimensions

### Invincibility frames (i-frames)
- **Generous** (Hades): ~15+ frames. Very forgiving, encourages aggression
- **Moderate** (Dead Cells): ~10 frames. Rewards timing without being punishing
- **Strict** (Dark Souls): ~7-13 frames depending on build. You WILL get hit if you panic roll

### Recovery time
- **Snappy** (Hades): Almost instant. You can chain dodges quickly
- **Moderate** (Enter the Gungeon): Short recovery, but you can't spam
- **Heavy** (Dark Souls): Long recovery. Roll at the wrong time and you're eating damage

### Distance & direction
- **8-directional** (Hades): Full freedom, very responsive
- **4-directional** (Dark Souls 1): Limited, more strategic
- **Fixed direction** (some platformers): Only rolls forward, becomes an offensive tool too

### Commitment level
- **No commitment** (Hades dash): Can cancel into other actions almost immediately
- **Partial commitment** (Dead Cells): Brief lockout before you can act again
- **Full commitment** (Dark Souls): You're locked into that roll, better hope it was the right call

## Anti-patterns

- **Spam-friendly**: If players can roll无限 times with no recovery, there's no decision-making
- **No visual feedback**: Players need to FEEL when i-frames start and end
- **Same dodge for everything**: One dodge type for all situations gets stale fast
- **Invisible recovery**: If recovery frames aren't communicated, players feel cheated

## References

- Dark Souls: The gold standard for committed, weighty dodge rolls
- Hades: Dash-based movement that doubles as combat repositioning
- Enter the Gungeon: Dodge roll with a bullet-time effect
- Dead Cells: Fluid dodge that integrates with the platforming

## Tutorials

- [How to Make a Dodge Roll in Godot 4](https://www.youtube.com/watch?v=dsyIluXs7dU) — Brackeys covers implementing i-frames, animation state machines, and recovery windows
- [Souls-Like Dodge Roll Tutorial](https://www.youtube.com/watch?v=G5aatedpGqI) — Building a committed dodge system with stamina cost and recovery frames

## Image Sources

- Character sprite animations — [Kenney Game Assets](https://kenney.nl/assets) (CC0 Public Domain)
- UI mockup elements — [Kenney UI Pack](https://kenney.nl/assets/ui-pack) (CC0 Public Domain)
