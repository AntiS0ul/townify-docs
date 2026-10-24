# Collaboration & Sharing

Everything you build and place on TownifyMC is protected by default. That's great against griefers, but it also means **friends can't help you until you give them access**. This page covers how to share your land, chests, shops, stalls, and warps with other players, and how to stay in touch while you work together.

!!! tip "Quick answer: “My friend can’t build / open my chest”"
    1. Add them as a **friend**: `/res friend add <player>`
    2. Let friends build on your plot: `/plot set perm friend on`
    3. Let them open your locked chest: look at the chest and run `/cmodify <player>`

## Who can do what, at a glance

| You want someone to… | Use |
|----------------------|-----|
| Live in and build in your town | `/town add <player>` (makes them a resident) |
| Build on **your** plot without joining your town | [Towny friends](#towny-friends) or [plot trust](#plot-trust) |
| Help run the town | [Town ranks](#town-ranks) like `assistant` |
| Open a specific chest, furnace, or barrel | [`/cmodify <player>`](#locked-containers-chests-furnaces-barrels) |
| Restock and manage one of your chest shops | [Shared shop members](#shared-chest-shops) |
| Use your rented market stall | [Stall members](#market-stalls) |
| Use your player warp while it's private | [Warp whitelist](#player-warps) |

## Land: Towny permissions

### Towny friends

Your **friends list** is the simplest way to share your own plots with people you trust.

```
/res friend add <player>       # add a friend
/res friend remove <player>    # remove a friend
/res friend list               # see your friends
```

Being on your friends list doesn't do anything by itself. You also have to switch on the **friend** permissions on your plots:

```
/plot set perm friend on              # friends can build, break, switch, and use items
/plot set perm friend build on        # or turn on one permission at a time
/plot set perm friend switch on       # doors, levers, buttons, etc.
/plot set perm friend itemuse on      # buckets, flint & steel, etc.
```

Run `/plot set perm` while standing in the plot. Use `/plot perm` to check what's currently allowed there.

### Plot trust

**Trusting** someone on a plot gives them access to **that plot only**, whatever its permission settings are. It's good for a builder helping on one project.

```
/plot trust add <player>       # trust a player on the plot you're standing in
/plot trust remove <player>    # take it away
```

### Permission groups explained

Towny permissions are split into **who** and **what**:

| Who | Means |
|-----|-------|
| `resident` | Members of the town that owns the plot |
| `friend` | Players on the plot owner's friends list |
| `ally` | Members of allied towns and nations |
| `outsider` | Everyone else |

| What | Covers |
|------|--------|
| `build` | Placing blocks |
| `destroy` | Breaking blocks |
| `switch` | Doors, trapdoors, buttons, levers, gates |
| `itemuse` | Using items like buckets, flint & steel, and bone meal |

Combine them: `/plot set perm ally switch on` lets allies use doors on your plot, and `/town set perm outsider build off` makes sure outsiders can't build anywhere in town.

### Town ranks

Mayors can hand out **town ranks** so trusted residents can help manage the town:

```
/town rank add <player> <rank>       # give a rank
/town rank remove <player> <rank>    # take it away
/town ranklist                       # see who has which rank
```

Town ranks on TownifyMC: **assistant**, **helper**, **sheriff**, **vip**, and **donator**. An **assistant** gets most of the mayor's powers, such as inviting and kicking residents and claiming land, so only give it to people you really trust.

### Quarters: sharing part of a plot

[Quarters](towns.md#plots-and-quarters) let you mark out a room or apartment *inside* a plot and give it its own owner and trusted players. It's handy for shared buildings where everyone gets their own space. Run `/q` in game to see the Quarters commands.

!!! warning "Access isn't permission to grief"
    Being trusted, ranked, or added as a friend does **not** give anyone permission to steal from or damage the build. Abusing access breaks the [server rules](../getting-started/rules.md#claims-towns-griefing), so give access only to people you trust.

## Locked containers (chests, furnaces, barrels)

Containers you place **inside a town** are **locked to you automatically**. That includes chests, trapped chests, copper chests, barrels, furnaces, blast furnaces, smokers, droppers, dispensers, crafters, lecterns, composters, decorated pots, and shelves. Even your own town's residents can't open them unless you add them.

Look at the container and run:

| Command | Does |
|---------|------|
| `/cmodify <player>` | Give a player access to this container |
| `/cmodify -<player>` | Take a player's access away |
| `/cinfo` | See who owns it and who has access |
| `/cpublic` | Make it usable by anyone |
| `/cprivate` | Make it private again (just you plus anyone you add) |
| `/cpassword <password>` | Lock it with a password instead (others unlock it with `/cunlock <password>`) |
| `/cremove` | Remove the lock completely |
| `/chopper on` · `/chopper off` | Allow or block **hoppers** moving items in and out of it |

After you type the command, **left-click the container** if you're asked to select it.

### Letting hoppers use locked containers

Locked containers **block hoppers** by default, so nobody can drain your chest with a hopper underneath it. That also stops your own **sorters, smelters, and farm collectors** from working with locked chests and furnaces.

To let hoppers move items in and out of a container you own, run the command and then **left-click the container**:

```
/chopper on     # allow hoppers on this container
/chopper off    # block hoppers again
```

Do this for **every** locked container in the system, such as the chest that feeds a hopper line, the furnace it feeds into, and the chest at the end. Check a container's settings with `/cinfo`.

!!! warning "Hoppers can be used to steal"
    With `/chopper on`, **anyone** who can place a hopper next to the container can pull items out of it. Only turn it on for containers inside your own protected plots, where outsiders can't place blocks.

!!! tip "Sharing a whole storage room?"
    Instead of running `/cmodify` on every chest, use **LWC Trust** to trust a player on **all** your locked containers at once. Containers placed in the wilderness, outside towns, aren't locked at all, so keep valuables inside your town.

## Shared chest shops

A [chest shop](../money/shops.md#setting-up-your-own-chest-shop) can have **members** who help you run it, which is great for town co-ops and business partners.

1. Open `/market myshops` and pick the shop.
2. Turn on **Shared shop mode**.
3. Add members by name, then set what each member is allowed to do.

Members can help restock, and you can **deposit or withdraw** the shop's revenue from the same menu. Turning shared mode off removes all members.

!!! note "Building shops on someone else's plot"
    To create a chest shop on a town plot that isn't yours, you need to be **trusted on that plot** (see [Plot trust](#plot-trust)).

## Market stalls

Rented a [market stall](../money/shops.md#rent-a-market-stall)? Add your business partners as **members** so they can build and stock it with you:

```
/arm            # open the stall menu → My regions → pick your stall → Members
```

The player you're adding must be **online**. The stall still belongs to you, so you're the one who pays the rent.

## Player warps

Each [player warp](../perks/storage.md#player-warps) has an access setting:

| Access | Who can use it |
|--------|----------------|
| **Public** | Everyone |
| **Whitelisted** | Only players you add to the warp's whitelist |
| **Private** | Only you |

Open `/pwarp`, go to **My Warps**, and edit the warp to change its access or manage the whitelist. A whitelisted warp is a handy private teleport to a shared base for your group.

## Staying in touch

| Command | Talks to |
|---------|----------|
| `/tc <message>` | Your **town** |
| `/nc <message>` | Your **nation** |
| `/ac <message>` | Your **alliance** |
| `/g <message>` | Everyone (global) |
| `/msg <player> <message>` | One player privately |

Type a channel command **on its own** (for example just `/tc`) to switch to that channel, so everything you type goes there until you switch back with `/g`.

**Proximity voice chat** works too if you install the *Simple Voice Chat* mod. Players within 48 blocks can hear you, and you can create a **voice group** in the mod's menu (press ++g++ by default) so your team can talk from anywhere.

---

**Related:** [Creating a Town](towns.md) · [Nations](nations.md) · [Shops & Markets](../money/shops.md)
