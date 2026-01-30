# Minecraft Revival+ 1.16.5 Implementation TODO

## 1. Critical Bug Fixes (High Priority)

### World Generation Bugs
- [x] Fix chunk border seams where biomes abruptly cut off (Biome blending in ChunkGenerator.java or BiomeProvider.java)
- [x] Resolve floating Nether terrain fragments (NetherChunkGenerator.java or Nether biome generation)
- [x] Correct broken Bastion Remnant structure generation overlapping lava oceans (BastionRemnantStructure.java)
- [x] Fix stronghold generation occasionally failing to spawn End Portal frames (StrongholdStructure.java)
- [x] Prevent structures spawning inside bedrock layers (Structure placement logic)
- [x] Address village path blocks generating incorrectly on slopes (Village generation)

### Entity & Mob Bugs
- [x] Fix mobs despawning incorrectly in loaded chunks (Mob despawn logic)
- [x] Resolve zombie villagers not converting properly when cured (ZombieVillagerEntity.java)
- [x] Fix piglins randomly attacking players wearing gold armor (PiglinEntity.java)
- [ ] Correct wither skull hitbox inconsistencies (WitherSkullEntity.java)
- [ ] Fix endermen teleporting into unloaded chunks (EndermanEntity.java)
- [ ] Address ghasts firing fireballs through solid blocks (GhastEntity.java)

### Redstone Bugs
- [ ] Fix quasi-connectivity inconsistencies (Redstone wire logic)
- [ ] Correct observer block double-trigger behavior (ObserverBlock.java)
- [ ] Fix pistons duplicating blocks in edge cases (PistonBlock.java)
- [ ] Address hopper item loss during chunk reloads (HopperBlock.java)
- [ ] Resolve redstone dust visual desync with signal strength (RedstoneWireBlock.java)

### Combat Bugs
- [ ] Fix hit registration desync in multiplayer (Combat mechanics)
- [ ] Resolve shield blocking angles being inconsistent (ShieldItem.java)
- [ ] Fix sweeping edge not damaging mobs in some scenarios (SwordItem.java)
- [ ] Correct critical hit calculation issues (Combat calculations)
- [ ] Address knockback inconsistencies (Entity knockback)

## 2. Performance Improvements

### Client Optimization
- [ ] Reduce memory usage when loading large worlds (World loading)
- [ ] Improve chunk rendering speed (ChunkRenderer.java)
- [ ] Optimize lighting engine updates (Lighting engine)
- [ ] Reduce lag spikes when loading new chunks (Chunk loading)
- [ ] Improve particle rendering efficiency (ParticleManager.java)

### Server Optimization
- [ ] Improve mob AI tick scheduling (Mob AI)
- [ ] Reduce server-side lag from hopper chains (HopperBlock.java)
- [ ] Optimize entity collision calculations (Entity collision)
- [ ] Improve chunk save performance (Chunk saving)
- [ ] Reduce network packet spam from redstone devices (Redstone networking)

### Low-End System Support
- [ ] Improve FPS stability on integrated GPUs (Rendering optimizations)
- [ ] Add better chunk unload management (Chunk unloading)
- [ ] Reduce VRAM usage for textures (Texture management)
- [ ] Optimize world generation for low-end systems

## 3. Nether Update Polish (1.16 Focus)

### Biome Improvements
- [ ] Increase biome transition smoothness (Biome blending)
- [ ] Add small decorative blocks (fallen blackstone debris, warped roots clusters)
- [ ] Improve fog color blending between Nether biomes
- [ ] Add ash particle storms in Basalt Deltas

### Structure Improvements
- [ ] Improve Bastion loot balance (Bastion loot tables)
- [ ] Fix fortress generation frequency (NetherFortressStructure.java)
- [ ] Add visual variation to Nether bridges
- [ ] Improve ruined portal placement logic (RuinedPortalStructure.java)

### Mob Behavior Enhancements
- [ ] Improve piglin bartering randomness (PiglinEntity.java)
- [ ] Add smarter hoglin pathfinding (HoglinEntity.java)
- [ ] Improve strider lava navigation (StriderEntity.java)
- [ ] Reduce zombified piglin overcrowding (ZombifiedPiglinEntity.java)

## 4. Quality of Life Improvements

### Inventory & UI
- [ ] Add optional item sorting button (InventoryScreen.java)
- [ ] Improve recipe book filtering (RecipeBook.java)
- [ ] Add durability percentage display (optional toggle) (Item durability display)
- [ ] Improve tooltip readability (Tooltip rendering)
- [ ] Add search bar improvements (Search functionality)

### Gameplay Flow
- [ ] Improve respawn anchor feedback (RespawnAnchorBlock.java)
- [ ] Improve beacon interface clarity (BeaconScreen.java)
- [ ] Improve brewing stand UI speed (BrewingStandScreen.java)
- [ ] Add clearer enchantment hints (without removing randomness) (Enchantment hints)

