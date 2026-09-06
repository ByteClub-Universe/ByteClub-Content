# Momentum-Based Movement

## Overview

This is the mechanic that makes you feel like a god when you're flowing through a level. Your character accelerates, decelerates, and carries momentum between actions. It's the difference between "I'm controlling a character" and "I AM the character."

## Core loop

1. Player provides input to move
2. Character accelerates gradually (not instant max speed)
3. Player releases input, character decelerates
4. Jumping/dashing preserves some horizontal momentum
5. Skilled players chain movements to maintain flow state

## Design dimensions

### Acceleration curve
- **Instant** (some platformers): No buildup, responsive but less physical
- **Linear** (Sonic): Steady acceleration, predictable and learnable
- **Exponential** (Celeste): Slow start, then rapid speed. Feels explosive
- **Variable** (Doom Eternal): Different weapons/modes change acceleration

### Momentum preservation
- **Full preservation** (Sonic): Keep all speed through jumps and turns
- **Partial** (Celeste): Carry ~70-80% of speed through actions
- **Minimal** (Mario): Some carryover, but mostly grounded movement
- **None** (top-down RPGs): Each movement is independent

### Air control
- **Full air control** (Celeste): Can change direction mid-air freely
- **Limited** (Doom Eternal): Some control but trajectory is mostly set
- **None** (some platformers): Locked into jump arc once airborne

### Movement tech ceiling
- **High** (Celeste): Wave dashing, hyper dashes, corner boosts
- **Moderate** (Doom Eternal): Glory kills reset dash, creating rhythm
- **Low** (casual platformers): Movement is simple by design

## Anti-patterns

- **Too slippery**: If players can't stop when they want to, it's frustrating not fun
- **No feedback**: Speed lines, camera effects, and sound sells the momentum
- **One speed**: If there's no variance between slow and fast movement, momentum is meaningless
- **Punishes speed**: If going fast makes the game harder without reward, players slow down

## References

- Celeste: The pinnacle of movement feel in 2D platformers
- Doom Eternal: Movement as combat — staying mobile IS the defense
- Sonic Mania: Classic momentum physics done right
- Metroid Dread: Fluid transitions between movement states

## Tutorials

- [Celeste Movement Deep Dive](https://www.youtube.com/watch?v=yorTG9at90g) — Analyzing how Celeste creates that addictive movement feel
- [Doom Eternal Movement & Combat Loop](https://www.youtube.com/watch?v=a0bTnDJCQCM) — How movement ties into the combat system design

## Image Sources

- Platformer tilesets — [Kenney Platformer Pack](https://kenney.nl/assets/platformer-pack) (CC0 Public Domain)
- Speed effect sprites — [Kenney Particle Pack](https://kenney.nl/assets/particle-pack) (CC0 Public Domain)
