# Charge Attack

## Overview

The high-risk, high-reward move. Hold a button, your character powers up, release for massive damage. You're a sitting duck while charging, so every successful charge attack feels earned. It's the mechanic that rewards reading the fight and picking your moment.

## Core loop

1. Player holds attack button
2. Character enters charge state (visual/audio feedback)
3. Damage scales with charge time
4. Player releases at the right moment
5. Devastating hit connects (or miss = punishment)

## Design dimensions

### Charge time
- **Short** (Hollow Knight nail art): ~0.5-1 second
- **Medium** (Monster Hunter): ~1-3 seconds
- **Long** (Dark Souls heavy attacks): ~2-4 seconds
- **Variable**: Charge time depends on weapon/upgrade

### Damage scaling
- **Linear**: More charge = proportionally more damage
- **Threshold**: Certain charge levels unlock damage tiers
- **Exponential**: Full charge does massive damage
- **Binary**: Partial or full charge, no in-between

### Movement during charge
- **Immobile** (Monster Hunter): Locked in place while charging
- **Slow movement** (Hollow Knight): Can inch forward
- **Full movement** (some games): Charge while dodging
- **Dash cancel** (Hollow Knight): Can cancel charge into dash

### Feedback systems
- **Visual glow**: Character/weapon glows as charge builds
- **Sound build**: Audio pitch/intensity increases
- **Controller vibration**: Haptic feedback for charge level
- **UI indicator**: Charge meter on screen

## Combat integration

### Opening windows
- **Post-dodge**: Dodge enemy attack, charge during recovery
- **Stagger**: Enemy stunned = free charge opportunity
- **Ranged pressure**: Charge from safe distance
- **Teammate distraction**: Multiplayer: teammate holds aggro

### Risk-reward balance
- **Commitment**: Can't cancel late = high risk
- **Recovery**: Long recovery after charge = punished for missing
- **Resource cost**: Some charge attacks cost stamina/mana
- **Opportunity cost**: Charging = not attacking normally

## Anti-patterns

- **No vulnerability**: If charging has no downside, it's just "press for big damage"
- **Too slow**: If charge time exceeds enemy attack windows, it's unusable
- **No feedback**: If players can't tell charge level, timing is guesswork
- **Always optimal**: If charge attack is always the best option, normal attacks are pointless

## References

- Hollow Knight: Nail arts are optional but deeply satisfying
- Monster Hunter Rise: Charge attacks are core to great sword gameplay
- Metroid Dread: Charge beam is essential for progression
- Dark Souls: Heavy/charge attacks reward patience and positioning

## Tutorials

- [Charge Attack Design in Action Games](https://www.youtube.com/watch?v=G5aatedpGqI) — How to design charge mechanics that feel rewarding and fair
- [Hollow Knight Combat Mechanics Analysis](https://www.youtube.com/watch?v=81a_ky2yKtc) — Deep dive into Hollow Knight's combat system including charge mechanics

## Image Sources

- Charge state progression diagrams — Self-created visual guides
- Combat timing windows — Self-created frame data illustrations
