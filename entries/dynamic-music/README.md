# Dynamic Music

## Overview

Static soundtracks are cool, but dynamic music? That's when the game becomes a music video and YOU'RE the director. The music layers in and out based on what's happening — combat, exploration, danger, victory. It turns mundane moments into epic ones.

## Core loop

1. Player enters a gameplay state (exploration, combat, danger)
2. System detects state change
3. Music layers crossfade or stack based on intensity
4. Player feels the emotional shift without consciously noticing
5. Transition back when state changes

## Design dimensions

### Layering approach
- **Horizontal resequencing** (Hades): Switch between different tracks entirely
- **Vertical layering** (Doom Eternal): Stack instrument layers on top of each other
- **Adaptive stems** (Red Dead Redemption 2): Individual instrument stems fade in/out
- **Hybrid**: Mix of approaches depending on context

### Intensity mapping
- **Combat intensity**: More enemies = more layers
- **Health-based**: Low health = more frantic music
- **Proximity**: Getting close to danger ramps up
- **Player aggression**: Attacking more = harder music
- **Exploration state**: Finding something new triggers a shift

### Transition quality
- **Beat-matched**: Transitions happen on beat boundaries (cleanest)
- **Crossfade**: Gradual blend between states (smoothest)
- **Hard cut**: Immediate switch (most jarring, sometimes intentional)
- **Stinger**: Short musical flourish to bridge transitions

### Emotional range
- **Tension build**: Subtle layers adding unease
- **Combat peak**: Full orchestra/band hitting hard
- **Victory/relief**: Release of tension, calming down
- **Exploration wonder**: Open, ambient, curious

## Anti-patterns

- **Abrupt transitions**: Jumping between tracks with no blending sounds terrible
- **No variation**: If the music doesn't change during intense moments, it's wasted potential
- **Over-layering**: Too many layers = cacophony instead of music
- **Ignoring player state**: Music that doesn't respond to what the player is doing

## References

- Doom Eternal: Mick Gordon's adaptive soundtrack is legendary
- Hades: Music shifts seamlessly between rooms and combat
- Red Dead Redemption 2: Ambient world music that breathes with the environment
- Celeste: Adaptive music in boss fights reflects player struggle

## Tutorials

- [Dynamic Music Systems in Games](https://www.youtube.com/watch?v=7pkqRMI5-8w) — Overview of FMOD and adaptive music implementation techniques
- [How Doom Eternal's Music Works](https://www.youtube.com/watch?v=xyE2Qe6vBqY) — Analysis of Mick Gordon's adaptive soundtrack design

## Image Sources

- Audio waveform visualizations — Self-created diagrams
- FMOD middleware screenshots — FMOD (educational use)
