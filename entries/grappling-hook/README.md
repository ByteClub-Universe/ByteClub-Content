# Grappling Hook

The grappling hook is a traversal mechanic that allows players to attach to surfaces and propel themselves through the environment.

## How it works

The player fires a hook that attaches to a surface. Once attached, the player can:
- Swing from the attachment point
- Pull themselves toward the attachment point
- Reel in or extend the rope

## Design considerations

- **Momentum preservation**: The hook should maintain the player's momentum for fluid movement
- **Attachment rules**: What surfaces can be hooked? (walls, ceilings, specific materials)
- **Range limits**: Maximum hook distance to prevent abuse
- **Cooldown**: Prevents spamming

## Variations

- **Swinging**: Classic grappling hook that lets player swing
- **Pull-to-target**: Instantly pulls player to attachment point
- **Reel-in**: Gradually pulls player toward the point

## Tutorials

- [ADVANCED GRAPPLING HOOK in 11 MINUTES - Unity Tutorial](https://www.youtube.com/watch?v=TYzZsBl3OI0) — Step-by-step implementation of a precise grappling gun with raycasting, line renderer visualization, and physics-based pull force
- [Physically Accurate Grappling Hook/Gun in Unity](https://www.youtube.com/watch?v=q9F_ricTfw4) — 5-level tutorial covering physically accurate grapple mechanics

## Image Sources

- Grappling Hook SVG asset — [OpenGameArt.org](https://opengameart.org/content/grappling-hook) (CC0 Public Domain, by azureguy)