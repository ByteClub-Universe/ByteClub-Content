# Wall Jump

## Overview

The moment you realize you can jump off walls, the game transforms. Suddenly every surface is a path, every gap is a challenge, and vertical space becomes your playground. Wall jumping is one of the most satisfying movement mechanics when done right — it turns platforming from a chore into an art form.

## Core loop

1. Player jumps toward a wall
2. Player presses jump while touching the wall
3. Character pushes off wall in opposite direction
4. Player can chain wall jumps between parallel walls
5. Skilled players maintain momentum through sequences

## Design dimensions

### Input feel
- **Snap** (Celeste): Instant response, very tight timing
- **Floaty** (Ori): Longer air time, more forgiving
- **Committing** (Super Metroid): Momentum-based, carries speed
- **Sticky** (Guacamelee): Brief wall stick before jump

### Wall interaction
- **Slide** (Celeste): Slowly slide down walls
- **Stick** (Ori): Can cling to walls briefly
- **No interaction** (some games): Wall = instant jump, no sliding
- **Climb** (Super Metroid): Vertical movement on walls

### Direction control
- **Fixed angle** (Celeste): Always jumps at same angle
- **Variable** (Guacamelee): Can aim jump direction
- **Charged** (some games): Hold for higher/longer jump
- **Automatic**: Character jumps at optimal angle

### Combo potential
- **Chain jumps** (Celeste): Wall → wall → dash → wall
- **Speed building** (Super Metroid): Momentum increases through sequences
- **Reset mechanics** (Ori): Wall jump resets dash/ability
- **Rhythm-based**: Timing windows create rhythmic movement

## Techniques

### Basic wall jump
- Jump at wall → press jump → push off
- Foundation for all advanced movement

### Wall climb
- Alternate left/right wall jumps to ascend
- Requires good timing and rhythm

### Wave dash / wall boost
- Dash from wall to maintain horizontal speed
- Advanced tech for speed and precision

### Corner boost
- Jump at wall corner for extra height/speed
- Exploits geometry for advantage

## Anti-patterns

- **Too stiff**: If wall jumps feel robotic, movement loses flow
- **No visual feedback**: Players need to see when they can wall jump
- **One-speed**: If wall jumping is always the same speed, it's boring
- **Punishes failure**: Falling all the way down after one missed jump = rage quit material

## References

- Celeste: Wall jumping is buttery smooth and deeply satisfying
- Super Metroid: Wall jumping opened up speedrunning possibilities
- Guacamelee 2: Wall jumping tied into combat and exploration
- Ori and the Will of the Wisps: Wall jumping feels like flying

## Tutorials

- [Wall Jump Mechanics in Platformers](https://www.youtube.com/watch?v=2M7fW2RC1Xk) — How to implement satisfying wall jump physics and timing
- [Celeste Movement System Breakdown](https://www.youtube.com/watch?v=yorTG9at90g) — Analyzing Celeste's movement system including wall mechanics

## Image Sources

- Wall jump trajectory diagrams — Self-created physics illustrations
- Platformer layout examples — Self-created level design concepts