### Accessibility
- [ ] Add colorblind mode presets (Color settings)
- [ ] Improve subtitle accuracy (Subtitle system)
- [ ] Improve UI scaling options (UI scaling)
- [ ] Add better controller support mapping (Controller input)

### Multiplayer
- [x] Add username selection in multiplayer screen (MultiplayerScreen.java)

## 5. Balance Changes

### Combat Balance
- [ ] Slightly rebalance sword vs axe damage (Weapon damage)
- [ ] Improve bow draw consistency (BowItem.java)
- [ ] Balance crossbow reload time (CrossbowItem.java)
- [ ] Reduce knockback randomness (Knockback calculations)

### Survival Balance
- [ ] Adjust Netherite durability scaling (Netherite items)
- [ ] Balance piglin bartering drops (Piglin bartering)
- [ ] Adjust blaze rod drop rates slightly (BlazeEntity.java)
- [ ] Balance ancient debris spawn rates (Ancient debris generation)

### Economy Balance
- [ ] Improve villager trade fairness (Villager trading)
- [ ] Prevent emerald inflation from exploit farms (Trading mechanics)
- [ ] Improve wandering trader usefulness (WanderingTraderEntity.java)

## 6. New Features (Minor Additions, No Major Overhaul)

### Blocks
- [x] Polished Blackstone Variants
- [x] Cracked Nether Bricks
- [x] Warped Lantern
- [x] Crimson Lantern
- [ ] Decorative Chains (color variants)

### Items
- [x] Nether Backpack (Nether-only fire resistant storage)
- [x] Piglin Compass (points to nearest Bastion)
- [x] Soul Torch Variants

### Ambient Additions
- [x] Ash particle storms in Basalt Deltas
- [ ] Nether ambient sounds improvements
- [ ] Biome-specific echo effects

## 15. Revival+ Custom Features (New Additions)

### UI Enhancements
- [x] Add "Revival Settings" button to main menu
- [x] Revival settings screen with toggles for new features

### AI Improvements
- [x] Enhanced mob pathfinding to avoid lava
- [x] Improved villager job site detection

## 7. AI & Pathfinding Improvements
- [ ] Improve mob navigation around lava (Pathfinding)
- [ ] Fix mobs getting stuck on slabs (Mob movement)
- [ ] Improve flying mob path prediction (Flying entity pathfinding)
- [ ] Improve villager job site detection (Villager AI)
- [ ] Reduce mob jitter movement (Mob animation)

## 8. Multiplayer Improvements
- [ ] Improve server stability under high player count (Server optimizations)
- [ ] Reduce rubber-banding (Network synchronization)
- [ ] Improve chunk synchronization (Chunk networking)
- [ ] Add better anti-lag entity caps (Entity management)
- [ ] Improve spectator mode camera smoothness (Spectator mode)

## 9. Modding & Developer Support
- [ ] Improve datapack error handling (Datapack loading)
- [ ] Add better crash logging (Crash reporting)
- [ ] Improve debug screen clarity (Debug screen)
- [ ] Improve custom dimension API stability (Dimension API)
- [ ] Improve world export compatibility (World export)

## 10. Visual Polish
- [ ] Improve water shader reflections (Water rendering)
- [ ] Improve Nether lava lighting (Lava lighting)
- [ ] Improve shadow transitions (Shadow rendering)
- [ ] Fix texture mipmap flickering (Texture rendering)
- [ ] Improve animation smoothness for mobs (Mob animations)

## 11. Audio Improvements
- [ ] Improve ambient Nether sound layering (Nether sounds)
- [ ] Fix sound delay bugs (Sound system)
- [ ] Improve spatial audio positioning (3D audio)
- [ ] Balance explosion sound levels (Explosion sounds)
- [ ] Improve step sound variation (Footstep sounds)

## 12. Security & Exploit Fixes
- [ ] Patch duplication glitches (Item duplication)
- [ ] Fix chunk corruption exploits (Chunk validation)
- [ ] Improve anti-cheat detection hooks (Anti-cheat)
- [ ] Fix creative mode NBT injection exploits (Creative mode)
- [ ] Patch infinite XP farm exploits (XP farming)

## 13. Testing Requirements
- [ ] Automated Testing: Chunk generation tests, Mob behavior simulations, Redstone reliability tests, Server stress tests
- [ ] Manual Testing: Hardcore survival playthrough, Multiplayer stress servers, Speedrun compatibility tests, Redstone contraption testing

## 14. Long-Term Preparation
- [ ] Prepare the engine for: Future cave generation overhaul, Vertical world expansion, Improved lighting system rewrite, Better animation framework, More biome blending technology
