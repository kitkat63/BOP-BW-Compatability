# BOP + ZAWA Spawn Control (Forge 1.20.1)

This datapack uses Forge biome modifiers to curate ZAWA spawns in Biomes O' Plenty overworld biomes.

## Design goals

- Per-biome placement for BOP overworld biomes.
- Bugs allowed in mystical biomes, but other fauna blocked there.
- Savannah specialists only in explicit savannah biomes.
- Monkeys/apes primarily in rainforest and tropics biomes.
- Snow leopard is very rare and restricted to tundra/mountain-like BOP biomes.
- Wildlife rarity roughly mirrors real-world rarity (lower weights for rare species).

## How it works

1. `00_remove_zawa_from_bop_overworld.json` clears all known ZAWA entity spawns from BOP overworld biome IDs.
2. Additional `forge:add_spawns` biome modifiers then add controlled spawn sets by biome group.

## Notes

- Lemurs are restricted to rainforest variants only; giant pandas are focused on bamboo jungle and redwood forest.
- Aquatic profiles are tuned for fish-heavy waters with orcas intentionally rarer than fish (including frozen ocean support).
- Koalas are explicitly removed from stony shore and gharials from frozen river.
- "Mystical Biomes" have a higher bug populace than the rest of the biomes.
- Asian Elephants are limited to 1 biome only.
- Macaws only spawn in rainforests.
- Biomes not included in add-spawn modifiers intentionally receive no ZAWA spawns (example: end biomes and nether biomes).
- Adds brown rats in village-associated biomes (closest datapack-only approximation for structure spawns).
- If another datapack/modifier adds spawns later in pack order, it can override these results.
- Use `/reload` after installing and prefer this datapack near the end of load order.
