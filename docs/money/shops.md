# Shops & Markets

TownifyMC has a **fully player-driven economy** — everything is bought and sold **by players**, which means real supply and demand, prices that move, and genuine opportunities to profit if you pay attention. Here's how each marketplace works and when to use it.

## Player markets

**Player markets** are the heart of the economy — a marketplace where players list goods for others to buy. This is where supply, demand, and real prices live.

```
/market         # browse player markets :material-wrench:
/markets        # alternative :material-wrench:
```

Categories cover the full range — building blocks, tools, food, decoration, and more. Because every listing is set by a player, prices vary: shop around, compare sellers, and you'll often find a bargain (or a gap you can undercut and profit from).

!!! tip "Selling here is your main income from goods"
    **Player markets and the [auction house](#the-auction-house) are how you turn gathered resources into money.** Keep an eye on what's in demand and price to move volume.

## Setting up your own shop

Want **passive income**? Run your own storefront so players can buy from you even while you're offline.

To set up a shop you'll generally need:

1. **A town plot** you own (or permission to build in one). See [Creating a Town](../towns/towns.md).
2. **Stock** — items players actually want.
3. **A shop setup** — typically chest shops or a market listing, depending on the system.

!!! tip "What sells well"
    - **Building blocks** in bulk (always in demand for big builds)
    - **Food** (everyone needs to eat)
    - **Enchanted gear and books**
    - **Rare drops and event items**
    - **Spawners** and farm products

Price competitively — watch your neighbors' prices and undercut where it makes sense. A well-stocked, fairly-priced shop in a busy town is excellent passive money, and in a player-run economy a reliable supplier earns repeat customers.

### Get more foot traffic with Player Warps

TownifyMC has **player warps**, which let you create a public warp point others can teleport to — perfect for driving customers to your shop.

```
/pwarp          # browse player warps
/pwarp set <name>    # create a warp (rank-gated) :material-wrench:
```

The number of player warps you can own scales with your [rank](../progression/ranks.md): your first at **Count (#20)**, a second at **Jarl (#21)**, and up to **5 at Royal (#25)**. A warp named for your shop ("MegaBuild Blocks") pulls in buyers from across the map.

## The auction house

For **rare, high-value, one-off items**, use the auction house — list something and let the whole server bid or buy it.

```
/ah             # open the auction house
/ah sell <price>     # list the item in your hand
```

- Best for items a fixed-price listing would **undervalue** — rare gear, special drops, event items.
- The whole server sees your listing, so you get true market value.
- Check `/ah` regularly for deals — other players list valuable things too, and bargains go fast.

## Which should I use?

```mermaid
graph TD
    Q{What are you doing?}
    Q -->|Buying anything| A[Player Markets / other players' shops]
    Q -->|Selling bulk common goods| B[Player Markets or your own shop]
    Q -->|Selling something rare/valuable| C[Auction House /ah]
    Q -->|Want passive income| D[Run a Player Shop + Player Warp]
```

| Situation | Use |
|-----------|-----|
| Buying items | **Player markets** / other players' shops |
| Selling lots of common items | **Player markets** / your own shop |
| Selling a rare, valuable item | **Auction house** (`/ah`) |
| Building passive income | **Your own shop** + a **player warp** |

!!! note "It's all players"
    Since the economy is entirely player-run, **the best prices come from paying attention** — to what's in demand, what's overpriced, and where there's no seller yet. That gap is your opportunity.

---

**Next:** [Fishing →](fishing.md)
