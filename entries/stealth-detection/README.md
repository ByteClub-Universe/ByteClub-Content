# Stealth Detection

## Overview

Stealth detection is the invisible handshake between player and AI. The player is trying to not be seen, and the AI is trying to catch them. A good system gives the player clear rules to work with while keeping the tension high. A bad system feels random and unfair.

## Core loop

1. Player enters enemy perception range
2. Enemy processes detection (sight, sound, other cues)
3. Detection state transitions: idle → suspicious → alert → combat
4. Player has windows to react at each transition
5. Clear communication of enemy state at all times

## Detection channels

### Visual detection
- **Line of sight**: Raycast from enemy eyes, blocked by obstacles
- **Detection cone**: Finite field of view (typically 60-120 degrees)
- **Distance falloff**: Closer = faster detection
- **Lighting**: In darkness = harder to spot (classic stealth trope)
- **Disguises**: Some systems (Hitman) add identity-based detection layers

### Audio detection
- **Footstep radius**: Running is louder than walking
- **Environmental sound**: Rain, machinery cover your noise
- **Gunshots**: Instant high alert in the area
- **Object sounds**: Knocking over stuff = bad

### State machine
- **Idle**: Patrol, no awareness
- **Suspicious**: Heard/saw something, investigating
- **Alert**: Confirmed enemy, calling for backup / engaging
- **Combat**: Full aggression, chasing player

### NPC communication
- **Visual confirmation**: Guard sees body → alerts others
- **Radio calls**: Can be intercepted or jammed
- **Sound propagation**: Gunshot heard by nearby guards
- **Knowledge transfer**: "I saw something" → others investigate same area

## Anti-patterns

- **Instant detection**: No reaction time = no counterplay
- **Omniscient AI**: Guards magically know your location through walls
- **No state feedback**: Players can't tell if they've been spotted
- **Binary states**: Going from "nothing" to "full alert" with no middle ground
- **Memory issues**: AI forgetting you were just standing there 2 seconds ago

## References

- Metal Gear Solid V: The best stealth AI system ever made — dynamic, emergent, fair
- Hitman 3: Layered disguise system with social stealth
- Alien: Isolation: The alien's detection is genuinely terrifying
- The Last of Us Part II: Balanced stealth with accessible options

## Tutorials

- [Stealth AI System in Unity](https://www.youtube.com/watch?v=8o-iq1bNRqY) — Building vision cones, state machines, and investigation behavior
- [Hitman AI Design Analysis](https://www.youtube.com/watch?v=GLOxH9LZXTo) — Deep dive into Hitman's social stealth and NPC awareness systems

## Image Sources

- AI behavior flowcharts — Self-created diagrams
- Vision cone visualizations — Inspired by [Redblobgames AI tutorials](https://www.redblobgames.com/) (referenced with permission)
