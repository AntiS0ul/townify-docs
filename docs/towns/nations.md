# Nations

Once your town is established, the next step is joining or founding a **nation** — a union of towns under a single banner. Nations are where the server's politics, alliances, and large-scale conflicts play out.

## Unlocking nations

Creating a nation unlocks at **Warrior (rank #10)** — <span class="chip money">$500,000</span> in total rank progression. Founding the nation also has a Towny cost paid from your town bank.

!!! tip
    You don't need to *found* a nation to be part of one. Any town can be **invited into** an existing nation — often a faster route to the benefits of nationhood.

## Founding a nation

As a **mayor**, with your town as the future capital:

```
/nation new <name>
```

Your town becomes the **capital** and you become the **king/leader**. Other towns can then be invited to join.

### Core nation commands

```
/nation                  # view your nation's info panel
/nation add <town>       # invite a town to your nation
/nation set capital <town>    # designate the capital
/nation set spawn        # set the nation spawn
/nation deposit <amount>      # fund the nation bank
/nation ally add <nation>     # propose an alliance
/nation enemy add <nation>    # declare a nation an enemy
```

## Why join a nation?

| Benefit | What it means |
|---------|---------------|
| **Strength in numbers** | Allied towns support each other in [war](war.md) |
| **Diplomacy** | Form alliances, declare enemies, negotiate |
| **Shared identity** | A nation tag and shared spawn network |
| **Bigger bonuses** | Nations can unlock perks scaling with size |
| **Fast travel** | Cheaper/possible travel between allied and nation spawns |

### Spawn travel costs

Travelling to spawns across the nation/alliance network has small fees:

| Travel to… | Cost |
|------------|------|
| Your own town spawn | <span class="chip money">Free</span> |
| A town in your nation | <span class="chip money">$5</span> |
| An allied town's spawn | <span class="chip money">$10</span> |
| A public town's spawn | <span class="chip money">$10</span> |

```
/town spawn              # your town
/town spawn <town>       # another town (cost depends on relationship)
/nation spawn            # your nation's capital spawn
```

## Diplomacy & neutrality

Nations choose how they engage with the world:

- **Allies** fight alongside you and can use each other's spawns cheaply.
- **Enemies** can be targeted in (and target you with) [Siege War](war.md).
- **Neutrality** — a nation or town can declare itself neutral to stay out of conflicts, for a fee (town neutrality costs <span class="chip money">$25</span>).

!!! note "Politics is player-driven"
    Alliances, rivalries, and wars are created by **players**, not staff. Who you ally with and who you fight is up to you — that emergent politics is a big part of what makes a Towny server fun.

---

**Next:** [Sieges & War →](war.md)
