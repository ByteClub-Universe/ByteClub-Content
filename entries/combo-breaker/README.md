# Combo Breaker

## Overview

You're getting juggled. Your health is melting. You need out NOW. Combo breakers let you spend a resource to break free from an opponent's combo and reset to neutral. It's the mechanic that keeps matches competitive when one player is clearly outclassing the other.

## Core loop

1. Player A starts a combo on Player B
2. Player B is locked into hitstun/blockstun
3. Player B spends a resource (meter, life, cooldown) to break free
4. Combo resets to neutral or advantage for the breaker
5. Both players reassess — now what?

## Design dimensions

### Resource cost
- **Life** (Killer Instinct): Costs health — you're trading survival for freedom
- **Meter** (Mortal Kombat): Uses offensive/defensive meter
- **Stock** (some systems): Limited breakers per round
- **Cooldown** (Guilty Gear): Can break, but then you can't for a while

### Timing windows
- **During hitstun only**: Can only break when being actively hit
- **During blockstun**: Can break while blocking a string too
- **Specific windows**: Only at certain points in the combo (e.g., after a launcher)
- **Freeform**: Break at any time, but the cost scales with combo length

### Combo counter interaction
- **No scaling** (Mortal Kombat): Break whenever, fixed cost
- **Scaling cost** (Killer Instinct): Later in combo = more expensive to break
- **Combo counter**: Some games show when breakers are available

### Mind-game layer
- **Baiting breaks**: Experienced players predict breaks and reset combos to bait them out
- **Resource tracking**: Knowing when your opponent is low on break resources
- **Staggered pressure**: Mixing combo lengths to force early breaks

## Anti-patterns

- **No breaker**: If combos are long with no escape, matches feel one-sided
- **Free breaker**: If breaking costs nothing, combos become pointless
- **Unreactable**: If the break window is too small, it becomes luck not skill
- **Too expensive**: If breaking costs more than taking the combo, why bother

## References

- Killer Instinct: THE combo breaker game — the "C-C-C-COMBO BREAKER" is iconic
- Mortal Kombat 11: Defensive meter-based break system
- Guilty Gear Strive: Burst system as combo breaker
- Tekken 8: Heat system adds combo extension AND escape options

## Tutorials

- [Combo Breaker System Design](https://www.youtube.com/watch?v=nBHevCjODcs) — Analysis of combo breaker mechanics across fighting games
- [Killer Instinct Combo System Breakdown](https://www.youtube.com/watch?v=Gg1E3Z14gRM) — Deep dive into KI's combo and breaker system architecture

## Image Sources

- Fighting game UI elements — [Kenney Game Assets](https://kenney.nl/assets) (CC0 Public Domain)
- Combo counter mockups — Self-created UI concepts
