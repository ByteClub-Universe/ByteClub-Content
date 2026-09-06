# Inventory Management

## Overview

Inventory management is the tension of limited space. You can't carry everything, so every pickup becomes a decision. Do you drop the handgun ammo for the shotgun shells? Keep the herbs or the grenades? It turns looting into strategy and makes every item feel valuable.

## Core loop

1. Player encounters items in the world
2. Player evaluates item value vs. current inventory state
3. Player decides: pick up (replace something?) or leave
4. Inventory state affects gameplay decisions
5. Management becomes a puzzle of optimization

## Inventory types

### Slot-based (Resident Evil 4)
- **Fixed grid**: Items take specific grid spaces
- **Tetris-style**: Rotate and arrange to fit more
- **Weight/size**: Different items take different amounts of space
- **Organized**: Visual layout makes management intuitive

### Weight-based (Fallout, Tarkov)
- **Encumbrance system**: Total weight limit
- **Movement penalty**: Over-encumbered = slow
- **Realistic**: More immersive but less tactile
- **Math-heavy**: Players optimize by numbers

### Stack-based (Minecraft, Terraria)
- **Stacking**: Same items stack to limit
- **No spatial puzzle**: Just count management
- **Simple**: Less overhead, more focus on gameplay
- **Organized**: Easier to manage, less tension

### Unlimited (some RPGs)
- **No limit**: Carry everything
- **No management**: Less tension, less decisions
- **Quality of life**: Less tedium, more action
- **Depends on game**: Works for some, not for others

## Design dimensions

### Capacity
- **Tiny** (Resident Evil): 12-20 slots, every item matters
- **Moderate** (Minecraft): 36 slots + hotbar, comfortable
- **Large** (Terraria): 50+ slots, almost everything fits
- **Unlimited** (some games): No limit at all

### Item categorization
- **Equipment vs. consumables**: Different sections
- **Quick access**: Hotbar or favorites system
- **Storage**: Base storage for excess items
- **Sorting**: Auto-sort by type, rarity, etc.

### Management friction
- **High friction** (Tarkov): Every slot matters, constant decisions
- **Medium** (Resident Evil): Need to manage but not overwhelming
- **Low friction** (Minecraft): Easy to organize, minimal stress
- **No friction** (unlimited inventories): No management needed

### Tension generation
- **Scarcity pressure**: Can't carry everything = hard choices
- **Risk of loss**: Drop items on death (Tarkov, Rust)
- **Time pressure**: Can't manage inventory during combat
- **Opportunity cost**: Choosing one item means not having another

## Anti-patterns

- **Too small**: If inventory is frustratingly small, players get annoyed not challenged
- **Too large**: If everything fits, there's no management puzzle
- **Unclear item value**: Players don't know what's important
- **Tedious sorting**: If organizing is the hard part, not deciding, it's bad design
- **No storage**: If you can't store excess items, you're just dropping things

## References

- Resident Evil 4: The attaché case is inventory management perfection
- Escape from Tarkov: Hardcore inventory that IS the game
- Path of Exile: Massive stash tabs as endgame management
- Stardew Valley: Simple but satisfying inventory with shipping bin

## Tutorials

- [Inventory Management Design](https://www.youtube.com/watch?v=NlqZ4LT1Jxk) — How to design inventory systems that create meaningful decisions
- [Resident Evil 4 Inventory Analysis](https://www.youtube.com/watch?v=KfWFRaUn8Jo) — Why RE4's attaché case is iconic game design

## Image Sources

- Inventory UI mockups — Self-created design concepts
- Slot arrangement diagrams — Self-created spatial analysis
