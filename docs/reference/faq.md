# FAQ

Quick answers to the questions new players ask most. Can't find yours? Ask in [Discord](https://discord.gg/townify).

## Getting in

??? question "What's the server address?"
    Java and Bedrock both connect at `play.townifymc.xyz` (Bedrock uses the default port, `19132`). See [Connecting](../getting-started/connecting.md) for step-by-step instructions.

??? question "Can I play on Bedrock / mobile / console?"
    Yes! TownifyMC supports **crossplay** through Geyser. Bedrock players (mobile, console, Windows 10/11) share the same world as Java players. See [Connecting](../getting-started/connecting.md).

??? question "Do I need the latest Minecraft version?"
    Not exactly — the network runs ViaVersion, so a range of recent versions can connect. If you can't get in, update to the newest release.

??? question "I can't connect. What do I do?"
    Double-check the address (and port, on Bedrock), make sure your client is reasonably current, and check [Discord](https://discord.gg/townify) in case the server is restarting. The [Connecting](../getting-started/connecting.md) page has a full checklist.

## Money & ranks

??? question "How do I make money as a new player?"
    [Join a job](../progression/jobs.md) and work it — that's your main income. Then [vote daily](../rewards/voting.md) and do your [daily quests](../progression/quests.md) for free bonus cash. Full breakdown: [Ways to Earn](../money/making-money.md).

??? question "How do I rank up?"
    Save up money and run `/rankup`. Each rank costs more than the last (Pleb is free, the next is $500, and so on up to $160M for Celestial). Open `/ranks` to see your progress, and turn on **auto rank-up** so it happens automatically. See [The Rank Ladder](../progression/ranks.md).

??? question "What's the difference between Money and Gems?"
    **Money** (`$`) runs the main economy — ranks, shops, towns. **Gems** are a premium currency for the Gem Store and top-tier upgrades. Full details: [Economy & Currencies](../progression/economy.md).

??? question "How many jobs can I have?"
    You start with **1** job slot. A **2nd** unlocks at Merchant (rank #7) and a **3rd** at Duke (rank #23). See [Jobs](../progression/jobs.md).

??? question "When can I fly?"
    Flight unlocks gradually at high ranks: **Fly in Claims** at Marquess (#22), **Wilderness Fly** at Royal (#25), and **Global Fly** at Celestial (#27). See [The Rank Ladder](../progression/ranks.md).

??? question "What's the fastest way to learn the commands?"
    Open `/menu` and click around; nearly everything is linked from there. For typed shortcuts, see [Useful Commands & Shortcuts](shortcuts.md).

??? question "Can I earn money while AFK?"
    Only in the **AFK Pool**, which pays $200–$1,000 an hour, and a separate pool gives a Vote Crate key every 90 minutes. Macros or AFK-bypass tricks anywhere else break the rules. See [Events & Minigames](../rewards/events.md#afk-pool).

??? question "How do I get Gems?"
    Win [chat games](../rewards/events.md#chat-games), place in [fishing competitions](../money/fishing.md), open crates, join events, or buy them on the [store](https://townify.tebex.io/category/gems). Spend them in the [Gem Store](../perks/store.md) (`/servershop`).

## Towns

??? question "How do I make a town?"
    First reach **Countryman (rank #5)** to unlock town creation, then run `/town new <name>`. Founding the town costs **$2,500**. Full guide: [Creating a Town](../towns/towns.md).

??? question "Do I have to make my own town?"
    No — **joining an existing town** is free, instant, and the easiest path for new players. Ask in [Discord](https://discord.gg/townify) or browse the [live map](https://map.townifymc.xyz) for towns recruiting. See [Towns & Nations](../towns/index.md).

??? question "How much does claiming land cost?"
    Claims start at **$25** and rise **$1** per claim you own, capped at **$250**. Your town can hold **8 townblocks per resident**, so recruiting members lets you claim more. See [Creating a Town](../towns/towns.md).

??? question "Can someone grief or raid my town?"
    Towny protects your claimed land from griefing. War happens **only** through the official [Siege War](../towns/war.md) system — which fights for control, **not** by destroying your builds. Working around protection to grief is against the [rules](../getting-started/rules.md).

??? question "My friend can't build on my land or open my chests. How do I share?"
    Add them with `/res friend add <player>` and turn on `/plot set perm friend on`, then look at a chest and run `/cmodify <player>`. Full guide: [Collaboration & Sharing](../towns/collaboration.md).

??? question "Why won't my hopper pull items out of my chest?"
    Locked containers block hoppers by default. Run `/chopper on` and left-click the container, then do the same for every locked container in the setup. See [Letting hoppers use locked containers](../towns/collaboration.md#letting-hoppers-use-locked-containers).

??? question "What are Town Deeds?"
    Reward items that add **+1, +3, +5, or +10** bonus claim chunks to your town. Right-click one while you're in a town. See [Creating a Town](../towns/towns.md#town-deeds).

??? question "My town fell into ruin — can I get it back?"
    A ruined town can be reclaimed for **$500** within the grace period. To avoid this, keep your town bank funded so it can pay daily upkeep. See [Creating a Town](../towns/towns.md).

## Rewards & items

??? question "How do I vote and what do I get?"
    Run `/vote`, click each site link, and enter your username. You get **money and crate keys** — every day. There are also vote parties, streaks, and milestones. See [Voting](../rewards/voting.md).

??? question "Where are the crates and how do I open them?"
    Crates are at `/warp crates`. Right-click a crate while holding its matching **key** (keys are physical items) — the [Vote Crate](../rewards/crates.md) key comes free from daily voting. See [Crates](../rewards/crates.md).

??? question "I died — did I lose my stuff?"
    Probably not! TownifyMC has **death chests (graves)** — your items are stored at your death location for you to recover. Head back reasonably promptly, as graves expire after a timer. See [Cosmetics & Pets → Death Chests](../perks/cosmetics.md#death-chests-graves).

??? question "How do I get more storage space?"
    Several ways, mostly rank-unlocked: **player vaults** (`/pv`), **backpacks**, and your **enderchest** (`/ec`). See [Storage & Backpacks](../perks/storage.md).

## World & travel

??? question "Where should I mine and gather?"
    In the **Resource World** (`/rw`, or `/nrw` for the Nether). It has no hostile mobs and resets about every 30 days, so don't build there. See [Travel & Worlds](../world/travel.md#the-resource-world).

??? question "How do I get to a specific part of the world?"
    Use `/rtp <continent>`, for example `/rtp europe` or `/rtp asia`. See [Random teleport](../world/travel.md#random-teleport-rtp).

??? question "Why do I suddenly walk faster?"
    You're on a player-built **road**. Trails, roads, and highways give +25%, +50%, and +75% speed. Turn it off with `/roadspeed`. See [Roads](../world/travel.md#roads-travel-faster).

??? question "Can I rent a shop without a town?"
    Yes. Rent a **market stall** at `/warp market` for $100/day (corner stalls $500/day). See [Shops & Markets](../money/shops.md#rent-a-market-stall).

## Other

??? question "Is there a map I can look at?"
    Yes — the live map is at [map.townifymc.xyz](https://map.townifymc.xyz). Great for scouting land and finding towns.

??? question "How do I report a player or a bug?"
    Open a ticket in our [Discord](https://discord.gg/townify). For bugs, **report them** rather than abusing them — exploiting bugs is against the [rules](../getting-started/rules.md).

??? question "Can I get my Java and Bedrock accounts linked?"
    Account linking may be available so both editions share your progress. Ask staff or check [Discord](https://discord.gg/townify). See [Connecting](../getting-started/connecting.md).

---

!!! tip "Still stuck?"
    The fastest way to get help is our [Discord](https://discord.gg/townify) — staff and friendly players are usually around to answer questions.
