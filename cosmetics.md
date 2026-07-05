# Creating a Town

This page walks you through founding and running your own town on TownifyMC, including the real costs you'll pay.

## Before you start

To **create a town** you need two things:

1. **The rank unlock.** Town creation unlocks at **Countryman (rank #5)** — that's <span class="chip money">$10,000</span> in total spent climbing the [rank ladder](../progression/ranks.md).
2. **The town cost.** Founding the town itself costs <span class="chip money">$2,500</span>.

!!! tip "Not ready yet? Join a town instead"
    If you can't afford to found your own town, **join an existing one** — it's free, instant, and a great way to learn the ropes. See [Towns & Nations](index.md) for how.

## Founding your town

Stand where you want your town's first claim and home block to be, then:

```
/town new <name>
```

This claims your starting plot and makes you the **mayor**. Choose your spot carefully — your first claim is your town's anchor.

### Essential first commands

```
/town                 # view your town's info panel
/town set spawn       # set where /town spawn teleports to
/town claim           # claim the chunk you're standing in
/town set perm ...     # configure who can build/use things
/town add <player>    # invite a player to your town
/town deposit <amount>    # put money in the town bank
```

## Claiming land

Your town protects **townblocks** (chunks). Here's how claiming works and what it costs:

| | Value |
|---|---|
| **Cost per claim** | <span class="chip money">$25</span> to start |
| **Cost increase** | +$1 per claim you own |
| **Max claim cost** | <span class="chip money">$250</span> |
| **Claims per resident** | 8 |
| **Max claim radius (one command)** | 4 |

In plain terms:

- Each chunk you claim costs a little **more** than the last (starting at $25, rising $1 each time, capped at $250).
- Your town can hold **8 townblocks per resident** — so the more members you recruit, the more land you can claim. A solo town is limited; a populous town can sprawl.
- You can also **purchase bonus townblocks** beyond your resident limit for <span class="chip money">$100</span> each (the price climbs as you buy more).

```
/town claim           # claim the current chunk
/town claim outpost   # claim a detached outpost (away from your town)
/town unclaim         # release the current chunk
```

!!! warning "Plan your layout"
    Because claims cost more as you grow and you're capped by resident count, **claim deliberately**. Grab the land you'll actually build on rather than claiming everything in sight early.

## Protecting your town

Once land is claimed, Towny protects it automatically — outsiders can't build, break, or open containers unless you grant permission. Tune access with:

```
/town set perm           # open the permission menu
/plot set perm           # per-plot permissions
/town toggle pvp         # enable/disable PvP in town
/town toggle explosion    # enable/disable explosions
```

### Plots and Quarters

- **Plots:** divide your town into plots and assign them to residents or set them for sale (`/plot forsale <price>`).
- **Quarters:** TownifyMC also runs **Quarters**, which lets you define sub-areas *within* a plot — handy for renting out shops or apartments inside a larger building. Use the Quarters commands to carve up and sell/rent smaller spaces.

## Running your town

A town is a small economy of its own:

- **Town bank:** claims and upkeep are paid from the town bank. Keep it funded with `/town deposit`.
- **Taxes:** set resident taxes (`/town set taxes <amount>`) to keep the bank topped up.
- **Upkeep:** towns pay **daily upkeep**. If the bank can't cover it, your town risks falling into ruin — so budget for it.
- **Ranks:** assign town ranks (assistant, etc.) to trusted members so they can help manage things.

!!! danger "Don't let your town go bankrupt"
    If your town can't pay upkeep, it can be **ruined**. A ruined town can be reclaimed for <span class="chip money">$500</span> within the grace period — but it's far easier to just keep the bank funded.

## Extra town features

TownifyMC layers several add-ons on top of standard Towny:

- **:material-airplane: TownyFlight** — lets eligible players fly within town claims (also tied to [rank perks](../progression/ranks.md) like Fly in Claims at Marquess).
- **:material-tent: Towny Camps** — set up temporary camps in the wilderness.
- **:material-book-open-variant: Towny Histories** — your town keeps a historical record.
- **:material-peace: Towny Pacifist** — towns can opt into a pacifist stance (relevant to [war](war.md)).
- **:material-menu: Towny Menus** — GUI menus for managing your town without memorizing commands.

---

**Next:** [Nations →](nations.md)
