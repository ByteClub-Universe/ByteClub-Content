# Procedural Generation

## Overview

Procedural generation is the art of making randomness feel intentional. Instead of hand-crafting every room, you build systems that compose levels from parts. Done right, players can't tell the difference. Done wrong, they're playing the same bland corridors forever.

## Core loop

1. Algorithm selects templates/chunks based on rules
2. Pieces are assembled with constraints (connectivity, difficulty)
3. Metadata stamps ensure variety (enemy counts, item placement)
4. Player experiences a "new" level that follows design principles
5. Each run feels fresh but fair

## Generation techniques

### Tile-based
- **Cellular automata**: Cave generation, organic shapes
- **Wave function collapse**: Constraint-based, very flexible
- **BSP trees**: Binary space partitioning for room layouts
- **Drunkard's walk**: Random walk for cave connectivity

### Template-based
- **Room templates** (Spelunky): Pre-designed rooms stitched together
- **Chunk systems** (Minecraft): Pre-built chunks assembled
- **Handmade + random**: Core paths handcrafted, details randomized

### Rule-based
- **Difficulty curves**: Algorithm adjusts enemy density per area
- **Biome rules**: Different tilesets/enemies per zone
- **Loot tables**: Random drops weighted by area difficulty

### Seed-based
- **Deterministic**: Same seed = same level (speedrun competitive)
- **Shareable**: Players can share seeds for the same experience
- **Debuggable**: Can reproduce specific generated levels

## Design dimensions

### Randomness vs. handcrafting
- **Pure random** (early roguelikes): Completely algorithmic, can be unfair
- **Guided random** (Spelunky): Templates + rules = fair and varied
- **Mostly handcrafted** (Dead Cells): Handmade rooms, random order
- **Hybrid** (Hades): Fixed rooms, random encounter selection

### Replayability impact
- **High** (Spelunky): Every run genuinely different
- **Medium** (Dead Cells): Same rooms but different combos
- **Low** (some games): Generation adds variety but not depth

### Fairness guarantees
- **Landing zones**: Safe starting area guaranteed
- **Resource minimums**: Enough health/ammo to survive
- **Difficulty scaling**: Later areas harder but still beatable
- **No dead ends**: Always a way forward

## Anti-patterns

- **Obvious repetition**: If players notice the same patterns, the illusion breaks
- **Unfair layouts**: Random doesn't mean impossible — always ensure solvability
- **Bland generation**: Random rooms with no identity = boring
- **Performance cost**: Heavy generation can cause loading hitches

## References

- Spelunky: The godfather of modern roguelike generation
- Rogue Legacy 2: Castle generation with biome-based rules
- Dead Cells: Template-based with handcrafted quality
- Minecraft: Infinite world generation at massive scale

## Tutorials

- [Spelunky's Procedural Generation Explained](https://www.youtube.com/watch?v=GpTk5vwaNtU) — How Derek Yu built Spelunky's generation system
- [Procedural Level Generation Techniques](https://www.youtube.com/watch?v=ZZY9YE7rZJw) — Overview of different procedural algorithms and when to use them

## Image Sources

- Level layout diagrams — Self-created procedural generation examples
- Algorithm visualizations — Inspired by [Redblobgames](https://www.redblobgames.com/) (referenced)
