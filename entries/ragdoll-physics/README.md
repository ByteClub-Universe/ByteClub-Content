# Ragdoll Physics

## Overview

Ragdoll is what happens when you replace canned death animations with real-time physics simulation. Enemies flop, tumble, and crash into things in unpredictable ways. Sometimes it's realistic and immersive. Sometimes it's the funniest thing you've ever seen. Either way, players LOVE it.

## Core loop

1. Character is alive, playing standard animations
2. Character dies or enters ragdoll state
3. Physics simulation takes over (no more animation)
4. Body interacts with environment realistically
5. Emergent moments happen naturally

## Implementation approaches

### Full ragdoll (GTA V)
- **Complete physics**: Entire body is physics-driven
- **Joint constraints**: Limbs have realistic limits
- **Momentum transfer**: Bodies carry impact force
- **Environmental interaction**: Collide with everything

### Hybrid (Elden Ring)
- **Animation blend**: Blend between animation and ragdoll
- **Partial ragdoll**: Some parts physics-driven, others animated
- **Triggered ragdoll**: Only on specific events (backstabs, death)
- **Controlled chaos**: Physics feel dramatic but predictable

### Physics playground (Human Fall Flat)
- **Full body control**: Player controls physics directly
- **Wobbly movement**: Physics ARE the gameplay
- **Collaborative physics**: Multiplayer physics chaos
- **Puzzle integration**: Physics used for problem-solving

### Comedy physics (Gang Beasts)
- **Exaggerated**: Physics are unrealistic but hilarious
- **Sticky**: Characters grab and stick to surfaces
- **Bouncy**: Exaggerated bounce and impact
- **Environmental hazards**: Physics interact with kill zones

## Design dimensions

### Realism vs. fun
- **Realistic** (GTA V): Physics simulate real body movement
- **Semi-realistic** (Elden Ring): Physics enhanced for drama
- **Exaggerated** (Human Fall Flat): Physics prioritized for humor
- **Absurd** (Gang Beasts): Physics are the comedy

### Transition quality
- **Smooth blend**: Animation fades into physics naturally
- **Hard cut**: Instant switch to ragdoll
- **Gradual**: Physics influence increases over time
- **Event-triggered**: Specific actions trigger ragdoll

### Environmental interaction
- **Collision**: Bodies hit walls, floors, objects
- **Bounce**: Physics material properties (rubber, stone)
- **Drag**: Bodies slow down on surfaces
- **Stacking**: Bodies pile up on each other

## Emergent gameplay

### Comedy moments
- **Funny deaths**: Unexpected physics outcomes
- **Chain reactions**: One ragdoll hits another
- **Environmental chaos**: Bodies flying off cliffs
- **Player expression**: Creative uses of physics

### Gameplay impact
- **Cover**: Ragdolled enemies become temporary cover
- **Obstacles**: Bodies block paths or doors
- **Weapons**: Ragdoll bodies can be used as weapons (Human Fall Flat)
- **Physics puzzles**: Ragdoll becomes a puzzle element

## Anti-patterns

- **Too floaty**: If bodies feel weightless, immersion breaks
- **Too stiff**: If ragdoll feels robotic, it defeats the purpose
- **Performance cost**: Heavy physics can tank framerates
- **Inconsistent**: If ragdoll works sometimes but not others, it feels buggy
- **Overused**: If every death is ragdoll, it loses impact

## References

- GTA V: Ragdoll is part of the game's identity
- Human Fall Flat: Physics ARE the game
- Gang Beasts: Comedy physics that make for great multiplayer moments
- Elden Ring: Ragdoll adds drama to boss kill animations

## Tutorials

- [Ragdoll Physics in Games](https://www.youtube.com/watch?v=KJ4qADfvOfY) — How to implement ragdoll systems that feel good and perform well
- [Physics-Based Game Design](https://www.youtube.com/watch?v=LyV4o7F5P3s) — Using physics to create emergent gameplay and player expression

## Image Sources

- Ragdoll joint diagrams — Self-created physics illustrations
- Physics material comparison — Self-created visual guides
