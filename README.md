# BOP + Biological Wonders Spawn Control (Forge 1.20.1)

This datapack uses Forge biome modifiers to fully control Biological Wonders spawning so creatures only appear in the biome IDs configured by this pack.

## Design goals

- Prevent default BW spawns from interfering with curated spawn design.
- Keep compatibility-friendly behavior for parallel datapacks by scoping to explicit biome/entity rules.
- Configure spawns per biome file (not per animal) for easier maintenance.
- Keep spawn rates vanilla-like: visible in expected biomes without overpopulation.

## How it works

1. `00_remove_bw_from_overworld.json` removes the configured BW animals from all overworld biomes.
2. Each `10_biome_*.json` file re-adds only the intended creatures for a single biome ID.

## Notes

- Uses `biomesoplenty:*` and `minecraft:*` biome IDs.
- If you add an animal to a new biome, update that biome's file only.
