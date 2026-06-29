# Creating a Town

This page walks you through founding and running your own town on TownifyMC, using the values from the Towny configuration.

## Before you start

To **create a town** you need two things:

1. **The rank unlock.** Town creation unlocks at **Countryman (rank #5)**, which costs <span class="chip money">$10,000</span> in rank progression.
2. **The town cost.** Founding the town itself costs <span class="chip money">$2,500</span>.

!!! tip "Not ready yet? Join a town instead"
    Joining an existing town is free, instant, and a great way to learn Towny without paying the founding and claim costs yourself.

## Founding your town

```
/town new <name>
```

### Essential first commands

```
/town
/town set spawn
/town claim
/town set perm
/town add <player>
/town deposit <amount>
```

## Claiming land

Towny protects land in **townblocks**, which are standard 16x16 chunks.

| | Value |
|---|---|
| **Founding cost** | <span class="chip money">$2,500</span> |
| **Outpost cost** | <span class="chip money">$500</span> |
| **Cost per claim** | <span class="chip money">$25</span> to start |
| **Cost increase** | +$1 per claim you own |
| **Max claim cost** | <span class="chip money">$250</span> |
| **Claims per resident** | 8 townblocks |
| **Townblock size** | 16x16 blocks |
| **Max claim radius in one command** | 4 |
| **Bonus townblock cost** | <span class="chip money">$100</span>, increasing by 1.05x up to <span class="chip money">$250</span> |

```
/town claim
/town claim outpost
/town unclaim
```

## Protecting your town

```
/town set perm
/plot set perm
/town toggle pvp
/town toggle explosion
```

### Plots and Quarters

- **Plots:** divide your town into plots and assign them to residents or set them for sale with `/plot forsale <price>`.
- **Quarters:** TownifyMC runs Quarters, which lets you define smaller rentable or sellable areas inside a plot.

## Running your town

- **Town bank:** claims and upkeep are paid from the town bank. Keep it funded with `/town deposit`.
- **Taxes:** use `/town set taxes <amount>` if you want residents to help fund the town.
- **Daily upkeep:** towns pay <span class="chip money">$100</span> per claimed plot because plot-based upkeep is enabled.
- **Ruins:** if a town falls into ruin, reclaiming it costs <span class="chip money">$500</span>.
- **Neutrality:** town neutrality costs <span class="chip money">$25</span>.

## Extra town features

TownifyMC also runs TownyFlight, Towny Camps, Towny Histories, Towny Pacifist, Towny Menus, Quarters, Dynmap-Towny, and SiegeWar.

---

**Next:** [Nations ->](nations.md)
