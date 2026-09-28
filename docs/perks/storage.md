# Storage & Backpacks

Inventory space is always at a premium in Minecraft. TownifyMC gives you several ways to expand it — most of which **scale with your [rank](../progression/ranks.md)**.

## Player Vaults (`/pv`)

Player Vaults are **personal stored inventories** you can access from anywhere — like having extra enderchests. You unlock more vaults as you rank up.

```
/pv 1           # open vault #1
/pv <number>    # open a specific vault
```

### Vaults by rank

| Vaults | Unlocked at | Rank |
|:------:|-------------|------|
| `/pv 1` | <span class="chip money">$1,000,000</span> | <span class="tier-rare">Landlord</span> (#11) |
| `/pv 1–2` | <span class="chip money">$3,500,000</span> | <span class="tier-rare">Elder</span> (#13) |
| `/pv 1–3` | <span class="chip money">$15,000,000</span> | <span class="tier-epic">Knight</span> (#17) |
| `/pv 1–4` | <span class="chip money">$33,000,000</span> | <span class="tier-epic">Count</span> (#20) |
| `/pv 1–5` | <span class="chip money">$67,000,000</span> | <span class="tier-legendary">Duke</span> (#23) |
| `/pv 1–6` | <span class="chip money">$160,000,000</span> | <span class="tier-celestial">Celestial</span> (#27) |

So your storage grows right alongside your wealth — by the endgame you've got **six full vaults** of overflow space. Lifetime donor ranks from the [Gem Store](store.md#lifetime-donor-ranks) raise this to as many as **10 vaults**.

## Backpacks

Backpacks are **portable storage** you carry with you — open them anywhere without running to a chest. They come in **three tiers**, each bigger than the last.

| Backpack | Unlocked at | Rank |
|----------|-------------|------|
| **Tier 1** | <span class="chip money">$2,000,000</span> | <span class="tier-rare">Patriarch</span> (#12) |
| **Tier 2** | <span class="chip money">$33,000,000</span> | <span class="tier-epic">Count</span> (#20) |
| **Tier 3** | <span class="chip money">$67,000,000</span> | <span class="tier-legendary">Duke</span> (#23) |

Backpacks are **physical items**: hold one and **right-click** to open it.

!!! tip "Backpacks vs. Vaults"
    - **Backpacks** travel *with you* — perfect for mining trips and long expeditions where you fill up fast.
    - **Vaults** are *stored* and accessed on demand — better for long-term overflow you don't carry around.

    Use both: dump expedition loot into your backpack in the field, then offload into vaults back home.

## Void Storage

A **Void Storage** item holds **thousands of one item type** in a single inventory slot. It's handy for builders hauling huge amounts of one block.

**Create one:** open your inventory, pick up a **Void Crystal** on your cursor, hover over a block or stackable item, and **right-click**. The crystal and the item combine into a Void Storage for that item.

Capacity is rolled when you create it:

| Rarity | Chance | Holds |
|--------|:------:|------:|
| Common | 55% | 1,000 |
| Uncommon | 25% | 2,500 |
| Rare | 12% | 5,000 |
| Epic | 6% | 10,000 |
| Legendary | 2% | 20,000 |

**Using it:**

| Action | How |
|--------|-----|
| Deposit a stack | Pick up matching items and **right-click** the Void Storage |
| Deposit everything matching | **Shift + Left-click** the Void Storage |
| Withdraw one stack | Empty cursor, **right-click** the Void Storage |
| Withdraw as much as fits | Empty cursor, **Shift + Right-click** the Void Storage |
| Build straight from it | Hold a block-type Void Storage and **right-click** to place. It stays in your hand and the count goes down |

## Homes

You start with **1 home**. Buy more from the `/upgrades` menu: up to 10 with money, and 20–25 with Gems. See [Gem Store & Upgrades](store.md#homes).

```
/sethome <name>     # set a home
/home <name>        # go to it
/upgrades           # buy more home slots
```

## Enderchest

Your vanilla enderchest gets a command unlock at **Landlord (#11)**, so you can open it anywhere:

```
/enderchest     # or /ec
```

## Player Warps

Not storage exactly, but worth mentioning here — **player warps** let you set public teleport points (great for your shop). You can buy slots with money from `/upgrades` ([prices](store.md#player-warp-slots)), and ranks also grant them:

| Warps | Unlocked at | Rank |
|:-----:|-------------|------|
| 1 | <span class="chip money">$33,000,000</span> | <span class="tier-epic">Count</span> (#20) |
| 2 | <span class="chip money">$42,000,000</span> | <span class="tier-legendary">Jarl</span> (#21) |
| 5 | <span class="chip money">$105,000,000</span> | <span class="tier-royal">Royal</span> (#25) |

```
/pwarp          # browse all player warps
/pwarp create <name>    # create one of your warps
```

See [Shops & Markets](../money/shops.md#get-more-foot-traffic-with-player-warps) for using warps to drive shop traffic.

## Quality-of-life storage commands

A few rank-unlocked helpers for managing items:

| Command | Does | Unlocks at |
|---------|------|-----------|
| `/dispose` | Open a trash GUI to delete junk | <span class="tier-rare">Patriarch</span> (#12) |
| `/condense` | Condense materials into blocks (charcoal too) | <span class="tier-uncommon">Mercenary</span> (#6) |
| `/bulkcraft` | Bulk-craft whole inventories into blocks | [Cyclops](store.md#bulk-crafting) donor rank |

---

**Next:** [Cosmetics & Pets →](cosmetics.md)
