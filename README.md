# PM5 Block State Converter

> **Bedrock Edition Block States → PocketMine-MP 5 PHP Code**

Free online tool to convert Minecraft Bedrock Edition block states into ready-to-use PocketMine-MP 5 (PM5) PHP code.

🔗 **[Open Converter →](https://w1zardz.github.io/pm5-block-state-converter/)**

## What is this?

With the transition to PocketMine-MP 5, the old numeric block IDs and metadata were completely removed. Blocks now use **string identifiers** and **typed state properties** (BlockTraits).

This makes creating custom blocks more complex — you need to know the exact property names, valid values, and how Bedrock states map to PM5 setter methods.

**This tool solves that problem.** Select a block, configure its states visually, and copy the generated PHP code.

## How it works

1. **Search** for a block by name or Bedrock ID (e.g., `minecraft:oak_stairs`)
2. **Select** the block from the grid
3. **Configure** state properties (facing direction, upside down, open/closed, etc.)
4. **Copy** the generated `VanillaBlocks` PHP factory code

## Example output

```php
use pocketmine\block\VanillaBlocks;
use pocketmine\math\Facing;

$block = VanillaBlocks::OAK_STAIRS()
    ->setFacing(Facing::NORTH)
    ->setUpsideDown(true);

// Bedrock: minecraft:oak_stairs
```

## Supported blocks

- **Stairs** — all wood and stone variants (40+)
- **Slabs** — single, top, double (50+)
- **Doors & Trapdoors** — all wood + iron
- **Fence Gates** — all wood types
- **Buttons & Pressure Plates** — wood + stone
- **Logs & Wood** — all types + stripped variants
- **Walls** — all stone variants (25+)
- **Colored Blocks** — wool, concrete, terracotta, glass, carpet, shulker boxes (140+)
- **Redstone** — repeater, comparator, lever, rail, wire, daylight sensor, hopper
- **Torches & Lanterns** — regular, soul, redstone
- **Candles** — all 17 color variants
- **Crops** — wheat, carrots, potatoes, beetroot, nether wart, cocoa
- **Signs** — floor and wall, all wood types
- **Furnaces** — regular, blast, smoker
- **And more** — beds, chests, campfires, bells, barrels, ladders, vines, liquids...

**200+ blocks** with configurable state properties.

## Features

- Mobile-optimized responsive design
- Instant search and category filtering
- Syntax-highlighted PHP code output
- One-click copy to clipboard
- No dependencies, pure HTML/CSS/JS
- Works offline (GitHub Pages)

## Tech

Single-page static app. No build tools, no frameworks, no dependencies.

- HTML5 + CSS3 + Vanilla JS
- Hosted on GitHub Pages
- SEO optimized for Google and Yandex

## Contributing

Found a missing block or incorrect mapping? [Open an issue](https://github.com/w1zardz/pm5-block-state-converter/issues) or submit a PR.

## Links

- [PocketMine-MP](https://github.com/pmmp/PocketMine-MP) — the server software
- [PM5 Documentation](https://doc.pmmp.io/) — official docs
- [PMMP Discord](https://discord.gg/bmSAZBG) — community

## License

MIT
