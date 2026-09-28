# Travel & Worlds

TownifyMC's main world is a large **Earth map**, so knowing how to get around matters. This page covers warps, random teleport, the Resource World, road speed, and elevators.

## The warp menu

```
/warp           # open the travel menu
/warp <name>    # go straight to a warp
```

The `/warp` menu is the quickest way to anywhere:

| Destination | What's there |
|-------------|--------------|
| :material-earth: **Overworld** | Random teleport into the main Earth world |
| :material-fire: **The Nether** | Random teleport into the Nether |
| :material-orbit: **The End** | Random teleport into the End |
| :material-sword-cross: **PvP Arena** | Fight other players for glory |
| :material-skull: **Dungeons** | The dungeon hub (see [Dungeons & Combat](dungeons.md)) |
| :material-grave-stone: **Your Gravestone** | Teleport to your latest grave |
| :material-home: **Spawn** | Back to spawn |

Named warps you can type directly include `market`, `crates`, `vote`, `dungeons`, `tower`, `zoo`, `pvp`, `fishing`, `bounties`, and `pinataparty`. Press ++tab++ after `/warp ` to see them all.

## Random teleport (RTP)

```
/rtp            # random spot in the world (also /wild)
/rtp <continent>    # random spot on a specific continent
```

Because the world is Earth, you can choose **which continent** to land on:

| Type | Lands you in |
|------|--------------|
| `/rtp northamerica` (or `na`) | North America |
| `/rtp southamerica` (or `sa`) | South America |
| `/rtp europe` (or `eu`) | Europe |
| `/rtp africa` (or `af`) | Africa |
| `/rtp asia` (or `as`) | Asia |
| `/rtp australia` (or `au`) | Australia / Oceania |
| `/rtp antarctica` (or `ant`) | Antarctica |

Continent RTP has a **30-second cooldown** and always looks for dry, safe ground (no water, lava, leaves, or ice).

!!! tip "Scouting for a town site"
    Pair continent RTP with the [live map](https://map.townifymc.xyz) (`/map`) to find open land in the part of the world you want to settle before you commit to claiming.

## The Resource World

Don't strip-mine the main map. Gather in the **Resource World** instead:

```
/rw     # go to the Resource World
/nrw    # random teleport into the Resource Nether
```

| | |
|---|---|
| **Resets** | About every **30 days**. Everything in it is wiped |
| **Size** | 10,000-block world border |
| **Hostile mobs** | Off (animals still spawn) |
| **PvP** | Off |

!!! warning "Don't build or store anything there"
    The Resource World is **deleted and regenerated** on reset. You get a 60-second chat countdown before it happens, and anyone inside is moved to the hub. Anything you left there is gone. Build your base in the main world, inside a [town](../towns/towns.md).

The [server rules](../getting-started/rules.md) ask you to do heavy gathering in resource areas like this one rather than scarring the main map.

## Roads: travel faster

Walking on **player-built roads** makes you faster. The better the road, the bigger the boost:

| Tier | Speed | Blocks that count |
|------|:-----:|-------------------|
| :material-walk: **Trail** | +25% | Dirt Path, Gravel, Mud, Packed Mud |
| :material-road: **Road** | +50% | Cobblestone, Stone, Smooth Stone, Andesite, Diorite, Granite (and polished), Cobbled/Polished Deepslate, Mud Bricks |
| :material-highway: **Highway** | +75% | Stone Bricks (any), Deepslate Bricks, Polished Blackstone Bricks, **any Concrete or Concrete Powder** |

- Road and Highway blocks only count if a **player placed them**. Natural stone in the wild doesn't give a boost.
- **Dirt paths** always count as Trails, including the paths that wear into the grass naturally where players walk a lot.
- Your action bar shows "Entering Trail / Roadway / Highway" as you switch tiers.

```
/roads          # show the full road building guide
/roadtier       # what are you standing on right now?
/roadspeed      # turn road boosts off/on
```

!!! tip "Build highways between towns"
    Towns and nations that connect to each other with concrete or stone-brick highways make travel much faster for everyone. It's a good nation project.

## Elevators

**Elevator Blocks** let you move between floors instantly. Stack them in the same column (same X/Z) and:

- **Jump** on one to go **up** to the next elevator above.
- **Sneak** on one to go **down** to the next elevator below.

Placed elevators show a floating "Jump ↑ • Sneak ↓" label. Anyone can **use** an elevator once it's placed.

**Crafting an Elevator Block** (lodestone-looking block) needs the elevator crafting perk:

```
      Redstone
Redstone  Smooth Stone  Redstone
      Redstone
```

## Flight

Flight unlocks through ranks (see [The Rank Ladder](../progression/ranks.md)) or by buying **Town Flight** from the [Gem Store](../perks/store.md). Check whether you can fly where you're standing:

```
/canfly         # or /cf
```

## Happy Ghasts

Tamed **Happy Ghasts** drift slowly on their own, but they **speed up a lot when you ride one**, so they make a real travel mount.

---

**Related:** [Dungeons & Combat](dungeons.md) · [Useful Commands & Shortcuts](../reference/shortcuts.md)
