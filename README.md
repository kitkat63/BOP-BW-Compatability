# BOP + Biological Wonders Spawn Control (Forge 1.20.1)

This datapack uses Forge biome modifiers to curate ZAWA spawns in Biomes O' Plenty overworld biomes.

## Design goals

- Per-biome placement for BOP overworld biomes.
- Bugs allowed in mystical biomes, but other fauna blocked there.
- Wildlife rarity roughly mirrors real-world rarity (lower weights for rare species).

## How it works

1. `00_remove_bw_from_bop_overworld.json` clears all known Biological Wonders entity spawns from BOP overworld biome IDs.
2. Additional `forge:add_spawns` biome modifiers then add controlled spawn sets by biome group.

## Notes

- Aquatic Animals Should Spawn In Appropriate Biomes
- No Competition Between Gharial and Cuban Crocodile
