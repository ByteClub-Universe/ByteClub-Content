# Dynamic Difficulty Adjustment

## Overview

DDA is the game secretly adjusting difficulty based on how you're doing. Dying a lot? Enemies get slightly weaker. Dominating? More enemies spawn. The goal is keeping you in that sweet spot of challenge without frustration. Left 4 Dead's AI Director is the GOAT of this.

## Core loop

1. Game monitors player performance metrics
2. Algorithm evaluates if player is above/below target difficulty
3. Adjustments happen (invisible to player ideally)
4. Player stays in flow state — challenged but not frustrated
5. Continuous adjustment throughout the experience

## Adjustment levers

### Combat difficulty
- **Enemy damage dealt**: Reduce/increase based on performance
- **Enemy health**: Scale HP up/down
- **Enemy accuracy**: Adjust AI aim precision
- **Enemy数量**: More/fewer enemies spawning
- **Enemy spawn rate**: Faster/slower waves

### Resource economy
- **Health drop rate**: More heals when struggling
- **Ammo availability**: More ammo for struggling players
- **Loot quality**: Better drops when doing well (or struggling?)
- **Checkpoint frequency**: More checkpoints when dying often

### Pacing
- **Wave intensity** (Left 4 Dead): Director controls horde timing
- **Encounter density**: More/fewer combat encounters
- **Exploration time**: More downtime between fights when stressed
- **Boss timing**: Delay or rush boss encounters

### Information
- **Aim assist**: Stronger when struggling
- **Hint frequency**: More hints for stuck players
- **UI information**: Show more/less data based on skill
- **Slow-motion**: Brief slowdowns for struggling players

## Detection metrics

### Direct metrics
- **Death count**: Most obvious signal
- **Damage taken**: How much punishment player absorbs
- **Healing item usage**: Frequent healing = struggling
- **Time per encounter**: Fast clear = skilled, slow = struggling

### Indirect metrics
- **Movement patterns**: Confident vs. hesitant movement
- **Ability usage**: Skilled players use abilities more
- **Optional content**: Doing side content = comfortable
- **Retry rate**: How often players restart sections

### Composite scoring
- **Multi-factor**: Combine multiple metrics for accuracy
- **Weighted recent**: Recent performance matters more
- **Time-decay**: Old data matters less over time

## Design dimensions

### Transparency
- **Invisible** (Resident Evil 4): Player never knows adjustments happen
- **Subtle** (Left 4 Dead): AI Director is mentioned but not explained
- **Transparent** (Forza): "Drivatar" system is visible and marketed
- **Opt-in** (Devil May Cry): Player chooses difficulty, no auto-adjust

### Adjustment speed
- **Gradual**: Slow adjustments over many encounters
- **Immediate**: Adjusts between encounters or deaths
- **Phase-based**: Only adjusts between major sections
- **Session-based**: Adjusts between play sessions

### Scope of adjustment
- **Combat only**: Only enemy stats change
- **Full experience**: Resources, pacing, difficulty all adjust
- **Narrative**: Even story beats change (rare, ambitious)

## Anti-patterns

- **Noticeable adjustment**: If players see enemies getting weaker, immersion breaks
- **Rubber-banding**: Oscillating between easy and hard feels random
- **Punishing success**: Making the game harder just because you're good feels unfair
- **Removing player agency**: Auto-aim and auto-play defeat the purpose

## References

- Resident Evil 4: The pioneer of invisible DAA
- Left 4 Dead 2: AI Director is the gold standard for dynamic pacing
- Forza Horizon 5: Drivatar system makes AI feel human
- Devil May Cry 5: Style rating system naturally adjusts perceived difficulty

## Tutorials

- [Dynamic Difficulty Adjustment Explained](https://www.youtube.com/watch?v=zx7vG4Pvdxs) — How DDA works and why it matters for player retention
- [Left 4 Dead AI Director Deep Dive](https://www.youtube.com/watch?v=E1ozhIJM7TI) — How Valve's AI Director creates dynamic horror experiences

## Image Sources

- DDA flowchart diagrams — Self-created system design diagrams
- Difficulty curve visualizations — Self-created graphs
