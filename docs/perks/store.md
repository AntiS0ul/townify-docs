# Gem Store & Upgrades

There are two in-game menus for buying permanent upgrades: **`/upgrades`**, which takes money (and some Gems), and the **Gem Store** (`/servershop`), which takes Gems.

## Upgrades (`/upgrades`)

```
/upgrades       # open the upgrades menu
```

Upgrades must be bought **in order**: you need tier 2 before you can buy tier 3.

### Homes

| Homes | Price |
|:-----:|-------|
| 1 | Free |
| 3 | <span class="chip money">$25,000</span> |
| 5 | <span class="chip money">$50,000</span> |
| 7 | <span class="chip money">$75,000</span> |
| 10 | <span class="chip money">$100,000</span> |
| 20 | <span class="chip gems">10,000 Gems</span> |
| 25 | <span class="chip gems">25,000 Gems</span> |

### Player-warp slots

Another way to get [player warps](storage.md#player-warps) besides ranking up:

| Slots | Price |
|:-----:|-------|
| 1 | <span class="chip money">$50,000</span> |
| 2 | <span class="chip money">$75,000</span> |
| 3 | <span class="chip money">$100,000</span> |
| 4 | <span class="chip money">$200,000</span> |
| 5 | <span class="chip money">$500,000</span> |
| 7 | <span class="chip gems">10,000 Gems</span> |
| 10 | <span class="chip gems">25,000 Gems</span> |

## The Gem Store (`/servershop`)

```
/servershop     # or /serverstore
/store          # link to buy Gems online
```

Everything here is paid in <span class="chip gems">Gems</span>. Check your balance with `/bal`.

| Section | What you can buy |
|---------|------------------|
| :material-key: **Keys** | Crate keys for the [crates](../rewards/crates.md) |
| :material-cube-outline: **Chunk Loader / Hopper** | A **Chunk Loader** that keeps a chunk loaded for a month, and a **Chunk Hopper** that collects items from a whole chunk |
| :material-rocket-launch: **Job Boosts** | **Money** and **XP Boost Tokens** (see below) |
| :material-airplane: **Permissions** | **Town Flight**: fly inside town claims (<span class="chip gems">25,000 Gems</span>) |
| :material-ticket: **Premium Battle Pass** | Unlock the [premium track](../progression/quests.md#battle-pass) (<span class="chip gems">15,000 Gems</span>). Don't buy it twice in one season |
| :material-crown: **Lifetime ranks** | Donor ranks with cosmetic and QoL perks (below) |

### Job Boost Tokens

Right-click a **Money Boost Token** or **XP Boost Token** to start a **25% job boost for the whole server** for **60 minutes**.

- If a boost of that type is already running, your token **adds 60 minutes** to it. The boost stays at 25%; only the time stacks.
- Boosts survive server restarts.
- Everyone online benefits, so boosts make good times for group grinding.

### Lifetime donor ranks

These are **permanent** and separate from the [money rank ladder](../progression/ranks.md). You keep your ladder rank and add the donor perks on top.

| Rank | Perks |
|------|-------|
| **Goblin** | Hex-color nickname · Cursed & Slime suits · Donator chat · 5 player vaults |
| **Pixie** | Panda & Axolotl pets · 6 player vaults · `/feed` every 4h · Kit 1 |
| **Cyclops** | Horse & Nyan Sheep mounts · Head database · **Bulk crafting** · 7 player vaults |
| **Banshee** | Keep XP · `/glow` · Divine Halo & Magical Rods particles · 8 player vaults · `/feed` every 2h · Kit 2 |
| **Siren** | Find biome · Item hats · Llama & Axolotl morphs · 9 player vaults · `/feed` every 90m |
| **Sphinx** | **Keep inventory** · Marry other players · Explosion death effect & Love arrows · 10 player vaults · `/feed` every 1h · Kit 3 |
| **Phoenix** | `/fly` · Priority queue · All emojis · `/feed` every 30m · Kit 4 |

Open `/servershop` for current Gem prices and `/donator` to use the perks you own.

!!! info "Where Gems come from"
    You can buy Gems on the [online store](https://townify.tebex.io/category/gems) (`/store`), and you can earn them in game from [chat games](../rewards/events.md#chat-games), [fishing competitions](../money/fishing.md), crates, and events.

## Bulk crafting

With **bulk crafting** (a Cyclops perk), one command crafts everything in your inventory into blocks.

```
/bulkcraft      # list the bulk-craft commands you have
```

| Tier | Example commands |
|------|------------------|
| **Basic** | `/sandstone` `/haybale` `/boneblock` `/slimeblock` `/honeyblock` `/prismarine` `/clayblock` `/mossblock` … |
| **Builder** | `/concrete` `/stonebricks` `/deepslatebricks` `/bricks` `/quartzblock` `/purpur` `/lantern` `/sealantern` … |
| **Master** | `/ironblock` `/goldblock` `/diamondblock` `/emeraldblock` `/netheriteblock` … and **`/compact`**, which packs every ingot, gem, and coal/charcoal at once |

---

**Related:** [Storage & Backpacks](storage.md) · [Economy & Currencies](../progression/economy.md)
